# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a>Microsoft Graph zum Zugreifen auf Excel in einer Python-App verwenden

Sie können die Microsoft Graph-API zum Lesen und Aktualisieren von Arbeitsmappen verwenden, die in unterstützten Onlinespeicherplattformen gespeichert werden, einschließlich OneDrive und SharePoint. Die `Workbook`-Ressource (oder Excel-Datei) enthält alle anderen Excel-Ressourcen, und Ihre App kann über einfache Navigationen darauf zugreifen. 

Sie können auf eine Reihe von Excel-Objekten (wie Tabelle, Bereich oder Diagramm) mithilfe von standardmäßigen REST-APIs zugreifen, um Vorgänge zum Erstellen, Lesen, Aktualisieren und Löschen in der Abeitsmappe durchzuführen. Beispielsweise gibt `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
eine Sammlung von Arbeitsblattobjekten zurück, die Teil der Arbeitsmappe sind.    

In dieser Vorgehensweise wird beschrieben, wie Anforderungen an die Excel-REST-API aus einer Python-Web-App gestellt werden. 

##  <a name="prerequisites"></a>Voraussetzungen

* [Python 3.5.2](https://www.python.org/downloads/)
* [Flask-OAuthlib](https://github.com/lepture/flask-oauthlib)
* Ein [Geschäfts- oder Schulkonto](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. -->


## <a name="authorization-and-scopes"></a>Autorisierung und Bereiche
Sie können den [Azure AD v2.0-Endpunkt](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) verwenden, um Excel-REST-API-Aufrufe zu authentifizieren. Alle APIs benötigen den `Authorization: Bearer {access-token}`-HTTP-Header.   
  
Einer der folgenden [Berechtigungsbereiche](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) ist erforderlich, um die Excel-Ressource verwenden:

* Files.Read 
* Files.ReadWrite

## <a name="sessions-and-persistence"></a>Sitzungen und Beständigkeit

Excel-APIs können in einem der beiden folgenden Modi aufgerufen werden: 

1. Beständige Sitzung: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert. Dies ist die übliche Vorgehensweise. 
2. Nicht beständige Sitzung: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert. Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei  bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält. Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren. Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.   

Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header. 

## <a name="register-the-application-in-azure-active-directory"></a>Registrieren der Anwendung in Azure Active Directory

Sie müssen Ihre Anwendung zuerst registrieren und die Berechtigungen für die Verwendung von Microsoft Graph festlegen. Dann können Benutzer sich bei der Anwendung mit Geschäfts- oder Schulkonten anmelden.

### <a name="register-the-application"></a>Registrieren der App

Registrieren Sie eine App im Microsoft App-Registrierungsportal. Dadurch werden die ID und das Kennwort der App generiert, mit der bzw. dem Sie die App für die Authentifizierung konfigurieren.

1. Melden Sie sich beim [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.

2. Klicken Sie auf **App hinzufügen**.

3. Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.

    Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.

4. Kopieren Sie die Anwendungs-ID: Dies ist der eindeutige Bezeichner für Ihre App.

5. Wählen Sie unter **Anwendungsgeheimnisse** die Option **Neues Kennwort generieren** aus. Kopieren Sie das Anwendungsgeheimnis aus dem Dialogfeld **Neues Kennwort wurde generiert**.

    Sie werden die ID und das Geheimnis der Anwendung verwenden, um die App zu konfigurieren.

6. Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** > **Web** aus.

7. Stellen Sie sicher, dass das Kontrollkästchen **Impliziten Fluss zulassen** aktiviert ist, und geben Sie den Umleitungs-URI der App ein.

    Die Option **Impliziten Fluss zulassen** ermöglicht den OpenID Connect-Hybridfluss. Während der Authentifizierung ermöglicht dies der App, sowohl Anmeldeinformationen (das **id_token**) als auch Artefakte (in diesem Fall ein Autorisierungscode) abzurufen, den die App zum Abrufen eines Zugriffstokens verwendet.

8. Wählen Sie **Speichern** aus.

### <a name="create-oauth-client"></a>Erstellen eines OAuth-Clients

Ihre App muss eine Instanz des Flask-OAuth-Clients registrieren, den Sie zum Starten des OAuth-Flusses und zum Abrufen eines Zugriffstokens verwenden werden. Beachten Sie, dass der Bereich *Files.ReadWrite* erforderlich ist, um eine Excel-Sitzung abzurufen, die beibehaltene Änderungen unterstützt.

```python
    # Put your consumer key and consumer secret into a config file
    # and don't check it into github!
    microsoft = oauth.remote_app(
        'microsoft',
        consumer_key = client_id,
        consumer_secret = client_secret,
        request_token_params = {'scope': 'User.Read Files.ReadWrite'},
        base_url = 'https://graph.microsoft.com/v1.0/',
        request_token_url = None,
        access_token_method = 'POST',
        access_token_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/token',
        authorize_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
    )
