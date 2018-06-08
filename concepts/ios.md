# <a name="ios-samples-for-the-microsoft-graph-api"></a>iOs-Beispiele für die Microsoft Graph-API
Dieser Artikel führt zwei iOS-Beispiele ein, in denen ein Benutzer von Office 365- oder Managed Service-Konten (MSA), wie z. B. Consumer Outlook-Benutzer, authentifiziert wird. In beiden Beispielen wird eine E-Mail über den Outlook-Dienst versandt, aber in einem der Beispiele wird die Funktion erweitert, indem das Profilfoto des Benutzers im Textkörper der E-Mail versandt wird.

## <a name="ios-objective-c-connect-rest-sample"></a>Beispiel für iOS-Ziel-C-Connect-REST
In diesem Beispiel wird eine standardmäßige iOS-HTTPS-Bibliothek für REST-Aufrufe zu Microsoft Graph verwendet. Das Beispiel verwendet die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-objc/blob/dev/README.md) für die Authentifizierung eines Benutzers. Die MSAL-Bibliothek authentifiziert den Benutzer eines Office 365- oder MSA-Kontos. Benutzer einer lokalen Azure Active Directory-Instanz können jedoch nicht authentifiziert werden.

Sie können eine E-Mail-Nachricht mit diesem Beispiel versenden, aber das Foto des authentifizierten Benutzers wird nicht aufgerufen oder eingebettet.

- [Erste Schritte mit Microsoft Graph in einer Ziel-C-iOS-App](ios_objectivec.md)

## <a name="ios-swift-connect-rest-sample"></a>iOS Swift Connect-REST-Beispiel
In diesem Beispiel wird die Foundation-HTTP-Bibliothek und [PromiseKit](https://github.com/mxcl/PromiseKit/blob/master/README.md) für den Zugriff auf den Microsoft Graph-Endpunkt unter Verwendung von REST-Vorgängen mit dem asynchronen **Promises**-Muster verwendet. Das Beispiel verwendet die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-objc/blob/dev/README.md) für die Authentifizierung eines Benutzers. Mit dieser Bibliothek kann die App einen Benutzer von Office 365 oder einen MSA-Benutzer authentifizieren.

Im Beispiel wird der Zugriff mit Graph auf das Azure-Profil des Benutzers verdeutlicht. Sie erfahren außerdem, wie Sie das Profilfoto des Benutzers abrufen, es auf den OneDrive-Speicher des Benutzers hochladen und in den Textkörper einer E-Mail-Nachricht in Outlook einbetten können.

- [Erste Schritte mit Microsoft Graph in einer iOS-App](ios_swift.md)
