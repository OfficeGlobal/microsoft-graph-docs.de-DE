# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a>Erste Schritte mit Microsoft Graph in einer Swift iOS-App

> **Sie erstellen Apps für Unternehmenskunden?** Ihre App funktioniert möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfunktionen wie <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">bedingten Gerätezugriff</a> aktiviert. In diesem Fall treten bei Ihren Kunden möglicherweise Fehler auf. 

> Zur Unterstützung **aller Unternehmenskunden** über **alle Unternehmensszenarien** hinweg müssen Sie den Azure AD-Endpunkt verwenden und Ihre Apps mithilfe des [Azure-Portals](https://aka.ms/aadapplist) verwalten. Weitere Informationen finden Sie unter [Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom [Azure AD v2.0-Endpunkt](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) und zum Aufrufen von Microsoft Graph. Er führt Sie durch den Code im [Office 365 Connect-Beispiel für iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) und erläutert die wichtigsten Konzepte, die in einer App implementiert werden müssen, die Microsoft Graph verwendet. In diesem Artikel wird auch beschrieben, wie Sie mit REST-Vorgängen in einem asynchronen **Zusagenkette**-Muster auf Microsoft Graph zugreifen. Zusagen im Beispiel werden mit dem [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPod implementiert. 

Das Beispiel wurde mit **XCode 9.2** und **Swift 3.2** erstellt.

Sie können die Version der App, die Sie erstellen, aus diesem GitHub Repository herunterladen:

* [Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

In der folgenden Abbildung ist die App dargestellt, die Sie erstellen.

![Die exemplarische Vorgehensweise im Connect-Beispiel zeigt die Herstellung einer Verbindung und das Senden einer E-Mail in der App](./images/iOSConnectWalkthrough.png)


Der Workflow authentifiziert und autorisiert das Beispiel für den Zugriff auf Microsoft Graph-Ressourcen, meldet sich mit Ihrem Geschäfts- oder persönlichen Konto an und sendet schließlich eine E-Mail an einen Empfänger.

**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Microsoft Graph-Schnellstart](https://developer.microsoft.com/en-us/graph/quick-start).

## <a name="prerequisites"></a>Voraussetzungen

Für die ersten Schritte benötigen Sie: 

* [Xcode](https://developer.apple.com/xcode/downloads/) von Apple
* Installation von [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) als ein Abhängigkeits-Manager.
* Installation von [Carthage](https://github.com/Carthage/Carthage) zum Importieren und Erstellen der **MSAL**-Bibliothek.
* Installation von [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod. 
* Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)

## <a name="register-the-app"></a>Registrieren der App
 
1. Melden Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.
2. Klicken Sie auf **App hinzufügen**.
3. Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.
    
    Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.
 
4. Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** aus.
5. Wählen Sie **Systemeigene Plattform**.
6. Kopieren Sie die Client-ID in die Zwischenablage. Sie müssen diesen Wert in die Beispiel-App eingeben.

    Die App-ID ist ein eindeutiger Bezeichner für Ihre App. 

7. Klicken Sie auf **Speichern**.

## <a name="importing-the-project-dependencies"></a>Importieren der Projekt-Abhängigkeiten

1. Klonen Sie dieses Repository: [Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs](https://github.com/microsoftgraph/ios-swift-connect-rest-sample). 


2. Verwenden Sie CocoaPods, um die PromiseKit-Abhängigkeiten zu importieren. Diese Beispiel-App enthält bereits eine POD-Datei, die die Pods in das Projekt überträgt. Navigieren Sie zum Stammordner des Projekts in der **Terminal**-App, und führen Sie über **Terminal** Folgendes aus:

        pod install

   Sie erhalten eine Bestätigung, dass die Pods in das Projekt importiert wurden. Weitere Informationen finden Sie unter [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)

## <a name="install-the-msal-authentication-framework"></a>Installieren des MSAL-Authentifizierungsframeworks

Die Vorschauversion von MSAL wird als Header- und Symboldateien über Carthage verteilt. Gehen Sie wie folgt vor, um MSAL im Projekt zu installieren:

1. Öffnen Sie das Bash-Terminal, und gehen Sie zum App-Stammordner.
2. Erstellen Sie eine **cartfile**: Kopieren Sie `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` in das Terminal, und führen Sie den Befehl aus.
3. Erstellen Sie eine MSAL-Bibliothek: Kopieren Sie `carthage update` in das Terminal, und führen Sie den Befehl aus.


## <a name="enable-keychain-sharing"></a>Aktivieren der Schlüsselbundfreigabe
 
Für Xcode 8 müssen Sie die Schlüsselbundgruppe hinzufügen, sonst kann Ihre App nicht auf den Schlüsselbund zugreifen. So fügen Sie die Schlüsselbundgruppe hinzu:
 
1. Wählen Sie das Projekt im Projekt-Manager-Bereich in Xcode aus. (⌘ + 1).
 
2. Wählen Sie das Ziel **O365-iOS-Microsoft-Graph-Connect-swift** aus.

3. Stellen Sie sicher, dass auf der Registerkarte **Allgemein** und im Abschnitt **Signatur** die Option für die **automatische Verwaltung von Signaturen** aktiviert ist und Sie über ein gültiges Signaturzertifikat verfügen.
 
3. Aktivieren Sie auf der Registerkarte **Funktionen** die Option **Schlüsselbundfreigabe**.
 
4. Wenn sich **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** nicht in der Liste der Schlüsselbundgruppen befindet, fügen Sie es hinzu.

## <a name="authenticating-with-microsoft-graph"></a>Authentifizieren mit Microsoft Graph

Der Workflow für die Benutzeroberfläche sieht wie folgt aus: Die App fordert den Benutzer zur Authentifizierung auf. Nach der Authentifizierung kann der Benutzer eine E-Mail an einen anderen Benutzer senden. Um Abfragen in Microsoft Graph durchzuführen, verwendet das Beispiel die **MSAL**-Authentifizierungsbibliothek für HTTPS-Authentifizierungsanforderungen mit einem entsprechenden OAuth 2.0-Bearertoken. Im Beispielprojekt importiert die **AuthenticationClass.swift.** die **MSAL**-Bibliothek und erwirbt das Zugriffstoken, das für Microsoft Graph-REST-Operationen erforderlich ist.

1. Öffnen Sie den **Xcode**-Projektarbeitsbereich (**Graph-iOS-Swift-Connect.xcworkspace**), und öffnen Sie die Klassendatei **AuthenticationClas.swift**. Suchen Sie den folgenden Code in dieser Klasse.


  ```swift
     /**
     Authenticates to Microsoft Graph.
     If a user has previously signed in before and not disconnected, silent log in
     will take place.
     If not, authentication will ask for credentials
     */
    func connectToGraph(scopes: [String],
                        completion:@escaping (_ error: ApplicationConstants.MSGraphError?, _ accessToken: String) -> Bool)  {
        do {
            if let initError = self.lastInitError {
                if initError.lengthOfBytes(using: String.Encoding.ascii) > 1 {
                    throw NSError.init(domain: initError, code: 0, userInfo: nil)
                }
            }
            // We check to see if we have a current logged in user. If we don't, then we need to sign someone in.
            // We throw an interactionRequired so that we trigger the interactive signin.
            if  try authenticationProvider.users().isEmpty {
                throw NSError.init(domain: "MSALErrorDomain", code: MSALErrorCode.interactionRequired.rawValue, userInfo: nil)
            } else {
                // Acquire a token for an existing user silently
                try authenticationProvider.acquireTokenSilent(forScopes: scopes, user: authenticationProvider.users().first) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        _ = completion(nil, self.accessToken);
                    } else {
                        //"Could not acquire token silently: \(error ?? "No error information" as! Error )"
                       var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            }
        }  catch let error as NSError {
            // interactionRequired means we need to ask the user to sign-in. This usually happens
            // when the user's Refresh Token is expired or if the user has changed their password
            // among other possible reasons.
            if error.code == MSALErrorCode.interactionRequired.rawValue {
                authenticationProvider.acquireToken(forScopes: scopes) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        var _ = completion(nil, self.accessToken);
                    } else  {
                        var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            } else {
                var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);

            }
        } catch {
            // This is the catch all error.
            var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);
        }
    }

  ```


2. Wir rufen die **connectToGraph**-Funktion von **ConnectViewController.swift** auf. Dieser Controller ist die Standardansicht, die die App mit einer einzelnen Schaltfläche mit dem Namen **Verbinden** lädt. Der Benutzer tippt darauf, um den Authentifizierungsprozess zu initiieren. 

  ```swift
// MARK: Authentication
private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        let scopes = ApplicationConstants.kScopes
        AuthenticationClass.sharedInstance?.connectToGraph( scopes: scopes) {
            (result: ApplicationConstants.MSGraphError?, accessToken: String) -> Bool  in
            defer {self.loadingUI(show: false)}
            if let graphError = result {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.userInfo)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
                return false
            }
            else {
                // run on main thread!!
                DispatchQueue.main.async {
                    self.performSegue(withIdentifier: "sendMail", sender: nil)
                }
                return true
            }
        }
    }
}

  ```

## <a name="send-an-email-with-microsoft-graph"></a>Senden einer E-Mail mit Microsoft Graph

Nachdem der Benutzer mit Microsoft Graph verbunden wurde, ruft das Beispiel die E-Mail-Adresse, den Anzeigenamen und das Profilfoto des authentifizierten Benutzers ab. Das Beispiel lädt das Profilfoto in den OneDrive-Stammordner des Benutzers hoch und fragt OneDrive nach der Freigabe-URL des Bilds. Zum Schluss sendet das Beispiel eine REST-Anforderung an Microsoft Graph zum Senden einer E-Mail-Nachricht an die angegebene E-Mail-Adresse. 

Der Nachrichtentext enthält den Freigabelink für das Bild sowie das Bild selbst als angefügte Bilddatei. Der Standardempfänger ist der authentifizierte Benutzer, wobei das Beispiel dem Benutzer jedoch auch ermöglicht, die E-Mail-Adresse eines anderen Benutzers anzugeben. 

Der Code, den wir hier verwenden, befindet sich in der Klasse **SendMailViewController_WithPromise.swift.** Die `viewDidLoad()`-Funktion liest den `self.emailTextField.text`-Wert, um die E-Mail-Adresse des Empfängers abzurufen, und beginnt dann eine **Zusagenkette**, um das Profilbild des authentifizierten Benutzers abzurufen. Wenn die Zusage abgelehnt wird, wird `sendMailButton` nicht aktiviert.

1. Öffnen Sie **SendMailViewController_WithPromise.swift.**, und suchen Sie die Funktion `viewDidLoad`. Die Funktion `self.userPictureWork` wird aufgerufen, um die Zusagenkette zu starten.

   ```swift
    override func viewDidLoad() {
        super.viewDidLoad()
        //Get user state values before creating mail message to be sent
        do
        {
            try self.userName = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].name!
            try self.emailTextField.text = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].displayableId
            self.userEmailAddress = self.emailTextField.text
            self.headerLabel.text = "Hi, \(self.userName! )"
            
            updateUI(showActivityIndicator: true, statusText: "Getting picture", sendMail: true)

            //Important: Break out of async promise chain by declaring result returns Void
            _ = self.userPictureWork().then{
                result -> Void in
                    self.userPictureUrl = (result[1] as! String)
                    self.userProfilePicture = (result[0] as! UIImage)
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)

            }.catch{err -> Void  in
                self.updateUI(showActivityIndicator: false, statusText: "", sendMail: false)

            }
        } catch _ as NSError{
            self.updateUI(showActivityIndicator: false,
                          statusText: "Error getting user profile picture.", sendMail: false)
        }
    }
  
   ```

   

1. Suchen Sie die Hilfsfunktion für Mailanforderungserstellungen in der Klasse:

   ```swift
    /**
     Prepare mail content by loading the JSON request payload template and HTML message body template from resources and replacing placeholders in the templates with appropriate values.
     */
    func mailContent() -> Data? {
        if let emailFilePath = Bundle.main.path(forResource: "EmailPostContent", ofType: "json"),
            let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html")
        {
            do {
                // Prepare upload content
                let emailContent = try String(contentsOfFile: emailFilePath, encoding: String.Encoding.utf8)
                let emailBodyRaw = try String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
                // Request doesn't accept a single quotation mark("), so change it to the acceptable form (\")
                var emailValidBody: String;
                emailValidBody = emailBodyRaw.replacingOccurrences(of: "\"", with: "\\\"")
                emailValidBody = emailValidBody.replacingOccurrences(of: "a href=%s", with: ("a href=" + self.userPictureUrl!))
                let imageData: NSData = UIImagePNGRepresentation(self.userProfilePicture!)! as NSData;
                let emailPostContent = emailContent.replacingOccurrences(of: "<EMAIL>", with: self.emailTextField.text!)
                    .replacingOccurrences(of: "<CONTENTTYPE>", with: "HTML")
                    .replacingOccurrences(of: "<CONTENT>", with: emailValidBody)
                    .replacingOccurrences(of: "<ODATA.TYPE>", with: "#microsoft.graph.fileAttachment")
                    .replacingOccurrences(of: "<IMAGE.TYPE>", with: "image\\/png")
                    .replacingOccurrences(of: "<CONTENTBYTES>", with: imageData.base64EncodedString())
                    .replacingOccurrences(of: "<NAME>", with: "me.png")
                // Return JSON payload with mail body as HTML string and attached picture as a file attachment of type NSData
                return emailPostContent.data(using: String.Encoding.utf8)
            }
            catch {
                // Error handling in case file loading fails.
                return nil
            }
        }
        // Error handling in case files aren't present.
        return nil
    }

   ```
2. Suchen Sie die folgenden Hilfsfunktionen zum Abrufen des Benutzerprofilbilds, zum Hochladen des Fotos in OneDrive und zum Anfordern eines Freigabelinks für das Bild:

   ```swift
    /**
      Async func. Get user's profile photo, upload photo to OneDrive, and get sharing link
     - returns:
        Promise<UIImage>. The user's profile picture
     */
    func getUserPicture()->Promise<UIImage?>{
        return Promise{ fulfill, reject in
            let urlRequest = self.buildRequest(operation: "GET", resource: "photo/$value") as URLRequest
            let task = URLSession.shared.dataTask(with:urlRequest){ data , res , err in
                if let err:Error = err {
                    print(err.localizedDescription)
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return fulfill(self.getDefaultPicture())
                }
                if let data = data {
                    if let userImage: UIImage = UIImage(data:data) {
                        self.userProfilePicture = userImage
                        return fulfill(userImage)
                    } else {
                        return reject("no image" as! Error)
                    }
                } else {
                    return fulfill(self.getDefaultPicture())
                }
            }
            task.resume()
        }
    }
    
    /**
     Async func. Uploads a UIImage object to the signed in user's OneDrive root folder
     - Returns:
        A Promise encapsulating an array of AnyObject. Element 0 contains the user profile photo obtained in the previous chained async call
        Element 1 contains the web sharing URL of the photo in OneDrive as a String
     - Parameters:
     - UIImage: The image to upload to OneDrive
     */
    func uploadPicture(photo: UIImage) -> Promise<[AnyObject]> {
        return Promise<[AnyObject]>{ fulfill, reject in
            let uploadRequestUrl = self.buildRequest(operation: "PUT", resource: "drive/root:/me.jpg:/content", content: UIImageJPEGRepresentation(photo, 1.0)!) as URLRequest
            let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                if let err = err{
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return reject(HTTPError.InvalidRequest)
                }
                //data can be serialized to a DriveItem object
                //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                var itemId: String = "";
                if let responseContent = data {
                    itemId = self.getValueFromResponse(json: responseContent, key: "id" )
                    var returnValues = [AnyObject]();
                    returnValues.append(photo as AnyObject)
                    returnValues.append(itemId as AnyObject)
                    return fulfill(returnValues)
                }
            }
            task.resume()
        }
    }

    /**
     Async func. Requests a new sharing link for the OneDrive item specified by the item id.
     - returns:
     - Promise<String: AnyObject>. The new sharing link and the image wrapped in a Promise
     */
    func createSharingLink(itemId: String, image: UIImage) ->Promise<[AnyObject]>{
        return Promise<[AnyObject]>{ fulfill, reject in
            //Create Data object for the JSON payload
            if let sharingLinkFilePath = Bundle.main.path(forResource: "CreateSharingLink", ofType: "json")
            {
                do {
                    let sharingLinkcontent = try String(contentsOfFile: sharingLinkFilePath, encoding: String.Encoding.utf8)
                    let jsonPayload: Data = sharingLinkcontent.data(using: String.Encoding.utf8)!
                    let uploadRequestUrl = self.buildRequest(
                        operation: "POST", resource: "drive/items/"+itemId+"/createLink", content: jsonPayload) as URLRequest
                    let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                        if let err = err{
                            return reject(err)
                        }
                        if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                            return reject(HTTPError.InvalidRequest)
                        }
                        //data can be serialized to a DriveItem object
                        //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                        var sharingLink: String = "";
                        if let responseContent = data {
                            do {
                                let resultJson = try JSONSerialization.jsonObject(
                                    with: responseContent, options: []) as? [String:AnyObject]
                                sharingLink = (OneDriveFileLink.init(json:resultJson!)?.webUrl)!

                            } catch let error as NSError {
                                print(error)
                            }
                            var returnValues = [AnyObject]();
                            returnValues.append(image as AnyObject)
                            returnValues.append(sharingLink as AnyObject)
                            return fulfill(returnValues)
                        }
                    }
                    task.resume()

                }
            }
        }
   ```

3. Suchen Sie die folgende Methode zum Senden von E-Mail in der Klasse.  
 
   ```swift
    /**
     POSTS a new message to the sendmail resource
     - parameters:
        - Data: The body of the message
     */
    func sendMailRESTWithContent(_ content: Data) {
        let _ = self.sendCRUDMessage(resource: "microsoft.graph.sendmail",
                                     operation: "POST",
                                     content: content)
    }
    
    /**
     Send a create, read, update, delete (CRUD) message.
     Create= POST, Update= PUT, Delete= DELETE.
     Read= GET. Use sendGETMessage(resource: String) to read Graph contents
     - returns:
     JSON response as Data
     - parameters:
        - String: The REST resource receiving the CRUD request
        - String: the REST operation requested
        - Data: The json (as Data) representing the values to update
     */
    func sendCRUDMessage(resource: String, operation:String, content: Data)->Data  {
        var returnData: Data;
        returnData = Data.init();
        if  (self.connectToGraph()){
            if (operation == "GET") {
                return self.sendGETMessage(resource: resource)
            }
            let request = self.buildRequest(operation: operation, resource: resource, content:content);
            let task = URLSession.shared.dataTask(with:request as URLRequest, completionHandler:{ data, res, err in
                if let err = err{
                    self.updateUI(showActivityIndicator: false,
                             statusText: "Error assembling the mail content." + err.localizedDescription, sendMail: false)
                }
                let nttpError = self.checkResult(result: res!)
                if (nttpError != HTTPError.NoError) {
                    self.updateUI(showActivityIndicator: false,
                                  statusText: "Error sending the mail.", sendMail: false)
                }
                else {
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)
                }
            }) // let task
             task.resume()
        }
        return returnData;
    }

   ```


## <a name="run-the-app"></a>Ausführen der App
1. Vor dem Ausführen des Beispiels müssen Sie die Client-ID angeben, die Sie bei dem Registrierungsvorgang im Abschnitt **Registrieren der App** erhalten haben. Öffnen Sie **Info.plist** als Quellcode. 

   - Ersetzen Sie `ENTER_CLIENT_ID_HERE` durch die **ClientID** aus dem Registrierungsprozess. Stellen Sie sicher, dass `msal` nicht ersetzt wird. Nachdem Sie die Zeichenfolge ersetzt haben, sieht der Array-Zeichenfolgenwert so aus: `msal48d31887-5fad-4d73-a9f5-3c356e68a038`. Hierbei ist der GUID-Teil **Ihre** Client-ID:  

   Beispiel: 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msalENTER_CLIENT_ID_HERE</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

     wird zu... 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msal48d31887-5fad-4d73-a9f5-3c356e68a038</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

> **Hinweis:** Sie stellen fest, dass dei folgenden Berechtigungsumfänge für dieses Projekt konfiguriert wurden: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` . Die in diesem Projekt verwendeten Dienstaufrufe, also das Senden einer E-Mail an Ihr E-Mail-Konto und das Abrufen einiger Profilinformationen (Anzeigename, E-Mail-Adresse) sowie das Schreiben in das OneDrive-Stammverzeichnis des Benutzers erfordern diese Berechtigungen, damit die App ohne Berechtigungsfehler ausgeführt wird.

2. Führen Sie das Beispiel aus, tippen Sie auf **Verbinden**, melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an und gewähren Sie die erforderlichen Berechtigungen.

3. Klicken Sie auf die Schaltfläche **E-Mail senden**. Nachdem die E-Mail gesendet wurde, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt.

## <a name="next-steps"></a>Nächste Schritte
- Testen Sie die REST-API mithilfe des [Graph-Testers](https://graph.microsoft.io/graph-explorer).
- Beispiele allgemeiner Vorgänge für SDK-Operationen finden Sie in dem Beispiel [Microsoft Graph iOS Objective C Snippets](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).

## <a name="see-also"></a>Siehe auch
- [Azure AD v2.0-Protokolle](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0-Tokens](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