```

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a>Erhalten eines Autorisierungscodes auf Ihrer Antwort-URL-Seite

Nachdem sich der Benutzer angemeldet hat, wird der Browser an Ihre Antwort-URL umgeleitet. Nach erfolgreicher Autorisierung wird das Zugriffstoken (das zum Autorisieren zusätzlicher Anforderungen verwendet wird) in dem Antworttext zurückgegeben. 

```python
    @app.route('/login/authorized')
    def authorized():
        response = microsoft.authorized_response()
        if response is None:
            return "Access Denied: Reason=%s\nError=%s" % (
                request.args['error'], 
                request.args['error_description']
            )
    
        # Check response for state
        if str(session['state']) != str(request.args['state']):
            raise Exception('State has been messed with, end authentication')
        # Remove state session variable to prevent reuse.
        session['state'] = ""
            
        # Okay to store this in a local variable, encrypt if it's going to client
        # machine or database. Treat as a password. 
        session['microsoft_token'] = (response['access_token'], '')
        # Store the token in another session variable for easy access
        session['access_token'] = response['access_token']
```

## <a name="make-requests-to-the-excel-api"></a>Stellen von Anforderungen an die Excel-API

### <a name="request-headers"></a>Anforderungsheader 
Mit einem Zugriffstoken kann Ihre App authentifizierte Anforderungen an die Microsoft Graph-API senden. Ihre App muss das Zugriffstoken an den **Autorisierungs**-Header jeder Anforderung anfügen.

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
```
> **Hinweis** Die Anforderung muss auch einen Header des Typs **Content-Type** mit einem Wert senden, der von der Graph-API akzeptiert wird, z. B. `application/json`.

### <a name="getting-an-excel-session"></a>Abrufen einer Excel-Sitzung
#### <a name="request"></a>Anforderung 

Übergeben Sie ein JSON-Objekt durch Festlegen des `persistChanges`-Wert auf `true` oder `false`. Wenn der Wert von `persistChanges` auf `false` festgelegt wird, wird eine nicht beständige Sitzungs-ID zurückgegeben. In diesem Beispiel wird die HTTP-Bibliothek [Anforderungen](http://docs.python-requests.org/en/latest/user/quickstart) verwendet. 

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/createSession'
    # Set request headers
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
    # Specify type of session
    body = {
        'persistChanges': True
    }
    
    response = requests.post(url, headers = headers, json = body)
```

#### <a name="response"></a>Antwort

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
    "id": "{session-id}",
    "persistChanges": true
}
```

#### <a name="usage"></a>Verwendung 

Die vom vorherigen Aufruf zurückgegebene Sitzungs-ID wird als Header in nachfolgenden API-Anforderungen im HTTP-Header **Workbook-Session-Id** übergeben. Beispielsweise, um Arbeitsblätter in dieser Excel-Arbeitsmappe aufzuführen.

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/worksheets'
    # Set request headers - note the session header 
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Workbook-Session-Id': 'cluster=PP1&session=12.a04039942e021.A272...'
    }
    
    response = requests.get(url, headers = headers)
```

#### <a name="response"></a>Antwort

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets",
    "value": [
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0000-000000000000}",
        "name": "Session 1",
        "position": 0,
        "visibility": "Visible"
    },
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0100-000000000000}",
        "name": "Session 2",
        "position": 1,
        "visibility": "Visible"
    }]
}
```

## <a name="next-steps"></a>Nächste Schritte

Mit dem HTTP-Header **Workbook-Session-Id** können Sie beginnen, Anforderungen zum Abrufen von Daten, zum Erstellen von Diagrammen usw. auszustellen. 

* [Häufige Excel-API-Szenarien](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [Arbeiten mit Excel in Microsoft Graph](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

Die Excel-REST-API in Microsoft Graph bietet eine leistungsfähige Möglichkeit für den Zugriff auf und die Interaktion mit Daten in Excel-Arbeitsmappen. Finden Sie heraus, welche weiteren Vorteile Microsoft Graph bietet.

* [Übersicht über Microsoft Graph](https://developer.microsoft.com/graph/docs)
* [Erste Schritte mit Microsoft Graph in einer Python-App](https://developer.microsoft.com/graph/docs/get-started/python)
