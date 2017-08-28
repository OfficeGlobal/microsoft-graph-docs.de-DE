# <a name="get-started-with-microsoft-graph-and-rest"></a><span data-ttu-id="6c7d0-101">Erste Schritte mit Microsoft Graph und REST</span><span class="sxs-lookup"><span data-stu-id="6c7d0-101">Get started with Microsoft Graph and REST</span></span>

<span data-ttu-id="6c7d0-p101">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom Azure AD v2.0-Endpunkt und zum Aufrufen von Microsoft Graph mithilfe von REST-Aufrufen. Er beschreibt die Abfolge der Anforderungen und Antworten, die eine App zum Authentifizieren und Abrufen von E-Mail-Nachrichten verwendet.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph using REST calls. It describes the sequence of requests and responses that an app uses to authenticate and retrieve email messages.</span></span>

<span data-ttu-id="6c7d0-104">Zuerst müssen Sie Ihre App beim Azure Active Directory (Azure AD) registrieren.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-104">First, you need register your app with Azure Active Directory (Azure AD).</span></span> 

## <a name="register-the-application"></a><span data-ttu-id="6c7d0-105">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="6c7d0-105">Register the application</span></span>

<span data-ttu-id="6c7d0-106">Es gibt derzeit zwei Optionen für die Registrierung einer App bei Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-106">There are currently two options to register your app with Azure AD.</span></span>

  - <span data-ttu-id="6c7d0-107">Registrieren Sie eine App für die Verwendung des Azure AD v2.0-Endpunkts, der sowohl für persönliche (Microsoft) Identitäten als auch für Geschäfts- und Schulkonten (Azure AD) geeignet ist.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-107">Register an app to use the Azure AD v2.0 endpoint that works for both personal (Microsoft) identities and work and school (Azure AD) accounts.</span></span>
  - <span data-ttu-id="6c7d0-108">Registrieren Sie eine App für die Verwendung des Azure AD-Endpunkts, der nur Geschäfts- und Schulkonten unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-108">Register an app to use the Azure AD endpoint that supports work and school accounts only.</span></span>

