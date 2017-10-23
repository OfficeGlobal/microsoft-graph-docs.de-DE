# <a name="get-access-tokens-to-call-microsoft-graph"></a>Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph

Zum Aufrufen von Microsoft Graph muss Ihre App ein Zugriffstoken von Azure Active Directory (Azure AD) abrufen, dem Cloudidentitätsdienst von Microsoft. Das Zugriffstoken enthält Informationen (bzw. Ansprüche) zu Ihrer App und die Berechtigungen, über die es für die Ressourcen und APIs verfügt, die über Microsoft Graph bereitgestellt werden. Um ein Zugriffstoken abzurufen, muss Ihre App sich bei Azure AD authentifizieren können und entweder durch einen Benutzer oder einen Administrator zum Zugreifen auf die benötigten Microsoft Graph-Ressourcen autorisiert werden. 

Dieses Thema enthält eine Übersicht über Zugriffstoken, Azure AD und das Verfahren zum Abrufen von Zugriffstoken durch Ihre App. Wenn Sie mit der Verfahren zum Integrieren einer App in Azure AD zum Abrufen von Token vertraut sind, können Sie direkt mit dem Abschnitt [Nächste Schritte](#next-steps) fortfahren, der Informationen und Beispiele speziell zu Microsoft Graph enthält. 

> **Wichtig:**  Die Anwendung der Richtlinien für bedingten Zugriff für Microsoft Graph wurde geändert. Anwendungen müssen aktualisiert werden, um Szenarien ausführen zu können, für die bedingte Richtlinien konfiguriert sind. Weitere Informationen und Anleitungen hierzu finden Sie unter [Developer-Leitfaden zum bedingten Zugriff in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).

## <a name="what-is-an-access-token-and-how-do-i-use-it"></a>Was sind Zugriffstoken und wie werden sie verwendet?

Von Azure AD ausgestellte Zugriffstoken sind base64-codierte JSON Web Token (JWT). Sie enthalten Informationen (Ansprüche), die von Azure AD gesicherte Web-APIs wie Microsoft Graph verwenden, um die aufrufende Funktion zu überprüfen und sicherzustellen, dass diese über die richtigen Berechtigungen zum Ausführen des angeforderten Vorgangs verfügt. Beim Aufrufen von Microsoft Graph können Sie Zugriffstoken als undurchsichtig (opak) behandeln. Zugriffstoken sollten immer über einen sicheren Kanal wie z. B. Transport Layer Security (HTTPS) übertragen werden.

Hier sehen Sie ein Beispiel für ein Azure AD-Zugriffstoken:

`EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/oeJX6U8nnL9nJ5pHLVuPWD0aNnTPTJD8Y4oQTp5zLhDIIfaJCaGcQperULVF7K6yX8MhHxIBwek418rKIp11om0SWBXOYSGOM0rNNN59qNiKwLNK+MPUf7ObcRBN5I5vg8jB7IMoz66jrNmT2uiWCyI8MmYDZgAACPoaZ9REyqke+AE1/x1ZX0w7OamUexKF8YGZiw+cDpT/BP1GsONnwI4a8M7HsBtDgZPRd6/Hfqlq3HE2xLuhYX8bAc1MUr0gP9KuH6HDQNlIV4KaRZWxyRo1wmKHOF5G5wTHrtxg8tnXylMc1PKOtaXIU4JJZ1l4x/7FwhPmg9M86PBPWr5zwUj2CVXC7wWlL/6M89Mlh8yXESMO3AIuAmEMKjqauPrgi9hAdI2oqnLZWCRL9gcHBida1y0DTXQhcwMv1ORrk65VFHtVgYAegrxu3NDoJiDyVaPZxDwTYRGjPII3va8GALAMVy5xou2ikzRvJjW7Gm3XoaqJCTCExN4m5i/Dqc81Gr4uT7OaeypYTUjnwCh7aMhsOTDJehefzjXhlkn//2eik+NivKx/BTJBEdT6MR97Wh/ns/VcK7QTmbjwbU2cwLngT7Ylq+uzhx54R9JMaSLhnw+/nIrcVkG77Hi3neShKeZmnl5DC9PuwIbtNvVge3Q+V0ws2zsL3z7ndz4tTMYFdvR/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==`

Zum Aufrufen von Microsoft Graph fügen Sie das Zugriffstoken als Bearer-Token an den Autorisierungsheader einer HTTP-Anforderung an. Hier sehen Sie z. B. einen Aufruf, der die Profilinformationen des angemeldeten Benutzers zurückgibt (das Zugriffstoken wurde zur besseren Lesbarkeit abgeschnitten):

```
HTTP/1.1
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
Host: graph.microsoft.com`
GET https://graph.microsoft.com/v1.0/me/
```

## <a name="what-are-microsoft-graph-permissions"></a>Was sind Microsoft Graph-Berechtigungen?
Microsoft Graph stellt einen umfangreichen Satz von differenzierten Berechtigungen für die von der API gesteuerten Ressourcen zur Verfügung. Diese Berechtigungen werden als Zeichenfolgen ausgedrückt und gewähren Apps Zugriff auf Microsoft Graph-Ressourcen wie Benutzern, Gruppen, Benutzer-E-Mails usw. Beispiel:

- _User.Read_ ermöglicht einer App, das Profil des angemeldeten Benutzers zu lesen.
- _Mail.Send_ ermöglicht einer App, E-Mails im Namen des angemeldeten Benutzers zu senden.

Es gibt zwei Arten von Berechtigungen:

- Delegierte Berechtigungen werden von Apps verwendet, bei deren Ausführung ein Benutzer angemeldet ist. Die Rechte des Benutzers werden an die App delegiert, die Aufrufe im Namen des Benutzers an Microsoft Graph sendet. Viele dieser Berechtigungen können von einem Benutzer genehmigt werden, aber andere erfordern die Zustimmung eines Administrators.  
- Anwendungsberechtigungen werden von Apps verwendet, die ohne Benutzer ausgeführt werden. Diese Berechtigungen gewähren einer App häufig umfassende Rechte innerhalb einer Organisation und erfordern immer die Zustimmung eines Administrators.

Eine vollständige Liste der Microsoft Graph-Berechtigungen sowie die Unterschiede zwischen delegierten und Anwendungsberechtigungen finden Sie in der [Berechtigungsreferenz](permissions_reference.md).

## <a name="where-does-my-app-get-an-access-token"></a>Wo erhält meine App ein Zugriffstoken?
Ihre App ruft Zugriffstoken von Azure Active Directory (Azure AD) ab, dem Cloudidentitätsdienst von Microsoft. Um ein Zugriffstoken abzurufen, tauscht Ihre App HTTP-Anforderungen und -Antworten mit Azure AD aus; hierzu werden Industriestandardprotokolle verwendet, die in den Spezifikationen OAuth 2.0 und OpenID Connect 1.0 definiert sind. Diese Protokolle beschreiben die Azure AD-Endpunkte und den Austausch mit diesen, d. h. die Authentifizierungsflüsse, die Ihre App verwendet, um sich sicher bei Azure AD zu authentifizieren und Zugriffstoken abzurufen.  

Ganz einfach ausgedrückt, tauscht Ihre App zum Abrufen eines Zugriffstokens HTTP-Anforderungen mit den folgenden Endpunkten aus:

- Dem `/authorize`-Endpunkt; hierhin kann Ihre App einen Benutzer senden, damit dieser sich bei Azure AD authentifiziert und den von der App benötigten Berechtigungen zustimmt.
- Dem `/token`-Endpunkt; von diesem kann Ihre App ein Zugriffstoken abrufen, nachdem der Benutzer seine Zustimmung erteilt hat.

(Hinweis: Diese Definitionen sind nicht starr. Abhängig von dem von der App verwendeten Protokoll können Zugriffstoken ggf. direkt vom `/authorize`-Endpunkt abgerufen werden, oder die App kann sich direkt beim `/token`-Endpunkt authentifizieren.) 

Hier sehen Sie ein Beispiel für einen Satz der von Azure AD v2.0 verfügbar gemachten `/authorize`- und `/token`-Endpunkt:

```
https://login.microsoftonline.com/common/oauth2/v2.0/authorize
https://login.microsoftonline.com/common/oauth2/v2.0/token

```
Azure AD stellt zwei Sätze von Endpunkten zur Verfügung: Azure AD und Azure AD v2.0. Der Hauptunterschied zwischen ihnen besteht darin, dass der Azure AD-Endpunkt nur Geschäfts-, Schul- oder Unikonten unterstützt (d. h. Konten, die einem Azure AD-Mandanten zugeordnet sind), während Azure AD v2.0 auch Microsoft-Konten wie _live.com_- oder _outlook.com_-Konten unterstützt. Dies bedeutet Folgendes: Wenn Sie den Azure AD-Endpunkt verwenden, können Sie Ihre App nur für Organisationen entwickeln, mit Azure AD v2.0 jedoch für Heimanwender und Organisationen. 

Token vom Azure AD-Endpunkt und solche vom Azure AD v2.0-Endpunkt sind nicht austauschbar; daher müssen Sie sich für einen Endpunkt entscheiden, bevor Sie mit der Arbeit an einer App für die Produktion beginnen. Da der Azure AD v2.0-Endpunkt neuer ist und immer noch neue Features hinzugefügt werden, gibt es einige wichtigen Einschränkungen, die Sie bei der Entscheidung über den Endpunkt für Ihre App in der Produktion berücksichtigen müssen. Weitere Informationen finden Sie unter [Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt](#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

## <a name="whats-the-difference-between-oauth-20-and-openid-connect"></a>Worin besteht der Unterschied zwischen OAuth 2.0 und OpenID Connect?

Bei OAuth 2.0 handelt es sich um ein Autorisierungsprotokoll. Es definiert, wie Ihre App Zugriffstoken abrufen kann, indem sie sich direkt bei Azure AD authentifiziert oder einen Benutzer umleitet, damit er sich bei Azure AD authentifiziert und den von Ihrer App angeforderten Berechtigungen zustimmt. Im ersten Fall erhält Ihre App ein Zugriffstoken, mit dem sie Microsoft Graph im eigenen Namen aufrufen kann. Im zweiten Fall erhält Ihre App ein Zugriffstoken, mit dem sie Microsoft Graph im Namen eines Benutzers aufrufen kann. Bei Verwendung von OAuth 2.0 erhält Ihre App jedoch keine Informationen über den Benutzer oder wie er von Azure AD authentifiziert wird. OAuth 2.0-Flüsse werden am häufigsten von mobilen oder systemeigenen Apps verwendet, die die Identität des Benutzers bereits kennen, oder von Apps wie Hintergrunddiensten oder Daemons, die Microsoft Graph unter ihrer eigenen Identität und nicht im Namen eines Benutzers aufrufen.

OpenID Connect erweitert OAuth 2.0 und stellt eine Identitätsebene bereit. Bei Verwendung von OpenID Connect kann Ihre App zusätzlich zu einem Zugriffstoken auch ein ID-Token von Azure AD abrufen. ID-Token von OpenID Connect enthalten Ansprüche zur Identität des Benutzers und Details darüber, wie und wo sie authentifiziert wurden. OpenID Connect-Flüsse werden in der Regel von Web-Apps verwendet, z. B. auch von Einzelseiten-Apps (SPAs). Diese Apps können mithilfe des ID-Tokens ihr Verhalten für den jeweiligen Benutzer anpassen, für den sie ein Zugriffstoken angefordert haben; in vielen Fällen lagern sie außerdem die Anmeldung der Benutzer an Azure AD aus und aktivieren Funktionen wie einmaliges Anmelden (Single Sign-On, SSO).

## <a name="what-kind-of-apps-can-i-call-microsoft-graph-from"></a>Aus welcher Art von Apps kann ich Microsoft Graph aufrufen?
Sie können Microsoft Graph aus den folgenden Arten von Apps aufrufen: 

- **Systemeigene Apps**: Apps, die auf einem Gerät wie z. B. einem Desktop, Tablet-PC oder Mobiltelefon ausgeführt werden. Diese Apps verwenden das systemeigene Betriebssystem des Geräts wie iOS, Android oder Windows für die Benutzerdarstellung und zum Senden von Aufrufen an Microsoft Graph im Namen eines Benutzers.
- **Web-Apps**: Apps, die auf einem Server ausgeführt werden und über einen Benutzer-Agenten, normalerweise einen Webbrowser, mit dem angemeldeten Benutzer interagieren. Der Großteil der Darstellungsschicht wird auf dem Server verarbeitet, und Aufrufe von Microsoft Graph erfolgen serverseitig im Namen eines Benutzers.
- **Einzelseiten-App (Single Page App, SPA)**: Web-Apps mit umfassender Benutzeroberfläche, die einen großen Teil der Darstellungsschicht über clientseitige Skripts im Browser verarbeiten. Aufrufe von Microsoft Graph erfolgen im clientseitigen Skript mit Technologien wie AJAX und Frameworks wie Angular.js. Aufrufe erfolgen im Namen eines Benutzers.
- **Hintergrunddienste/Daemons**: Hintergrunddienste und Daemons, die ohne einen angemeldeten Benutzer auf einem Server ausgeführt werden und Aufrufe unter ihrer eigenen Identität an Microsoft Graph senden.
- **Web-APIs**: Eine Client-App ruft eine Web-API (von Azure AD gesichert) auf, die daraufhin Microsoft Graph aufruft, alles im Namen eines Benutzers. Wird vom Azure AD-Endpunkt unterstützt. Wird für den Azure AD v2.0-Endpunkt nur unterstützt, wenn der Client und die Web-API die gleiche Anwendungs-ID haben; ein Beispiel ist eine systemeigene App, die ein Web-API-Back-End aufruft. 

## <a name="how-do-i-get-my-app-talking-to-azure-ad-and-microsoft-graph"></a>Wie bringe ich meine App dazu, mit Azure AD und Microsoft Graph zu kommunizieren?
Bevor Ihre App ein Token von Azure AD abrufen kann, muss sie registriert werden. Für den Azure AD v2.0-Endpunkt verwenden Sie das [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/), um Ihre App zu registrieren. Für den Azure AD-Endpunkt verwenden das [Azure-Portal](https://portal.azure.com/). Durch die Registrierung wird Ihre App in Azure AD integriert, und es werden die Koordinaten und Bezeichner eingerichtet, die die App zum Abrufen von Token verwendet. Dies sind:

- **Anwendungs-ID**. Ein eindeutiger Bezeichner, der von Azure AD zugewiesen wird. 
- **Umleitungs-URI/-URL**: Ein oder mehrere Endpunkte, an denen Ihre App Antworten von Azure AD empfängt. (Für systemeigene und mobile Apps ist dies ein von Azure AD zugewiesener URI.)
- **Anwendungsgeheimnis**: Ein Kennwort oder ein öffentliches/privates Schlüsselpaar, mit dem sich Ihre App bei Azure AD authentifiziert. (Für systemeigene oder mobile Apps nicht erforderlich.)

Für Apps, die den Azure AD-Endpunkt verwenden, konfigurieren Sie außerdem vorab während der Registrierung die Microsoft Graph-Berechtigungen, die Ihre App benötigt. Für Apps, die den Azure AD v2.0-Endpunkt verwenden, ist die Vorabkonfiguration von Berechtigungen ggf. nicht erforderlich. 

Die während der Registrierung konfigurierten Eigenschaften werden bei der Übertragung verwendet. In der folgenden Tokenanforderung beispielsweise ist *client_id* die *Anwendungs-ID*, *redirect_uri* ist einer der registrierten *Umleitungs-URIs* Ihrer App, und *client_secret* ist das *Anwendungsgeheimnis*. 

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

## <a name="are-there-authentication-libraries-available"></a>Sind Authentifizierungsbibliotheken verfügbar?
Wie die meisten Entwickler werden auch Sie wahrscheinlich Authentifizierungsbibliotheken zum Verwalten Ihrer Interaktionen mit Azure AD verwenden. Authentifizierungsbibliotheken nehmen dem Entwickler viele Protokolldetails wie Überprüfung, Cookiebehandlung, Zwischenspeicherung von Token und Aufrechterhaltung sicherer Verbindungen ab, sodass Sie sich auf die Entwicklung Ihrer App konzentrieren können. Microsoft veröffentlicht Open Source-Clientbibliotheken und Servermiddleware für den Azure AD- und den Azure AD v2.0-Endpunkt. 

Für den Azure AD v2.0-Endpunkt: 

- Microsoft Authentication Library (MSAL)-Clientbibliotheken sind für .NET, JavaScript, Android und Objective-c verfügbar. Alle Plattformen befinden sich in produktionsunterstützter Vorschau, und für den Fall der Einführung grundlegender Änderungen garantiert Microsoft einen Upgradepfad.
- Servermiddleware von Microsoft steht für .NET Core und ASP.NET (OWIN OpenID Connect und OAuth) sowie für Node.js (Microsoft Azure AD Passport.js) zur Verfügung. 
- Der v2.0-Endpunkt ist mit vielen Authentifizierungsbibliotheken von Drittanbietern kompatibel.

Eine vollständige Liste der Microsoft-Clientbibliotheken, Microsoft-Servermiddleware und kompatibler Bibliotheken von Drittanbietern finden Sie unter [Azure Active Directory v2.0-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).

Für den Azure AD-Endpunkt:

- Active Directory Authentication Library (ADAL)-Clientbibliotheken stehen auf einer etwas größeren Anzahl von Plattformen zur Verfügung. 
- Servermiddleware von Microsoft ist für .NET Core und ASP.NET sowie für Node.js verfügbar. 

Eine vollständige Liste der Microsoft-Clientbibliotheken und -Servermiddleware finden Sie unter [Azure Active Directory-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).

## <a name="deciding-between-the-azure-ad-and-azure-ad-v20-endpoints"></a>Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt

Azure AD stellt zwei Sätze von Endpunkten bereit, Azure AD und Azure AD v2.0, von denen Sie Zugriffstoken abrufen können, um Aufrufe an Microsoft Graph zu senden. Die Token der beiden Endpunkte sind nicht austauschbar. Zum Ausführen von Beispielen oder Erkunden der Funktionen von Microsoft Graph ist die Entscheidung für einen Azure AD-Endpunkt unerheblich. Bevor Sie jedoch mit der Entwicklung einer Produktions-App beginnen, müssen Sie sich entscheiden, welcher Endpunkt für Ihr Szenario am besten geeignet ist. Die folgende Diskussion enthält einige allgemeine Richtlinien, die Ihnen bei der Entscheidungsfindung helfen können; aktuelle und umfassende Informationen finden Sie jedoch unter [Sollte ich den v2.0-Endpunkt verwenden?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations) in der Dokumentation zu Azure Active Directory. 

Der Hauptunterschied zwischen Azure AD und Azure AD v2.0 besteht in Folgendem:

* Azure AD unterstützt nur Geschäfts-, Schul- oder Unikonten, d. h. Konten, die einem Azure AD-Mandanten zugeordnet sind. Dies bedeutet, dass Sie Ihre App nur für Organisationen entwickeln können.
* Azure AD v2.0 unterstützt sowohl Geschäfts-, Schul- oder Unikonten als auch Microsoft-Konten wie _live.com_- oder _outlook.com_-Konten. Dies bedeutet, dass Sie Ihre App mithilfe des v2.0-Endpunkts sowohl für Heimanwender als auch für Organisationen entwickeln können. 

Azure AD v2.0 bietet außerdem einige zusätzliche Vorteile. Beispiel:

* Ihre App kann eine einzige Anwendungs-ID für mehrere Plattformen verwenden. Dies vereinfacht die App-Verwaltung für Entwickler und Administratoren.
* [Unterstützung von dynamischer und inkrementeller Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare#incremental-and-dynamic-consent). Mit diesem Feature kann Ihre App zusätzliche Berechtigungen während der Laufzeit anfordern und dabei die Anforderung der Benutzerzustimmung mit den Funktionen koppeln, die die Berechtigungen benötigen. Dies ist wesentlich benutzerfreundlicher als das Szenario, in dem Benutzer einer langen Liste von Berechtigungen zustimmen müssen, wenn sie sich zum ersten Mal anmelden.  

Da Azure AD v2.0 neuer als Azure AD ist und immer noch neue Features hinzugefügt werden, gibt es einige Einschränkungen beim v2.0-Endpunkt, die Sie bei der Entscheidung berücksichtigen müssen. Beispiel:

* Einige Features sind möglicherweise noch nicht vollständig in v2.0 implementiert. Ihre App funktioniert z. B. möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfeatures wie [bedingten Gerätezugriff](https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies) aktiviert.
* Sie können Microsoft Graph nicht von einer [eigenständigen Web-API](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#restrictions-on-app-types) aus aufrufen. 
* Sie können keine Apps von Cloud-Lösungsanbietern aufrufen.
* [Integrierte Windows-Authentifizierung für Partnermandanten](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#restrictions-for-work-and-school-accounts) wird nicht unterstützt. Dies bedeutet, dass Benutzer von Azure AD-Partnermandanten sich nicht im Hintergrund mit ihrer lokalen Active Directory-Instanz authentifizieren können. Sie müssen ihre Anmeldeinformationen erneut eingeben.

Weitere Informationen zu den Unterschieden zwischen dem Azure AD v2.0- und dem Azure AD-Endpunkt finden Sie unter [Wo liegen die Unterschiede beim v2.0-Endpunkt?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare)

>**Wichtig**
>
>**Bevor Sie eine Entscheidung bzgl. des Endpunkts treffen, den Sie zum Entwickeln einer App für die Produktion verwenden möchten, lesen Sie die Informationen unter [Sollte ich den v2.0-Endpunkt verwenden?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations)**

## <a name="next-steps"></a>Nächste Schritte

Sobald Sie Ihre App registriert haben, können Sie loslegen.

- Eine Kurzanleitung zum Abrufen eines Zugriffstokens für Apps, die Microsoft Graph im Namen eines Benutzers aufrufen, finden Sie unter [Im Namen eines Benutzers zugreifen](auth_v2_user.md).
- Eine Kurzanleitung zum Abrufen eines Zugriffstokens für Apps, die Microsoft Graph ohne Benutzer aufrufen, finden Sie unter [Ohne Benutzer zugreifen](auth_v2_service.md).
- Informationen über die Berechtigungen, die Sie mit Microsoft Graph verwenden können, finden Sie unter [Berechtigungen](permissions_reference.md).
- Wenn Sie ein Microsoft Cloud-Lösungsanbieter sind, der über Microsoft Graph auf partnerverwaltete Kundendaten zugreifen möchten, finden Sie weitere Informationen unter [App-Zugriff verwalten (CSPs)](auth_cloudsolutionprovider.md).


Wenn Sie mit dem Code beginnen möchten, können Sie die folgenden Ressourcen zu Hilfe nehmen, die Sie bei der Implementierung von Authentifizierung und Autorisierung mit Azure AD in Ihrer App unterstützen.

### <a name="microsoft-graph-connect-samples"></a>Microsoft Graph Connect-Codebeispiele 

Microsoft veröffentlicht Connect-Codebeispiele für Microsoft Graph für eine Vielzahl von Plattformen, z. B.: Android, Angular.JS, ASP.NET, iOS (Obj-C und Swift), Node.JS, PHP, Python, Ruby, UWP und Xamarin. In diesen Beispielen können Sie Code untersuchen, der verschiedene Authentifizierungsbibliotheken verwendet, um Token aus Azure AD abzurufen. Die meisten Codebeispiele verwenden derzeit Authentifizierungsbibliotheken von Drittanbietern; in den Beispielen für ASP.NET und UWP werden jedoch Microsoft-Bibliotheken verwendet.

- Der Abschnitt [Die erste App erstellen](get-started.md) enthält detaillierte Artikel, in den beschrieben wird, wie Sie Connect-Apps mit dem Azure AD v2.0-Endpunkt erstellen. Außerdem werden die Authentifizierungsbibliotheken erläutert, die auf den einzelnen Plattformen verwendet werden. Die verfügbaren Codebeispiele sind nach Plattform und Authentifizierungsendpunkt gegliedert aufgeführt.
- Um schnell ein funktionsfähiges Codebeispiel auf der Plattform Ihrer Wahl zu erhalten, wechseln Sie zum [Microsoft Graph-Schnellstart](https://developer.microsoft.com/graph/Quick-Start).
- Besuchen Sie das [Microsoft Graph-Repository](https://github.com/microsoftgraph) auf GitHub, um alle verfügbaren Codebeispiele für Microsoft Graph anzuzeigen. 

### <a name="azure-active-directory-samples-and-documentation"></a>Azure Active Directory-Codebeispiele und -Dokumentation 
Die Azure AD-Dokumentation enthält Artikel und Codebeispiele, die sich auf Authentifizierung und Autorisierung mit Azure AD konzentrieren.

Für den Azure AD v2.0-Endpunkt: 

- Der einfachste Ausgangspunkt ist die [Dokumentation zum Azure AD v2.0-Endpunkt ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview). Dieser Artikel enthält Links zu Übersichten, Protokolldokumentation und Erste-Schritte-Artikeln für verschiedene Plattformen, alle organisiert nach dem App-Typ, den Sie entwickeln. 
- Nach Client- oder Server-Authentifizierungsbibliothek gegliederte Codebeispiele finden Sie unter [Azure Active Directory v2.0-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries). 
- Im [Katalog der Azure-Codebeispiele](https://azure.microsoft.com/resources/samples/?service=active-directory) können Sie die Azure AD-Codebeispiele alternativ nach Plattform erkunden. Hinweis: Sie können Ihre Suche nicht nach Endpunktversion einschränken. 

Für den Azure AD-Endpunkt: 

- Der einfachste Ausgangspunkt ist die [Übersicht des Leitfadens „Azure Active Directory für Entwickler“](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide). Dieser Artikel enthält Links zu Übersichten, Protokolldokumentation und Erste-Schritte-Artikeln für verschiedene Plattformen, alle organisiert nach dem App-Typ, den Sie entwickeln. 
- Nach Client- oder Server-Authentifizierungsbibliothek gegliederte Codebeispiele finden Sie unter [Azure Active Directory-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries). 
- Nach App-Typ und Plattform gegliederte Codebeispiele finden Sie unter [Azure Active Directory-Codebeispiele](https://docs.microsoft.com/azure/active-directory/develop/active-directory-code-samples).
- Im [Katalog der Azure-Codebeispiele](https://azure.microsoft.com/resources/samples/?service=active-directory) können Sie die Azure AD-Codebeispiele alternativ nach Plattform erkunden. Hinweis: Sie können Ihre Suche nicht nach Endpunktversion einschränken. 


## <a name="see-also"></a>Siehe auch

- [Dokumentation zum Azure Active Directory-Endpunkt](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)
- [Dokumentation zum Azure Active Directory v2.0-Endpunkt](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)
