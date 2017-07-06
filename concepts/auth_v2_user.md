# <a name="get-access-on-behalf-of-a-user"></a>Im Namen eines Benutzers zugreifen
Um Microsoft Graph zum Lesen und Schreiben von Ressourcen im Namen eines Benutzers zu verwenden, muss Ihre App ein Zugriffstoken von Azure AD abrufen und das Token an Anforderungen anfügen, die die API an Microsoft Graph sendet. Welchen Authentifizierungsfluss genau Sie zum Abrufen von Zugriffstoken verwenden, ist davon abhängig, welche Art von App Sie entwickeln und ob Sie OpenID Connect zum Anmelden des Benutzers bei Ihrer App verwenden möchten. Ein Fluss, der häufig von systemeigenen und mobilen Apps und auch von einigen Web-Apps verwendet wird, ist der Fluss zur Erteilung von OAuth 2.0-Autorisierungscodes. In diesem Thema werden anhand eines Beispiels die einzelnen Schritte dieses Flusses erläutert. 

## <a name="authentication-and-authorization-steps"></a>Authentifizierungs- und Autorisierungsschritte

Um ein Zugriffstoken mit dem Fluss zur Erteilung von OAuth 2.0-Autorisierungscodes vom Azure AD v2.0-Endpunkt abzurufen, müssen die folgenden grundlegenden Schritte ausgeführt werden:

1. Registrieren der App bei Azure AD 
2. Abrufen eines Autorisierungscodes 
3. Abrufen eines Zugriffstokens
4. Aufrufen von Microsoft Graph mit dem Zugriffstoken
5. Abrufen eines neuen Zugriffstokens mithilfe eines Aktualisierungstokens

## <a name="1-register-your-app"></a>1. Registrieren der App
Für den Azure AD v2.0-Endpunkt müssen Sie Ihre App im [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) registrieren. Sie können entweder ein Microsoft-Konto oder ein Geschäfts-, Schul- oder Unikonto zum Registrieren einer App verwenden. 

Der folgende Screenshot zeigt ein Beispiel für eine Web-App-Registrierung. ![Web-App-Registrierung mit Kennwort und Zulassung des impliziten Flusses](./images/v2-web-registration.png)

Um eine App für die Verwendung des Flusses zur Erteilung von OAuth 2.0-Autorisierungscodes zu konfigurieren, müssen Sie beim Registrieren der App die folgenden Werte speichern:

- Die Anwendung-ID, die vom App-Registrierungsportal zugewiesen wurde.
- Ein Anwendungsgeheimnis, entweder ein Kennwort oder ein öffentliches/privates Schlüsselpaar (Zertifikat). Dies ist für systemeigene Apps nicht erforderlich. 
- Eine Umleitungs-URL, damit Ihre App Antworten von Azure AD empfangen kann.

Schritte zum Konfigurieren einer App mit dem Microsoft-App-Registrierungsportal finden Sie unter [Apps registrieren](./auth_register_app_v2.md).

## <a name="2-get-authorization"></a>2. Abrufen eines Autorisierungscodes
Der erste Schritt zum Abrufen eines Zugriffstokens für viele OpenID Connect- und OAuth 2.0-Flüsse besteht darin, den Benutzer zum Azure AD v2.0 `/authorize`-Endpunkt umzuleiten. Azure AD meldet den Benutzer an und sichert dessen Zustimmung zu den von der App angeforderten Berechtigungen. Im Fluss zur Erteilung von Autorisierungscodes gibt Azure AD nach Erhalt der Zustimmung einen Autorisierungscode an Ihre App zurück, den diese beim Azure AD v2.0 `/token`-Endpunkt für ein Zugriffstoken einlösen kann.

### <a name="authorization-request"></a>Autorisierungsanforderung 
Im Folgenden finden Sie ein Beispiel für eine an den `/authorize`-Endpunkt gesendete Anforderung. 

Beim Azure AD v2.0-Endpunkt werden Berechtigungen mit dem `scope`-Parameter angefordert. In diesem Beispiel werden die Microsoft Graph-Berechtigungen _User.Read_ und _Mail.Read_ angefordert, die es der App ermöglichen, das Profil und die E-Mails des angemeldeten Benutzers zu lesen. Die Berechtigung _offline\_access_ wird angefordert, damit die App ein Aktualisierungstoken abrufen kann, um nach Ablauf des aktuellen Zugriffstokens ein neues abzurufen. 

