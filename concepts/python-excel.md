# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a><span data-ttu-id="529ca-101">Microsoft Graph zum Zugreifen auf Excel in einer Python-App verwenden</span><span class="sxs-lookup"><span data-stu-id="529ca-101">Use Microsoft Graph to access Excel in a Python app</span></span>

<span data-ttu-id="529ca-102">Sie können die Microsoft Graph-API zum Lesen und Aktualisieren von Arbeitsmappen verwenden, die in unterstützten Onlinespeicherplattformen gespeichert werden, einschließlich OneDrive und SharePoint.</span><span class="sxs-lookup"><span data-stu-id="529ca-102">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The  (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> <span data-ttu-id="529ca-103">Die `Workbook`-Ressource (oder Excel-Datei) enthält alle anderen Excel-Ressourcen, und Ihre App kann über einfache Navigationen darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="529ca-103">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The `Workbook` (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> 

<span data-ttu-id="529ca-104">Sie können auf eine Reihe von Excel-Objekten (wie Tabelle, Bereich oder Diagramm) mithilfe von standardmäßigen REST-APIs zugreifen, um Vorgänge zum Erstellen, Lesen, Aktualisieren und Löschen in der Abeitsmappe durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="529ca-104">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, </span></span> <span data-ttu-id="529ca-105">Beispielsweise gibt `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span><span class="sxs-lookup"><span data-stu-id="529ca-105">For example:`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span></span>  
<span data-ttu-id="529ca-106">eine Sammlung von Arbeitsblattobjekten zurück, die Teil der Arbeitsmappe sind.</span><span class="sxs-lookup"><span data-stu-id="529ca-106">returns a collection of worksheet objects that are part of the workbook.</span></span>    

<span data-ttu-id="529ca-107">In dieser Vorgehensweise wird beschrieben, wie Anforderungen an die Excel-REST-API aus einer Python-Web-App gestellt werden.</span><span class="sxs-lookup"><span data-stu-id="529ca-107">This walkthrough describes how to make requests to the Excel REST API from a Python web app.</span></span> 

##  <a name="prerequisites"></a><span data-ttu-id="529ca-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="529ca-108">Prerequisites</span></span>

* [<span data-ttu-id="529ca-109">Python 3.5.2</span><span class="sxs-lookup"><span data-stu-id="529ca-109">Python 3.5.2</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="529ca-110">Flask-OAuthlib</span><span class="sxs-lookup"><span data-stu-id="529ca-110">Flask-OAuthlib</span></span>](https://github.com/lepture/flask-oauthlib)
* <span data-ttu-id="529ca-111">Ein [Geschäfts- oder Schulkonto](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span><span class="sxs-lookup"><span data-stu-id="529ca-111">A [work or school account](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span></span>


## <a name="authorization-and-scopes"></a><span data-ttu-id="529ca-112">Autorisierung und Bereiche</span><span class="sxs-lookup"><span data-stu-id="529ca-112">Authorization and scopes</span></span>
<span data-ttu-id="529ca-113">Sie können den [Azure AD v2.0-Endpunkt](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) verwenden, um Excel-REST-API-Aufrufe zu authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="529ca-113">You can use the [Azure AD v2.0 endpoint](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) to authenticate Excel REST API calls. All APIs require the  HTTP header.</span></span> <span data-ttu-id="529ca-114">Alle APIs benötigen den `Authorization: Bearer {access-token}`-HTTP-Header.</span><span class="sxs-lookup"><span data-stu-id="529ca-114">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="529ca-115">Einer der folgenden [Berechtigungsbereiche](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) ist erforderlich, um die Excel-Ressource verwenden:</span><span class="sxs-lookup"><span data-stu-id="529ca-115">One of the following [permission scopes](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) is required to use the Excel resource:</span></span>

* <span data-ttu-id="529ca-116">Files.Read</span><span class="sxs-lookup"><span data-stu-id="529ca-116">Files.Read</span></span> 
* <span data-ttu-id="529ca-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="529ca-117">Files.ReadWrite</span></span>

## <a name="sessions-and-persistence"></a><span data-ttu-id="529ca-118">Sitzungen und Beständigkeit</span><span class="sxs-lookup"><span data-stu-id="529ca-118">Sessions and persistence</span></span>

<span data-ttu-id="529ca-119">Excel-APIs können in einem der beiden folgenden Modi aufgerufen werden:</span><span class="sxs-lookup"><span data-stu-id="529ca-119">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="529ca-p104">Beständige Sitzung: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert. Dies ist die übliche Vorgehensweise.</span><span class="sxs-lookup"><span data-stu-id="529ca-p104">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="529ca-p105">Nicht beständige Sitzung: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert. Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei  bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält. Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren. Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.</span><span class="sxs-lookup"><span data-stu-id="529ca-p105">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="529ca-126">Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header.</span><span class="sxs-lookup"><span data-stu-id="529ca-126">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

## <a name="register-the-application-in-azure-active-directory"></a><span data-ttu-id="529ca-127">Registrieren der Anwendung in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="529ca-127">Register the application in Azure Active Directory</span></span>

<span data-ttu-id="529ca-p106">Sie müssen Ihre Anwendung zuerst registrieren und die Berechtigungen für die Verwendung von Microsoft Graph festlegen. Dann können Benutzer sich bei der Anwendung mit Geschäfts- oder Schulkonten anmelden.</span><span class="sxs-lookup"><span data-stu-id="529ca-p106">First, you need to register your application and set permissions to use Microsoft Graph. This lets users sign in to the application with work or school accounts.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="529ca-130">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="529ca-130">Register the application</span></span>

<span data-ttu-id="529ca-p107">Registrieren Sie eine App im Microsoft App-Registrierungsportal. Dadurch werden die ID und das Kennwort der App generiert, mit der bzw. dem Sie die App für die Authentifizierung konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="529ca-p107">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="529ca-133">Melden Sie sich beim [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="529ca-133">Sign in to the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="529ca-134">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="529ca-134">Choose **Add an app**.</span></span>

3. <span data-ttu-id="529ca-135">Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="529ca-135">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="529ca-136">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="529ca-136">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="529ca-p108">Kopieren Sie die Anwendungs-ID: Dies ist der eindeutige Bezeichner für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="529ca-p108">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="529ca-p109">Wählen Sie unter **Anwendungsgeheimnisse** die Option **Neues Kennwort generieren** aus. Kopieren Sie das Anwendungsgeheimnis aus dem Dialogfeld **Neues Kennwort wurde generiert**.</span><span class="sxs-lookup"><span data-stu-id="529ca-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>

    <span data-ttu-id="529ca-141">Sie werden die ID und das Geheimnis der Anwendung verwenden, um die App zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="529ca-141">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="529ca-142">Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** > **Web** aus.</span><span class="sxs-lookup"><span data-stu-id="529ca-142">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="529ca-143">Stellen Sie sicher, dass das Kontrollkästchen **Impliziten Fluss zulassen** aktiviert ist, und geben Sie den Umleitungs-URI der App ein.</span><span class="sxs-lookup"><span data-stu-id="529ca-143">Make sure the **Allow Implicit Flow** check box is selected, and enter your app's Redirect URI.</span></span>

    <span data-ttu-id="529ca-144">Die Option **Impliziten Fluss zulassen** ermöglicht den OpenID Connect-Hybridfluss.</span><span class="sxs-lookup"><span data-stu-id="529ca-144">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow.</span></span> <span data-ttu-id="529ca-145">Während der Authentifizierung ermöglicht dies der App, sowohl Anmeldeinformationen (das **id_token**) als auch Artefakte (in diesem Fall ein Autorisierungscode) abzurufen, den die App zum Abrufen eines Zugriffstokens verwendet.</span><span class="sxs-lookup"><span data-stu-id="529ca-145">During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app can use to obtain an access token.</span></span>

8. <span data-ttu-id="529ca-146">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="529ca-146">Choose **Save**.</span></span>

### <a name="create-oauth-client"></a><span data-ttu-id="529ca-147">Erstellen eines OAuth-Clients</span><span class="sxs-lookup"><span data-stu-id="529ca-147">Create OAuth client</span></span>

<span data-ttu-id="529ca-148">Ihre App muss eine Instanz des Flask-OAuth-Clients registrieren, den Sie zum Starten des OAuth-Flusses und zum Abrufen eines Zugriffstokens verwenden werden.</span><span class="sxs-lookup"><span data-stu-id="529ca-148">Your app needs to register an instance of the Flask-OAuth client that you'll use to start the OAuth flow and get an access token.</span></span> <span data-ttu-id="529ca-149">Beachten Sie, dass der Bereich *Files.ReadWrite* erforderlich ist, um eine Excel-Sitzung abzurufen, die beibehaltene Änderungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="529ca-149">Note that the *Files.ReadWrite* scope is required to obtain an Excel session that supports persisted changes.</span></span>

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

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a><span data-ttu-id="529ca-150">Erhalten eines Autorisierungscodes auf Ihrer Antwort-URL-Seite</span><span class="sxs-lookup"><span data-stu-id="529ca-150">Receive an authorization code in your reply URL page</span></span>

<span data-ttu-id="529ca-p112">Nachdem sich der Benutzer angemeldet hat, wird der Browser an Ihre Antwort-URL umgeleitet. Nach erfolgreicher Autorisierung wird das Zugriffstoken (das zum Autorisieren zusätzlicher Anforderungen verwendet wird) in dem Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="529ca-p112">After the user signs in, the browser is redirected to your reply URL. Upon successful authorization, the access token (which will be used to authorize additional requests) will be returned in the response body.</span></span> 

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

## <a name="make-requests-to-the-excel-api"></a><span data-ttu-id="529ca-153">Stellen von Anforderungen an die Excel-API</span><span class="sxs-lookup"><span data-stu-id="529ca-153">Make requests to the Excel API</span></span>

### <a name="request-headers"></a><span data-ttu-id="529ca-154">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="529ca-154">Request headers</span></span> 
<span data-ttu-id="529ca-p113">Mit einem Zugriffstoken kann Ihre App authentifizierte Anforderungen an die Microsoft Graph-API senden. Ihre App muss das Zugriffstoken an den **Autorisierungs**-Header jeder Anforderung anfügen.</span><span class="sxs-lookup"><span data-stu-id="529ca-p113">With an access token, your app can make authenticated requests to the Microsoft Graph API. Your app must append the access token to the **Authorization** header of each request.</span></span>

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
```
> <span data-ttu-id="529ca-157">**Hinweis** Die Anforderung muss auch einen Header des Typs **Content-Type** mit einem Wert senden, der von der Graph-API akzeptiert wird, z. B. `application/json`.</span><span class="sxs-lookup"><span data-stu-id="529ca-157">**Note** The request must also send a **Content-Type** header with a value accepted by the Graph API, for example, `application/json`.</span></span>

### <a name="getting-an-excel-session"></a><span data-ttu-id="529ca-158">Abrufen einer Excel-Sitzung</span><span class="sxs-lookup"><span data-stu-id="529ca-158">Getting an Excel Session</span></span>
#### <a name="request"></a><span data-ttu-id="529ca-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="529ca-159">Request</span></span> 

<span data-ttu-id="529ca-160">Übergeben Sie ein JSON-Objekt durch Festlegen des `persistChanges`-Wert auf `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="529ca-160">Pass a JSON object by setting the `persistChanges` value to `true` or `false`.</span></span> <span data-ttu-id="529ca-161">Wenn der Wert von `persistChanges` auf `false` festgelegt wird, wird eine nicht beständige Sitzungs-ID zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="529ca-161">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span> <span data-ttu-id="529ca-162">In diesem Beispiel wird die HTTP-Bibliothek [Anforderungen](http://docs.python-requests.org/en/latest/user/quickstart) verwendet.</span><span class="sxs-lookup"><span data-stu-id="529ca-162">This example uses the [Requests](http://docs.python-requests.org/en/latest/user/quickstart) HTTP library</span></span> 

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

#### <a name="response"></a><span data-ttu-id="529ca-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="529ca-163">Response</span></span>

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

#### <a name="usage"></a><span data-ttu-id="529ca-164">Verwendung</span><span class="sxs-lookup"><span data-stu-id="529ca-164">Usage</span></span> 

<span data-ttu-id="529ca-165">Die vom vorherigen Aufruf zurückgegebene Sitzungs-ID wird als Header in nachfolgenden API-Anforderungen im HTTP-Header **Workbook-Session-Id** übergeben.</span><span class="sxs-lookup"><span data-stu-id="529ca-165">The session ID returned from the previous call is passed as a header on subsequent API requests in the **Workbook-Session-Id** HTTP header. For instance, to list worksheets in that Excel workbook.</span></span> <span data-ttu-id="529ca-166">Beispielsweise, um Arbeitsblätter in dieser Excel-Arbeitsmappe aufzuführen.</span><span class="sxs-lookup"><span data-stu-id="529ca-166">For instance, to list worksheets in that Excel workbook.</span></span>

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

#### <a name="response"></a><span data-ttu-id="529ca-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="529ca-167">Response</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="529ca-168">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="529ca-168">Next steps</span></span>

<span data-ttu-id="529ca-169">Mit dem HTTP-Header **Workbook-Session-Id** können Sie beginnen, Anforderungen zum Abrufen von Daten, zum Erstellen von Diagrammen usw. auszustellen.</span><span class="sxs-lookup"><span data-stu-id="529ca-169">With the **Workbook-Session-Id** HTTP header, you can begin issuing requests to fetch data, create charts, and much more.</span></span> 

* [<span data-ttu-id="529ca-170">Häufige Excel-API-Szenarien</span><span class="sxs-lookup"><span data-stu-id="529ca-170">Common Excel API scenarios</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [<span data-ttu-id="529ca-171">Arbeiten mit Excel in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="529ca-171">Working with Excel in Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

<span data-ttu-id="529ca-p116">Die Excel-REST-API in Microsoft Graph bietet eine leistungsfähige Möglichkeit für den Zugriff auf und die Interaktion mit Daten in Excel-Arbeitsmappen. Finden Sie heraus, welche weiteren Vorteile Microsoft Graph bietet.</span><span class="sxs-lookup"><span data-stu-id="529ca-p116">The Excel REST API in Microsoft Graph provides a powerful way to access and interact with data in Excel workbooks. Explore what else is possible with Microsoft Graph.</span></span>

* [<span data-ttu-id="529ca-174">Übersicht über Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="529ca-174">Overview of Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs)
* [<span data-ttu-id="529ca-175">Erste Schritte mit Microsoft Graph in einer Python-App</span><span class="sxs-lookup"><span data-stu-id="529ca-175">Get started with Microsoft Graph in a Python app</span></span>](https://developer.microsoft.com/graph/docs/get-started/python)