<span data-ttu-id="6c7d0-p102">In diesem Artikel wird eine v2.0-Registrierung vorausgesetzt, weshalb Sie Ihre App im [App-Registrierungsportal](https://apps.dev.microsoft.com/) registrieren. Folgen Sie den Anweisungen in [Registrieren Ihrer Microsoft Graph-Anwendung mit dem Azure AD-Version 2.0-Endpunkt](../concepts/auth_register_app_v2.md), um Ihre App zu registrieren. Informationen zur Verwendung des Endpunkts Azure AD finden Sie unter [Authentifizieren mit Azure AD](../concepts/auth_v2_user.md).</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p102">This article assumes a v2.0 registration, so you'll register your app on the [Application Registration Portal](https://apps.dev.microsoft.com/). Follow the instructions in [Register your Microsoft Graph application with the Azure AD v2.0 endpoint](../concepts/auth_register_app_v2.md) to register your app. For information about using the Azure AD endpoint, see [Authenticate using Azure AD](../concepts/auth_v2_user.md).</span></span>

> <span data-ttu-id="6c7d0-p103">Einige Einschränkungen sind zu beachten, wenn Sie den Endpunkt Version 2.0 verwenden. Damit Sie die für Sie richtige Entscheidung treffen können, informieren Sie sich unter [Sollte ich den v2.0-Endpunkt verwenden?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p103">Some limitations apply when using the v2.0 endpoint. To decide if it's right for you, see [Should I use the v2.0 endpoint?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span></span>

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="6c7d0-114">Authentifizierung des Benutzers und Abrufen eines Zugriffstokens</span><span class="sxs-lookup"><span data-stu-id="6c7d0-114">Authenticate the user and get an access token</span></span>

<span data-ttu-id="6c7d0-p104">Die in diesem Artikel beschriebene App implementiert den [Authorization Code Grant-Datenfluss](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) zum Abrufen der Zugriffstoken von dem Azure AD v2.0-Endpunkt gemäß standardmäßiger[ OAuth 2.0-Protokolle](http://tools.ietf.org/html/rfc6749). Eine vollständige Anleitung zu den im Azure AD v2.0-Endpunkt unterstützten Datenflüssen finden Sie unter [v2.0-Endpunkt-Typen](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p104">The app described in this article implements the [Authorization Code Grant flow](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) to get access tokens from the Azure AD v2.0 endpoint, following standard [OAuth 2.0 protocols](http://tools.ietf.org/html/rfc6749). For a complete guide to the flows supported in the Azure AD v2.0 endpoint see [Types of the v2.0 endpoint](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span></span>

<span data-ttu-id="6c7d0-117">Mit dem Authorization Code Grant-Datenfluss rufen Sie zuerst einen Autorisierungscode ab und tauschen diesen Code dann gegen ein Zugangstoken aus.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-117">With the Authorization Code Grant flow, first you get an authorization code and then you exchange the code for an access token.</span></span>

### <a name="getting-an-authorization-code"></a><span data-ttu-id="6c7d0-118">Abrufen eines Autorisierungscodes</span><span class="sxs-lookup"><span data-stu-id="6c7d0-118">Getting an authorization code</span></span>

<span data-ttu-id="6c7d0-p105">Im ersten Schritt des Authorization Code Grant-Datenflusses wird der Autorisierungscode abgerufen. Der Code wird vom Autorisierungsserver an die App übergeben, wenn der Benutzer sich anmeldet und den von der App angeforderten Berechtigungen zustimmt.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p105">The first step in the Authorization Code Grant flow is to get an authorization code. The code is returned to the app by the authorization server when the user signs in and consents to the permissions requested by the app.</span></span>

<span data-ttu-id="6c7d0-p106">Sie fordern einen Autorisierungscode an, indem Sie eine GET-Anforderung an den Azure AD v2.0-Endpunkt senden. Diese URL muss in einem Browser geöffnet werden, damit der Benutzer sich anmelden und seine Zustimmung erteilen kann.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p106">You request an authorization code by sending a GET request to the Azure AD v2.0 endpoint. This URL must be opened in a browser so that the user can sign in and provide consent.</span></span>

#### <a name="construct-the-request"></a><span data-ttu-id="6c7d0-123">Erstellen der Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c7d0-123">Construct the request</span></span>

<span data-ttu-id="6c7d0-124">1 – Beginnen Sie mit der Basis-URL:</span><span class="sxs-lookup"><span data-stu-id="6c7d0-124">1- Start with the base URL:</span></span>

```
https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
```

<span data-ttu-id="6c7d0-p107">Das *Mandanten*-Segment im Pfad bestimmt, wer sich bei der Anwendung anmelden kann. Zulässige Werte sind *Allgemein*, *Organisationen*, *Consumer* und Mandantenbezeichner. Weitere Informationen finden Sie unter [Protokoll-Endpunkte](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p107">The *tenant* segment in the path controls who can sign into the application. Allowed values are *common*, *organizations*, *consumers*, and tenant identifiers. For more information, see [Protocol endpoints](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span></span>

<span data-ttu-id="6c7d0-p108">2 – Hängen Sie Abfrageparameter auf der Basis-URL an. Diese werden verwendet, um die App, die erforderlichen Berechtigungen und andere Informationen zur Anforderung der Authentifizierung zu identifizieren. In der folgenden Tabelle werden einige allgemeine Parameter beschrieben:</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p108">2- Append query parameters to the base URL. These are used to identify the app, the requested permissions, and other auth request information. The following table describes some common parameters.</span></span>

| <span data-ttu-id="6c7d0-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="6c7d0-131">Parameter</span></span> | <span data-ttu-id="6c7d0-132">Beschreibungen</span><span class="sxs-lookup"><span data-stu-id="6c7d0-132">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="6c7d0-133">client_id</span><span class="sxs-lookup"><span data-stu-id="6c7d0-133">client_id</span></span> | <span data-ttu-id="6c7d0-p109">Die beim Registrieren der App generierte Client-ID. Anhand dieser erkennt Azure AD, welche App die Anmeldung anfordert.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p109">The app ID generated by registering the app. This lets Azure AD know which app is requesting the logon.</span></span> |
| <span data-ttu-id="6c7d0-136">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="6c7d0-136">redirect_uri</span></span> | <span data-ttu-id="6c7d0-p110">Der Speicherort, zu dem Azure umleitet, nachdem der Benutzer seine Zustimmung für diese App erteilt hat. Dieser Wert muss mit dem Wert des beim Registrieren der App verwendeten **Umleitungs-URI** übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p110">The location that Azure will redirect to after the user has granted consent to the app. This value must correspond to the value of **Redirect URI** used when registering the app.</span></span> |
| <span data-ttu-id="6c7d0-139">response_type</span><span class="sxs-lookup"><span data-stu-id="6c7d0-139">response_type</span></span> | <span data-ttu-id="6c7d0-p111">Der Antworttyp, den die App erwartet. Dieser Wert ist `code` für den Authorization Code Grant-Datenfluss.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p111">The type of response the app is expecting. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="6c7d0-142">scope</span><span class="sxs-lookup"><span data-stu-id="6c7d0-142">scope</span></span> | <span data-ttu-id="6c7d0-p112">Eine durch Leerzeichen getrennte Liste von [Microsoft Graph Berechtigungsbereichen](./permissions_reference.md), die die App anfordert. Sie können auch [OpenId Connect-Bereiche](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) für [die einmalige Anmeldung](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/) angeben.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p112">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting. You can also specify [OpenId Connect scopes](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) for [single sign-on](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).</span></span>  |
| <span data-ttu-id="6c7d0-145">state</span><span class="sxs-lookup"><span data-stu-id="6c7d0-145">state</span></span> | <span data-ttu-id="6c7d0-146">Ein Wert, der in der Anforderung enthalten ist, die in der Tokenantwort für die Validierung zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-146">A value included in the request that will also be returned in the token response, used for validation.</span></span> |

<span data-ttu-id="6c7d0-147">Die Anforderungs-URL für eine Anwendung, die den Lesezugriff auf E-Mails anfordert, könnte beispielsweise wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-147">For example, the request URL for an application that requires read access to mail might look like the following.</span></span>

```
GET https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=<app ID>&redirect_uri=http%3A%2F%2Flocalhost/myapp%2F&response_type=code&state=1234&scope=mail.read
```

<span data-ttu-id="6c7d0-p113">3 – Leiten Sie dann den Benutzer zu der Anmelde-URL weiter. Es wird ein Anmeldefenster mit dem Namen der App angezeigt. Nach dem Anmelden wird eine Liste der Berechtigungen angezeigt, die die App anfordert, und der Benutzer wird aufgefordert, diesen zuzustimmen oder sie zu verweigern. Wenn der Benutzer zustimmt, veranlasst der Browser die Umleitung zu dem Umleitungs-URI mit dem Autorisierungscode und dem Status in der Abfragezeichenfolge, wie im folgenden Beispiel gezeigt.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p113">3- Redirect the user to the logon URL. The user is presented with a sign in screen that displays the name of the app. After signing in, the user is presented with the list of the permissions the app requires and prompted to allow or deny. If the user consents, the browser redirects to the redirect URI with the authorization code and state in the query string, as shown in the following example.</span></span>

```
http://localhost/myapp/?code=AwABAAAA...cZZ6IgAA&state=1234
```

<span data-ttu-id="6c7d0-152">Im nächsten Schritt wird der für ein Zugriffstoken zurückgegebene Autorisierungscode ausgetauscht.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-152">The next step is to exchange the authorization code returned for an access token.</span></span>

### <a name="getting-an-access-token"></a><span data-ttu-id="6c7d0-153">Abrufen eines Zugriffstokens</span><span class="sxs-lookup"><span data-stu-id="6c7d0-153">Getting an access token</span></span>

<span data-ttu-id="6c7d0-154">Zum Abrufen eines Zugriffstokens stellt die App fomularcodierte Parameter für die Tokenanforderungs-URL (beispielsweise `https://login.microsoftonline.com/common/oauth2/v2.0/token`) mit den folgenden Parametern bereit.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-154">To get an access token, the app posts form-encoded parameters to the token request URL (for example, `https://login.microsoftonline.com/common/oauth2/v2.0/token`) with the following parameters.</span></span>

| <span data-ttu-id="6c7d0-155">Parameter</span><span class="sxs-lookup"><span data-stu-id="6c7d0-155">Parameter</span></span> | <span data-ttu-id="6c7d0-156">Beschreibungen</span><span class="sxs-lookup"><span data-stu-id="6c7d0-156">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="6c7d0-157">client_id</span><span class="sxs-lookup"><span data-stu-id="6c7d0-157">client_id</span></span> | <span data-ttu-id="6c7d0-158">Die beim Registrieren der App generierte Client-ID.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-158">The app ID generated by registering the app.</span></span> |
| <span data-ttu-id="6c7d0-159">client_secret</span><span class="sxs-lookup"><span data-stu-id="6c7d0-159">client_secret</span></span> | <span data-ttu-id="6c7d0-160">Der beim Registrieren der App generierte geheime Anwendungsschlüssel.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-160">The app secret generated when registering the app.</span></span> |
| <span data-ttu-id="6c7d0-161">code</span><span class="sxs-lookup"><span data-stu-id="6c7d0-161">code</span></span> | <span data-ttu-id="6c7d0-162">Der im vorherigen Schritt abgerufene Autorisierungscode.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-162">The authorization code obtained in the prior step.</span></span> |
| <span data-ttu-id="6c7d0-163">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="6c7d0-163">redirect_uri</span></span> | <span data-ttu-id="6c7d0-164">Dieser Wert muss mit dem in der Autorisierungscodeanforderung verwendeten Wert übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-164">This value must be the same as the value used in the authorization code request.</span></span> |
| <span data-ttu-id="6c7d0-165">grant_type</span><span class="sxs-lookup"><span data-stu-id="6c7d0-165">grant_type</span></span> | <span data-ttu-id="6c7d0-p114">Der von der App verwendete Typ des Zugriffs. Dieser Wert ist `code` für den Authorization Code Grant-Datenfluss.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p114">The type of grant the app is using. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="6c7d0-168">Bereich</span><span class="sxs-lookup"><span data-stu-id="6c7d0-168">scope</span></span> | <span data-ttu-id="6c7d0-169">Eine durch Leerzeichen getrennte Liste von [Microsoft Graph Berechtigungsbereichen](./permissions_reference.md), die die App anfordert.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-169">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting.</span></span> |

<span data-ttu-id="6c7d0-170">Die Anforderungs-URL für unsere Anwendung sieht unter Verwendung des Codes aus dem vorherigen Schritt wie folgt aus.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-170">The request URL for our application, using the code from the previous step, looks like the following.</span></span>

```
POST https://login.microsoftonline.com/common/oauth2/v2.0/token
Content-Type: application/x-www-form-urlencoded

{
  grant_type=authorization_code
  &code=AwABAAAA...cZZ6IgAA
  &redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
  &resource=https%3A%2F%2Fgraph.microsoft.com%2F
  &scope=mail.read
  &client\_id=<app ID>
  &client\_secret=<app SECRET>
}
```

<span data-ttu-id="6c7d0-171">Der Server antwortet mit einer JSON-Nutzlast, die das Zugriffstoken enthält.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-171">The server responds with a JSON payload which includes the access token.</span></span>

```
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "token_type":"Bearer",
  "expires_in":"3600",
  "access_token":"eyJ0eXAi...b66LoPVA",
  "scope":"https://graph.microsoft.com/mail.read",
  ...
}
```

<span data-ttu-id="6c7d0-p115">Das Zugriffstoken befindet sich im Feld `access_token` der JSON-Nutzlast. Die App verwendet diesen Wert zum Festlegen des Autorisierungsheaders bei REST-Aufrufen für die API.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p115">The access token is found in the `access_token` field of the JSON payload. The app uses this value to set the Authorization header when making REST calls to the API.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="6c7d0-174">Aufrufen von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6c7d0-174">Call Microsoft Graph</span></span>

<span data-ttu-id="6c7d0-p116">Wenn die App über ein Zugriffstoken verfügt, kann Microsoft Graph aufgerufen werden. Da diese Beispiel-App Nachrichten abruft, verwendet sie eine HTTP-GET-Anforderung für den `https://graph.microsoft.com/v1.0/me/messages`-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p116">After the app has an access token, it's ready to call Microsoft Graph. Because this sample app is retrieving messages, it will use an HTTP GET request to the `https://graph.microsoft.com/v1.0/me/messages` endpoint.</span></span>

### <a name="refine-the-request"></a><span data-ttu-id="6c7d0-177">Beschränken der Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c7d0-177">Refine the request</span></span>

<span data-ttu-id="6c7d0-p117">Apps können das Verhalten der GET-Anforderungen mithilfe von OData-Abfrageparametern steuern. Diese Parameter sollten von den Apps verwendet werden, um die Anzahl der zurückgegebenen Ergebnisse und der für jedes Element zurückgegebenen Felder einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p117">Apps can control the behavior of GET requests by using OData query parameters. We recommend that apps use these parameters to limit the number of results that are returned and to limit the fields that are returned for each item.</span></span> 

<span data-ttu-id="6c7d0-p118">In dieser Beispiel-App werden die Nachrichten in einer Tabelle angezeigt, in der Betreff, Absender und der Zeitpunkt enthalten sind, zu dem die Nachricht empfangen wurde. In der Tabelle werden maximal 25 Zeilen angezeigt, wobei diese so sortiert sind, dass zuletzt empfangene Nachrichten oben aufgeführt sind. Die App verwendet die folgenden Abfrageparameter, um diese Ergebnisse zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p118">This sample app will display messages in a table that shows the subject, sender, and the date and time the message was received. The table displays a maximum of 25 rows and is sorted so that the most recently received message is at the top. The app uses the following query parameters to get these results.</span></span>

- <span data-ttu-id="6c7d0-183">`$select` - Gibt nur die Felder `subject`, `sender` und `dateTimeReceived` an.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-183">`$select` - Specifies only the `subject`, `sender`, and `dateTimeReceived` fields.</span></span>
- <span data-ttu-id="6c7d0-184">`$top` - Gibt maximal 25 Elemente an.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-184">`$top` - Specifies a maximum of 25 items.</span></span>
- <span data-ttu-id="6c7d0-185">`$orderby` - Sortiert die Ergebnisse nach dem `dateTimeReceived`-Feld.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-185">`$orderby` - Sorts the results by the `dateTimeReceived` field.</span></span>

<span data-ttu-id="6c7d0-186">Als Ergebnis erhält man die folgende Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-186">This results in the following request.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

<span data-ttu-id="6c7d0-p119">Da Sie nun gelernt haben, wie Aufrufe für Microsoft Graph getätigt werden, können Sie anhand der API-Referenz beliebige Arten von Aufrufen erstellen, die für Ihre App erforderlich sind. Denken Sie daran, dass entsprechende Berechtigungen für die App bei der App-Registrierung für die Aufrufe konfiguriert sein müssen.</span><span class="sxs-lookup"><span data-stu-id="6c7d0-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6c7d0-189">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="6c7d0-189">Next steps</span></span>
- <span data-ttu-id="6c7d0-190">Testen Sie die Möglichkeiten der REST-API mithilfe des [Graph-Explorers](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6c7d0-190">Try out more of the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="6c7d0-191">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6c7d0-191">See also</span></span>
- [<span data-ttu-id="6c7d0-192">Azure AD v2.0-Protokolle</span><span class="sxs-lookup"><span data-stu-id="6c7d0-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="6c7d0-193">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="6c7d0-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