```
// Line breaks for legibility only

https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize?
client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&response_type=code
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&response_mode=query
&scope=offline_access%20user.read%20mail.read
&state=12345
```
| Parameter |  | Beschreibung |
| --- | --- | --- |
| tenant |Erforderlich |Mit dem Wert `{tenant}` im Pfad der Anforderung kann gesteuert werden, wer sich bei der Anwendung anmelden kann.  Die zulässigen Werte sind `common` für Microsoft-Konten und Geschäfts-, Schul- oder Unikonten, `organizations` nur für Geschäfts-, Schul- oder Unikonten, `consumers` nur für Microsoft-Konten und Mandantenbezeichner wie z. B. Mandanten-ID oder Domänenname.  Weitere Informationen finden Sie unter [Grundlagen zu Protokollen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id |erforderlich |Die Anwendungs-ID, die Ihrer App vom Registrierungsportal ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) zugewiesen wurde. |
| response_type |erforderlich |Muss `code` für den Autorisierungscodefluss enthalten. |
| redirect_uri |empfohlen |Der Umleitungs-URI Ihrer API, an den Authentifizierungsantworten gesendet und von Ihrer App empfangen werden können.  Er muss genau mit einem der Umleitungs-URIs übereinstimmen, die Sie im App-Registrierungsportal registriert haben, mit der Ausnahme, dass er URL-codiert sein muss.  Für systemeigene und mobile Apps sollten Sie den Standardwert `https://login.microsoftonline.com/common/oauth2/nativeclient` verwenden. |
| Umfang |Erforderlich |Eine mit Leerzeichen getrennte Liste von Microsoft Graph-Berechtigungen, denen der Benutzer zustimmen soll. Hierzu können auch OpenID-Bereiche gehören. |
| response_mode |empfohlen |Gibt die Methode an, die verwendet werden soll, um das resultierende Token an die App zurückzusenden.  Kann `query` oder `form_post` sein. |
| Zustand |empfohlen |Ein Wert, der in der Anforderung enthalten ist und ebenfalls in der Tokenantwort zurückgegeben wird.  Es kann eine Zeichenfolge beliebigen Inhalts sein.  In der Regel wird ein zufällig generierter eindeutiger Wert verwendet, um [websiteübergreifende Anforderungsfälschungsangriffe zu verhindern ](http://tools.ietf.org/html/rfc6749#section-10.12).  Der Status wird auch verwendet, um Informationen über den Status des Benutzers in der App vor dem Versand der Authentifizierungsanforderung zu codieren, z. B. die Seite oder die Ansicht, auf bzw. in der sich der Benutzer befunden hat. |

> **Wichtig**: Microsoft Graph stellt zwei Arten von Berechtigungen zur Verfügung: Anwendungsberechtigungen und delegierte Berechtigungen. Für Apps, die mit einem angemeldeten Benutzer ausgeführt werden, fordern Sie delegierte Berechtigungen im `scope`-Parameter an. Diese Berechtigungen delegieren die Rechte des angemeldeten Benutzers an Ihre Anwendung und ermöglichen es ihr, als der angemeldete Benutzer zu agieren, wenn Aufrufe an Microsoft Graph gesendet werden. Ausführliche Informationen zu den in Microsoft Graph verfügbaren Berechtigungen finden Sie in der [Berechtigungsreferenz](./permissions_reference.md).
 
### <a name="consent-experience"></a>Zustimmungsfunktionalität

An diesem Punkt wird der Benutzer aufgefordert, seine Anmeldeinformationen einzugeben, um sich bei Azure AD zu authentifizieren. Der v2.0-Endpunkt stellt außerdem sicher, dass der Benutzer den im `scope`-Parameter angegebenen Berechtigungen zugestimmt hat.  Wenn der Benutzer keiner dieser Berechtigungen zugestimmt hat und wenn nicht zuvor ein Administrator im Namen aller Benutzer in der Organisation seine Zustimmung erteilt hat, fordert Azure AD den Benutzer auf, den erforderlichen Berechtigungen zuzustimmen.  

Hier sehen Sie ein Beispiel für das Zustimmungsdialogfeld, das für ein Microsoft-Konto angezeigt wird:

![Zustimmungsdialogfeld für Microsoft-Konto](./images/v2-consumer-consent.png)

> **Versuchen Sie es** Wenn Sie über ein Microsoft-Konto oder ein Azure AD-Geschäfts-, Schul- oder Unikonto verfügen, können Sie dies selbst ausprobieren, indem Sie auf den nachstehenden Link klicken. Nach der Anmeldung sollte Ihr Browser zu `https://localhost/myapp/` mit einem `code` in der Adressleiste umgeleitet werden.
> 
> <a href="https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F&response_mode=query&scope=offline_access%20user.read%20mail.read&state=12345" target="_blank">https://login.microsoftonline.com/common/oauth2/v2.0/authorize...</a>

### <a name="authorization-response"></a>Autorisierungsantwort
Falls der Benutzer den von Ihrer App angeforderten Berechtigungen zustimmt, enthält die Antwort den Autorisierungscode im `code`-Parameter. Hier sehen Sie ein Beispiel einer erfolgreichen Antwort auf die vorstehende Anforderung. Da der `response_mode`-Parameter in der Anforderung auf `query` festgelegt wurde, wird die Antwort in der Abfragezeichenfolge der Umleitungs-URL zurückgegeben.

```
GET http://localhost/myapp/?
code=M0ab92efe-b6fd-df08-87dc-2c6500a7f84d
&state=12345
```
| Parameter | Beschreibung |
| --- | --- |
| code |Der von der App angeforderte Autorisierungscode. Mit diesem Autorisierungscode kann die App ein Zugriffstoken für die Zielressource anfordern.  Autorisierungscodes haben nur eine sehr kurze Gültigkeit, normalerweise laufen sie nach ca. 10 Minuten ab. |
| Zustand |Wenn ein Statusparameter in der Anforderung enthalten ist, sollte der gleiche Wert in der Antwort angezeigt werden. Die App sollte überprüfen, ob die Statuswerte in Anforderung und Antwort identisch sind. |

## <a name="3-get-a-token"></a>3. Abrufen eines Tokens
Ihre App verwendet den im vorherigen Schritt empfangenen Autorisierungs-`code` zum Anfordern eines Zugriffstokens; hierzu wird eine `POST`-Anforderung an den `/token`-Endpunkt gesendet.

### <a name="token-request"></a>Tokenanforderung
```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

| Parameter |  | Beschreibung |
| --- | --- | --- |
| tenant |Erforderlich |Mit dem Wert `{tenant}` im Pfad der Anforderung kann gesteuert werden, wer sich bei der Anwendung anmelden kann.  Die zulässigen Werte sind `common` für Microsoft-Konten und Geschäfts-, Schul- oder Unikonten, `organizations` nur für Geschäfts-, Schul- oder Unikonten, `consumers` nur für Microsoft-Konten und Mandantenbezeichner wie z. B. Mandanten-ID oder Domänenname.  Weitere Informationen finden Sie unter [Grundlagen zu Protokollen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id |erforderlich |Die Anwendungs-ID, die Ihrer App vom Registrierungsportal ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) zugewiesen wurde. |
| grant_type |erforderlich |Muss `authorization_code` für den Autorisierungscodefluss sein. |
| scope |Erforderlich |Eine mit Leerzeichen getrennte Liste von Bereichen.  Die Bereiche, die in diesem Zweig angefordert werden, müssen den im ersten Zweig (Autorisierung) angeforderten Bereichen entsprechen oder eine Teilmenge davon sein.  Wenn die in dieser Anforderung angegebenen Bereiche sich über mehrere Ressourcenserver erstrecken, gibt der v2.0-Endpunkt ein Token für die im ersten Bereich angegebene Ressource zurück. |
| code |erforderlich |Der Autorisierungscode, den Sie im ersten Zweig des Flusses abgerufen haben. |
| redirect_uri |erforderlich |Die gleiche Umleitungs-URI-Wert, der zum Abrufen des Autorisierungscodes verwendet wurde. |
| client_secret |erforderlich für Web-Apps |Das Anwendungsgeheimnis, das Sie im App-Registrierungsportal für Ihre App erstellt haben.  Es sollte nicht in einer systemeigenen App verwendet werden, da Anwendungsgeheimnisse nicht zuverlässig auf Geräten gespeichert werden können.  Es ist für Web-Apps und Web-APIs erforderlich, die die Möglichkeit haben, das Anwendungsgeheimnis sicher auf dem Server zu speichern. |

### <a name="token-response"></a>Tokenantwort
Obwohl das Zugriffstoken für Ihre App undurchsichtig ist, enthält die Antwort im `scope`-Parameter eine Liste der Berechtigungen, für die das Zugriffstoken gültig ist. 

```
{
    "token_type": "Bearer",
    "scope": "user.read%20Fmail.read",
    "expires_in": 3600,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4..."
}
```
| Parameter | Beschreibung |
| --- | --- |
| token_type |Gibt den Tokentypwert an. Der einzige von Azure AD unterstützte Typ ist „Bearer“. |
| Umfang |Eine mit Leerzeichen getrennte Liste der Microsoft Graph-Berechtigungen, für die das Zugriffstoken gültig ist. |
| expires_in |Gültigkeit des Zugriffstokens (in Sekunden). |
| access_token |Das angeforderte Zugriffstoken. Mit diesem Token kann Ihre App Microsoft Graph aufrufen. |
| refresh_token |Ein OAuth 2.0-Aktualisierungstoken. Mit diesem Token kann Ihre App zusätzliche Zugriffstoken anfordern, nachdem das aktuelle Zugriffstoken abgelaufen ist.  Aktualisierungstoken haben eine lange Lebensdauer und können verwendet werden, um für längere Zeit Zugriff auf Ressourcen zu behalten.  Ausführliche Informationen finden Sie in der [v2.0-Tokenreferenz](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-tokens). |

## <a name="4-use-the-access-token-to-call-microsoft-graph"></a>4. Aufrufen von Microsoft Graph unter Verwendung des Zugriffstokens

Sobald Sie über ein Zugriffstoken verfügen, können Sie damit Microsoft Graph aufrufen, indem Sie das Token in den `Authorization`-Header einer Anforderung einschließen. Die folgende Anforderung ruft das Profil des angemeldeten Benutzers ab.

```
GET https://graph.microsoft.com/v1.0/me 
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com

```
Eine erfolgreiche Antwort sieht ähnlich wie die folgende aus (einige Antwortheader wurden entfernt):

```
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 727.0022
Date: Thu, 20 Apr 2017 05:21:18 GMT
Content-Length: 407

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="5-use-the-refresh-token-to-get-a-new-access-token"></a>5. Abrufen eines neuen Zugriffstokens mithilfe eines Aktualisierungstokens

Zugriffstokens sind kurzlebig, und Sie müssen sie nach ihrem Ablauf aktualisieren, um weiterhin auf Ressourcen zugreifen zu können.  Hierzu können Sie eine weitere `POST`-Anforderung an den `/token`-Endpunkt senden, in der Sie das `refresh_token` anstelle des `code` angeben.

### <a name="request"></a>Anforderung
```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&refresh_token=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=refresh_token
&client_secret=JqQX2PNo9bpM0uEihUPzyrh      // NOTE: Only required for web apps
```

| Parameter |  | Beschreibung |
| --- | --- | --- |
| client_id |erforderlich |Die Anwendungs-ID, die Ihrer App vom Registrierungsportal ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) zugewiesen wurde. |
| grant_type |erforderlich |Muss `refresh_token` sein. |
| scope |Erforderlich |Eine mit Leerzeichen getrennte Liste von Berechtigungen (Bereichen).  Die angeforderten Berechtigungen müssen den im ursprünglichen Autorisierungscode angeforderten Berechtigungen entsprechen oder eine Teilmenge davon sein. |
| refresh_token |erforderlich |Das während der Tokenanforderung abgerufene Aktualisierungstoken. |
| redirect_uri |erforderlich |Die gleiche Umleitungs-URI-Wert, der zum Abrufen des Autorisierungscodes verwendet wurde. |
| client_secret |erforderlich für Web-Apps |Das Anwendungsgeheimnis, das Sie im App-Registrierungsportal für Ihre App erstellt haben.  Es sollte nicht in einer systemeigenen App verwendet werden, da Anwendungsgeheimnisse nicht zuverlässig auf Geräten gespeichert werden können.  Es ist für Web-Apps und Web-APIs erforderlich, die die Möglichkeit haben, das Anwendungsgeheimnis sicher auf dem Server zu speichern. |

### <a name="response"></a>Antwort
Eine erfolgreiche Tokenantwort sieht ähnlich wie folgende aus.

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "token_type": "Bearer",
    "expires_in": 3599,
    "scope": "user.read%20mail.read",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4...",
}
```
| Parameter | Beschreibung |
| --- | --- |
| access_token |Das angeforderte Zugriffstoken. Dieses Token kann die App in Aufrufen verwenden, die an Microsoft Graph gesendet werden. |
| token_type |Gibt den Tokentypwert an. Der einzige von Azure AD unterstützte Typ ist „Bearer“. |
| expires_in |Gültigkeit des Zugriffstokens (in Sekunden). |
| scope |Die Berechtigungen (Bereiche), für die das Zugriffstoken gültig ist. |
| refresh_token |Ein neues OAuth 2.0-Aktualisierungstoken. Ersetzen Sie das alte Aktualisierungstoken durch dieses neu abgerufene Aktualisierungstoken, um sicherzustellen, dass Ihre Aktualisierungstoken möglichst lange gültig bleiben. |

## <a name="supported-app-scenarios-and-additional-resources"></a>Unterstützte App-Szenarios und weitere Ressourcen
Sie können Microsoft Graph aus den folgenden Arten von Apps im Namen eines Benutzers aufrufen: 

- Systemeigene/mobile Apps 
- Web-Apps
- Einzelseiten-App (Single Page App, SPA)
- Back-End-Web-APIs: Beispielsweise in Szenarios, in denen eine Client-App, wie eine systemeigene App, Funktionen in einem Web-API-Back-End implementiert. Beim Azure AD v2.0-Endpunkt müssen die Client-App und die Back-End-Web-API die gleiche Anwendungs-ID haben. 

Weitere Informationen zu für den Azure AD v2.0-Endpunkt unterstützten App-Typen finden Sie unter [App-Typen für den Azure Active Directory v2.0-Endpunkt](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-flows).

> **Hinweis**: Das Aufrufen von Microsoft Graph aus einer [eigenständigen Web-API](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#restrictions-on-app-types) wird derzeit vom Azure AD v2.0-Endpunkt nicht unterstützt. Für dieses Szenario müssen Sie den Azure AD-Endpunkt verwenden.

Hier finden Sie weitere Informationen zum Zugreifen auf Microsoft Graph im Namen eines Benutzers über den Azure AD-v2.0-Endpunkt:

- Links zu Protokolldokumentation und Erste-Schritte-Artikeln für verschiedene Arten von Apps stehen in der [Dokumentation zum Azure AD v.20-Endpunkt ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview) zur Verfügung. 
- Ausführliche Beschreibungen der Authentifizierungsflüsse enthalten die Artikel zu [2.0-Protokollen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).
- Weitere Informationen zu empfohlenen Authentifizierungsbibliotheken und Servermiddleware von Microsoft und Drittanbietern für Azure AD v2.0 finden Sie unter [Azure Active Directory v2.0-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).

## <a name="azure-ad-endpoint-considerations"></a>Überlegungen zum Azure AD-Endpunkt
Es gibt einige Unterschiede zwischen der Verwendung des Azure AD-Endpunkts und des Azure AD v2.0-Endpunkts. Beispiel:

- Sie verwenden das [Azure-Portal](https://portal.azure.com) zum Konfigurieren Ihrer App. Weitere Informationen zum Konfigurieren von Apps mit dem Azure-Portal finden Sie unter [Integrieren von Anwendungen in Azure Active Directory: Hinzufügen einer Anwendung](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application).
- Ihre App erfordert für jede Plattform eine andere Anwendungs-ID (Client-ID).
- Wenn Ihre App mehrinstanzenfähig ist, müssen Sie sie im [Azure-Portal](https://portal.azure.com) explizit als mehrinstanzenfähig konfigurieren.
- Beim Azure AD-Endpunkt müssen alle Berechtigungen, die Ihre App benötigt, vom Entwickler konfiguriert werden. Der Azure AD-Endpunkt unterstützt keine dynamische (inkrementelle) Zustimmung.
- Der Azure AD-Endpunkt verwendet einen `resource`-Parameter in Autorisierungs- und Tokenanforderungen zur Angabe der Ressource, z. B. Microsoft Graph, für die Berechtigungen benötigt werden. Der Parameter `scope` wird vom Endpunkt nicht unterstützt. 
- Der Azure AD-Endpunkt macht keinen bestimmten Endpunkt für die Administratorzustimmung verfügbar. Stattdessen verwenden Apps den Parameter `prompt=admin_consent` in der Autorisierungsanforderung, um die Zustimmung des Administrators für eine Organisation zu erhalten. Weitere Informationen finden Sie unter **Auslösen von Azure AD-Consent Framework zur Laufzeit** im Artikel [Integrieren von Anwendungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).

Hier finden Sie weitere Informationen zum Zugreifen auf Microsoft Graph im Namen eines Benutzers über den Azure AD-Endpunkt:

- Informationen über die Verwendung des Azure AD-Endpunkts mit verschiedenen Arten von Apps können Sie über die Links im Abschnitt **Erste Schritte** des Leitfadens [Azure Active Directory für Entwickler](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide) aufrufen. Der Leitfaden enthält Links zu Übersichtsthemen, schrittweise Codeerläuterungen und Protokolldokumentation für verschiedene Arten von Apps, die vom Azure AD-Endpunkt unterstützt werden.
- Informationen zur Active Directory Authentication Library (ADAL) und Servermiddleware für die Verwendung mit dem Azure AD-Endpunkt finden Sie unter [Azure Active Directory-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).


 