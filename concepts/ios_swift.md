# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="3c48c-101">Erste Schritte mit Microsoft Graph in einer Swift iOS-App</span><span class="sxs-lookup"><span data-stu-id="3c48c-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="3c48c-p101">**Sie erstellen Apps für Unternehmenskunden?** Ihre App funktioniert möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfunktionen wie <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">bedingten Gerätezugriff</a> aktiviert. In diesem Fall treten bei Ihren Kunden möglicherweise Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="3c48c-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="3c48c-p102">Zur Unterstützung **aller Unternehmenskunden** über **alle Unternehmensszenarien** hinweg müssen Sie den Azure AD-Endpunkt verwenden und Ihre Apps mithilfe des [Azure-Portals](https://aka.ms/aadapplist) verwalten. Weitere Informationen finden Sie unter [Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="3c48c-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="3c48c-p103">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom [Azure AD v2.0-Endpunkt](https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth) und zum Aufrufen von Microsoft Graph. Er führt Sie durch den Code im [Office 365 Connect-Beispiel für iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) und erläutert die wichtigsten Konzepte, die in einer App implementiert werden müssen, die Microsoft Graph verwendet. In diesem Artikel wird auch beschrieben, wie Sie mithilfe des [Microsoft Graph SDK für iOS](https://github.com/microsoftgraph/msgraph-sdk-ios) auf Microsoft Graph zugreifen.</span><span class="sxs-lookup"><span data-stu-id="3c48c-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="3c48c-110">Sie können die Version der App, die Sie erstellen, aus diesem GitHub Repository herunterladen:</span><span class="sxs-lookup"><span data-stu-id="3c48c-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="3c48c-111">Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs</span><span class="sxs-lookup"><span data-stu-id="3c48c-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-swift-connect-sample)

<span data-ttu-id="3c48c-112">In der folgenden Abbildung ist die App dargestellt, die Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="3c48c-112">The following image shows the app you'll create.</span></span>

![Die exemplarische Vorgehensweise im Connect-Beispiel zeigt die Herstellung einer Verbindung und das Senden einer E-Mail in der App.](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="3c48c-114">Der Workflow beinhaltet das Herstellen einer Verbindung zu Microsoft Graph sowie die Authentifizierung, das Anmelden mit Ihrem Büro- oder persönlichen Konto und schließlich das Senden einer E-Mail an einen Empfänger.</span><span class="sxs-lookup"><span data-stu-id="3c48c-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="3c48c-p104">**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Schnellstart Microsoft Graph](https://graph.microsoft.io/de-DE/getting-started).</span><span class="sxs-lookup"><span data-stu-id="3c48c-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/de-DE/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c48c-117">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3c48c-117">Prerequisites</span></span>

<span data-ttu-id="3c48c-118">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="3c48c-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="3c48c-119">[Xcode](https://developer.apple.com/xcode/downloads/) von Apple</span><span class="sxs-lookup"><span data-stu-id="3c48c-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="3c48c-120">Installation von [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) als ein Abhängigkeits-Manager.</span><span class="sxs-lookup"><span data-stu-id="3c48c-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="3c48c-121">Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="3c48c-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="3c48c-122">Das [Microsoft Graph Startprojekt für iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="3c48c-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="3c48c-123">Diese Vorlage enthält Klassen, denen Sie Code hinzufügen müssen.</span><span class="sxs-lookup"><span data-stu-id="3c48c-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="3c48c-124">Sie rufen dieses Projekt ab, indem Sie das Beispielprojekt von diesem Speicherort aus klonen oder herunterladen. Dann arbeiten Sie mit dem Arbeitsbereich innerhalb des Ordners **Startprojekt** (**ios-objectivec-connect-sample.xcworkspace**).</span><span class="sxs-lookup"><span data-stu-id="3c48c-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="3c48c-125">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="3c48c-125">Register the app</span></span>
 
1. <span data-ttu-id="3c48c-126">Melden Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="3c48c-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="3c48c-127">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="3c48c-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="3c48c-128">Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="3c48c-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="3c48c-129">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="3c48c-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="3c48c-130">Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="3c48c-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="3c48c-131">Wählen Sie **Systemeigene Plattform**.</span><span class="sxs-lookup"><span data-stu-id="3c48c-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="3c48c-p106">Kopieren Sie die Client-ID in die Zwischenablage. Sie müssen diesen Wert in die Beispiel-App eingeben.</span><span class="sxs-lookup"><span data-stu-id="3c48c-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="3c48c-134">Die App-ID ist ein eindeutiger Bezeichner für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="3c48c-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="3c48c-135">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="3c48c-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="3c48c-136">Importieren der Projekt-Abhängigkeiten</span><span class="sxs-lookup"><span data-stu-id="3c48c-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="3c48c-137">Klonen Sie dieses Repository, [Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="3c48c-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="3c48c-138">WICHTIG: Verwenden Sie das Beispiel im Startprojekt-Ordner und nicht im Beispiel auf der Stammebene des Projekts.</span><span class="sxs-lookup"><span data-stu-id="3c48c-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="3c48c-p107">Verwenden Sie CocoaPods, um das Microsoft Graph-SDK und Authentifizierungsabhängigkeiten zu importieren: Diese Beispiel-App enthält bereits eine POD-Datei, die die Pods in das Projekt überträgt. Navigieren Sie zu dem Ordner **Startprojekt** in der **Terminal** -App und führen Sie von **Terminal** folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="3c48c-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="3c48c-p108">Sie erhalten eine Bestätigung, dass die Pods in das Projekt importiert wurden. Weitere Informationen finden Sie unter [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span><span class="sxs-lookup"><span data-stu-id="3c48c-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="3c48c-144">Aktivieren der Schlüsselbundfreigabe</span><span class="sxs-lookup"><span data-stu-id="3c48c-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="3c48c-p109">Für Xcode 8 müssen Sie die Schlüsselbundgruppe hinzufügen, sonst kann Ihre App nicht auf den Schlüsselbund zugreifen. So fügen Sie die Schlüsselbundgruppe hinzu:</span><span class="sxs-lookup"><span data-stu-id="3c48c-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="3c48c-p110">Wählen Sie im Projekt-Manager-Bereich in Xcode das Projekt aus. (⌘ + 1).</span><span class="sxs-lookup"><span data-stu-id="3c48c-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="3c48c-149">Wählen Sie **iOS-ObjectiveC-Connect-Sample**.</span><span class="sxs-lookup"><span data-stu-id="3c48c-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="3c48c-150">Aktivieren Sie auf der Registerkarte „Funktionen“ die Option **Schlüsselbundfreigabe**.</span><span class="sxs-lookup"><span data-stu-id="3c48c-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="3c48c-151">Fügen Sie **com.microsoft.ios-objectivec-connect-sample** zu den Schlüsselbundgruppen hinzu.</span><span class="sxs-lookup"><span data-stu-id="3c48c-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="3c48c-152">Authentifizieren mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3c48c-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="3c48c-153">Für den Zugriff auf den Benutzeroberflächenworkflow muss die App den Benutzer authentifizieren, sodass dieser dann eine E-Mail an einen bestimmten Benutzer senden kann.</span><span class="sxs-lookup"><span data-stu-id="3c48c-153">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user.</span></span> <span data-ttu-id="3c48c-154">Für Anforderungen beim Microsoft Graph-Dienst muss ein Authentifizierungsanbieter bereitgestellt werden, der HTTPS-Anforderungen mit einem entsprechenden OAuth 2.0-Bearertoken authentifizieren kann.</span><span class="sxs-lookup"><span data-stu-id="3c48c-154">To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="3c48c-155">Im Beispielprojekt liegt eine Authentifizierungsstruktur mit der Bezeichnung **Authentication.swift.** bereits als Stub vor.</span><span class="sxs-lookup"><span data-stu-id="3c48c-155">In the sample project there's an authentication structure already stubbed out called **Authentication.swift.**</span></span> <span data-ttu-id="3c48c-156">Wir fügen eine Funktion zum Anfordern und Erwerben eines Zugriffstokens für den Aufruf der Microsoft Graph-API hinzu.</span><span class="sxs-lookup"><span data-stu-id="3c48c-156">We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="3c48c-157">Öffnen Sie den Xcode-Projektarbeitsbereich (**Graph-iOS-Swift-Connect.xcworkspace**) und öffnen Sie die Struktur- Erweiterungsdatei **Authentication.swift**. Suchen Sie den folgenden Code in dieser Erweiterung.</span><span class="sxs-lookup"><span data-stu-id="3c48c-157">Open the Xcode project workspace (**Graph-iOS-Swift-Connect.xcworkspace**), and open the structure extension file **Authentication.swift** Find the following code in that extension.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph. 
     If a user has previously signed in before and not disconnected, silent log in
     will take place. 
     If not, authentication will ask for credentials
     */
    func connectToGraph(withClientId clientId: String,
                                     scopes: [String],
                                     completion:@escaping (_ error: MSGraphError?) -> Void) {
    
        // Set client ID
        NXOAuth2AuthenticationProvider.setClientId(clientId, scopes: scopes)
        
        // Try silent log in. This will attempt to sign in if there is a previous successful
        // sign in user information.
        if NXOAuth2AuthenticationProvider.sharedAuth().loginSilent() == true {
            completion(nil)
        }
        // Otherwise, present log in controller.
        else {
            NXOAuth2AuthenticationProvider.sharedAuth()
                .login(with: nil) { (error: Error?) in
                    
                    if let nserror = error {
                        completion(MSGraphError.nsErrorType(error: nserror as NSError))
                    }
                    else {
                        completion(nil)
                    }
            }
        }
    }
  ```


2. <span data-ttu-id="3c48c-158">Wir rufen diese Methode aus **ConnectViewController.swift**  heraus auf.</span><span class="sxs-lookup"><span data-stu-id="3c48c-158">We'll call this method from **ConnectViewController.swift**.</span></span> <span data-ttu-id="3c48c-159">Dieser Controller ist die Standardansicht, die die App lädt, und es gibt eine einzelne Schaltfläche mit dem Namen **Verbinden**, die der Benutzer antippt, um den Authentifizierungsprozess zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="3c48c-159">This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process.</span></span> <span data-ttu-id="3c48c-160">Diese Methode akzeptiert einen einzigen Parameter, die **Bereiche**, die unten näher erläutert werden.</span><span class="sxs-lookup"><span data-stu-id="3c48c-160">This method takes in one parameter, the **scopes**, we'll discuss scopes in more detail below.</span></span> <span data-ttu-id="3c48c-161">Fügen Sie die folgende Aktion zu **ConnectViewController.swift** hinzu.</span><span class="sxs-lookup"><span data-stu-id="3c48c-161">Add the following action to **ConnectViewController.swift**.</span></span>

  ```swift
  // MARK: Authentication
  private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        
        let clientId = ApplicationConstants.clientId
        let scopes = ApplicationConstants.scopes
        
        authentication.connectToGraph(withClientId: clientId, scopes: scopes) {
            (error) in
            
            defer {self.loadingUI(show: false)}
            
            if let graphError = error {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
            }
            else {
                self.performSegue(withIdentifier: "showSendMail", sender: nil)
            }
        }
    }
  }

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="3c48c-162">Senden einer E-Mail mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3c48c-162">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="3c48c-163">Nachdem das Projekts für die Authentifizierung konfiguriert wurde, werden in den nächsten Schritten die authentifizierte E-Mail-Adresse, der Anzeigename und das Profilfoto des Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="3c48c-163">After configuring the project to be able to authenticate, the next tasks are getting the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="3c48c-164">Nachdem das Beispiel diese Werte erhalten hat, lädt es das Profilbild in OneDrive und ruft die Freigabe-Url des Bildes ab.</span><span class="sxs-lookup"><span data-stu-id="3c48c-164">After the sample gets these values it uploads the profile picture to OneDrive and gets the sharing Url of the picture.</span></span> <span data-ttu-id="3c48c-165">Schließlich wird mithilfe der Microsoft Graph-API eine E-Mail an einen Benutzer gesendet.</span><span class="sxs-lookup"><span data-stu-id="3c48c-165">Finally, it sends a mail to a user using the Microsoft Graph API.</span></span> 

<span data-ttu-id="3c48c-166">Standardmäßig ist der angemeldete Benutzer der Empfänger, aber Sie haben die Möglichkeit, einen beliebigen anderen Empfänger anzugeben.</span><span class="sxs-lookup"><span data-stu-id="3c48c-166">By default the logged in user will be the recipient, but you have the ability to change it to any other recipient.</span></span> <span data-ttu-id="3c48c-167">Der Code, den wir hier verwenden, gehört zur Klasse **SendMailViewController.swift.**</span><span class="sxs-lookup"><span data-stu-id="3c48c-167">The code we'll work with here is in the class **SendMailViewController.swift.**</span></span> <span data-ttu-id="3c48c-168">Sie werden sehen, dass es hier noch anderen Code für die Benutzeroberfläche und eine Hilfsmethode zum Abrufen von Benutzerprofildaten aus dem Microsoft Graph-Dienst gibt.</span><span class="sxs-lookup"><span data-stu-id="3c48c-168">You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service.</span></span> <span data-ttu-id="3c48c-169">Wir werden uns auf die Methoden zum Erstellen einer E-Mail-Nachricht und das Senden dieser Nachricht konzentrieren.</span><span class="sxs-lookup"><span data-stu-id="3c48c-169">We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="3c48c-170">Öffnen Sie **SendMailViewController.swift.**</span><span class="sxs-lookup"><span data-stu-id="3c48c-170">Open **SendMailViewController.swift.**</span></span>  <span data-ttu-id="3c48c-171">Suchen Sie den E-Mail-Textkörper für die Erstellung der Hilfsmethode in der Klasse:</span><span class="sxs-lookup"><span data-stu-id="3c48c-171">and find the mail body creating helper method in the class:</span></span>

  ```swift
    /**
     Creates sample email message
     
     - parameter emailAddress: recipient email address
     
     - returns: MSGraphMessage object with given recipient. The body is created from EmailBody.html
     */
    func createSampleMessage(to emailAddress: String, picLink pictureUrl: String) -> MSGraphMessage? {
        let message = MSGraphMessage()
        
        // set recipients
        
        let _ = self.userPicture
        let toRecipient = MSGraphRecipient()
        let msEmailAddress = MSGraphEmailAddress()
        msEmailAddress.address = emailAddress
        toRecipient.emailAddress = msEmailAddress
        let toRecipientList = [toRecipient]
        message.toRecipients = toRecipientList
        message.subject = NSLocalizedString("MAIL_SUBJECT", comment: "")
        let messageBody = MSGraphItemBody()
        messageBody.contentType = MSGraphBodyType.html()
        guard let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html") else {return nil}
        messageBody.content = try! String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
        messageBody.content = messageBody.content.replacingOccurrences(of: "a href=%s", with: ("a href=" + pictureUrl))
        message.body = messageBody

        if let unwrappedImage = self.userPicture {
            let fileAttachment = MSGraphFileAttachment()
            let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
            fileAttachment.contentType = "image/png"
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment"
            fileAttachment.contentBytes = data?.base64EncodedString()
            fileAttachment.name = "me.png"
            message.attachments.append(fileAttachment)
        }
        return message
    }

  ```
2. <span data-ttu-id="3c48c-172">Suchen Sie die folgende Hilfsmethoden, um Benutzerinformationen und ein Profilfoto abzurufen und das Foto auf OneDrive hochzuladen:</span><span class="sxs-lookup"><span data-stu-id="3c48c-172">find the following helper methods for getting user information, getting a profile photograph, and uploading the photograph to OneDrive:</span></span>

  ```swift
      /**
     Fetches user information such as mail and display name
     */
    func getUserInfo() {
        self.sendButton.isEnabled = false
        self.statusTextView.text = NSLocalizedString("LOADING_USER_INFO", comment: "")
        
        self.graphClient.me().request().getWithCompletion {
            (user: MSGraphUser?, error: Error?) in
            if let graphError = error {
                print(NSLocalizedString("ERROR", comment: ""), graphError)
                DispatchQueue.main.async(execute: {
                    self.statusTextView.text = NSLocalizedString("GRAPH_ERROR", comment: "")
                })
            }
            else {
                guard let userInfo = user else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_FAILURE", comment: "")
                    })
                    return
                }
                DispatchQueue.main.async(execute: {
                    self.emailTextField.text = userInfo.mail
                    
                    if let displayName = userInfo.displayName {
                        self.headerLabel.text = "Hi " + displayName
                    }
                    else {
                        self.headerLabel.text = NSString(format: NSLocalizedString("HI_USER", comment: "") as NSString, "") as String
                    }
                    
                    self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_SUCCESS", comment: "")
                    self.sendButton.isEnabled = true
                })
            }
        }
    }
    
    /**
     Uploads the user's profile picture (obtained via the Graph API) to the user's OneDrive drive. The OneDrive sharing url is
     returned in the completion handler.
    */
    func uploadPictureToOneDrive(uploadFile image: UIImage?, with completion: @escaping (_ result: GraphResult<String, NSError>) ->Void) {
        
        var webUrl: String = ""
        guard let unwrappedImage = image else {
            return
        }
        let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
        self.graphClient
            .me()
            .drive()
            .root()
            .children()
            .driveItem("me.png")
            .contentRequest()
            .upload(from: data, completion: {
                (driveItem: MSGraphDriveItem?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("UPLOAD_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return

                } else {
                    webUrl = (driveItem?.webUrl)!
                    completion(.success(webUrl))
                }
            })
    }


    /**
     Gets the user's profile picture. Returns the picture as a UIImage via completion handler
    */
    func getUserPicture(forUser upn: String, with completion: @escaping (_ result: GraphResult<UIImage, NSError>) -> Void) {
        
        //Asynchronous Graph call. Closure is invoked after getUserPicture completes. Requires @escaping attribute
        self.graphClient.me().photoValue().download {
            (url: URL?, response: URLResponse?, error: Error?) in
            
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return
                }
                guard let picUrl = url else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "User profile picture is nil")
                    })
                    return
                }
                print(picUrl)
            
                let picData = NSData(contentsOf: picUrl)
                let picImage = UIImage(data: picData! as Data)
            
                if let validPic = picImage {
                    completion(.success(validPic))
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "Picture data is invalid")
                    })
                }
            }
    }

  ```

3. <span data-ttu-id="3c48c-173">Suchen Sie die folgende Methode zum Versenden einer E-Mail-Nachricht in der Klasse.</span><span class="sxs-lookup"><span data-stu-id="3c48c-173">Find the following send mail method in the class.</span></span>  

  ```swift
    @IBAction func sendMail(_ sender: AnyObject) {
        guard let toEmail = self.emailTextField.text else {return}
        guard let picUrl = self.userPictureUrl else {return}
        if let message = self.createSampleMessage(to: toEmail, picLink: picUrl) {
            
            let requestBuilder = graphClient.me().sendMail(with: message, saveToSentItems: false)
            let mailRequest = requestBuilder?.request()
            
            _ = mailRequest?.execute(completion: {
                (response: [AnyHashable: Any]?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("SEND_FAILURE", comment: "")
                    })
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.descriptionLabel.text = "Check your inbox. You have a new message :)"
                        self.statusTextView.text = NSLocalizedString("SEND_SUCCESS", comment: "")
                    })
                }
            })
        }
    }

  ```


## <a name="run-the-app"></a><span data-ttu-id="3c48c-174">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="3c48c-174">Run the app</span></span>
1. <span data-ttu-id="3c48c-175">Vor dem Ausführen des Beispiels müssen Sie die Client-ID angeben, die Sie bei dem Registrierungsvorgang im Abschnitt **Registrieren der App** erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="3c48c-175">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="3c48c-176">Öffnen Sie **ApplicationConstants.swift**.</span><span class="sxs-lookup"><span data-stu-id="3c48c-176">Open **ApplicationConstants.swift** .</span></span> <span data-ttu-id="3c48c-177">Sie werden sehen, dass die ClientID aus dem Registrierungsprozess am Anfang der Datei hinzugefügt werden kann:</span><span class="sxs-lookup"><span data-stu-id="3c48c-177">You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  

  ```swift
struct ApplicationConstants {
    static let clientId = "Enter_Client_Id_Here"
    static let scopes   = ["openid", "profile", "Mail.ReadWrite","mail.send","Files.ReadWrite","User.ReadBasic.All"]
}


  ```

> <span data-ttu-id="3c48c-p117">Hinweis: Sie sehen, dass die folgenden Berechtigungsbereiche für dieses Projekt konfiguriert wurden: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. Die in diesem Projekt verwendeten Dienstaufrufe, also das Senden einer E-Mail an Ihr E-Mail-Konto und das Abrufen einiger Profilinformationen (Anzeigename, E-Mail-Adresse), benötigen diese Berechtigungen, damit die App ordnungsgemäß ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="3c48c-p117">Note: You'll notice that the following permission scopes have been configured for this project: "https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access". The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="3c48c-180">Führen Sie das Beispiel aus, tippen Sie auf **Verbinden**, melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an und gewähren Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="3c48c-180">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="3c48c-p118">Klicken Sie auf die Schaltfläche **E-Mail senden**.
 Nachdem die E-Mail gesendet wurde, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3c48c-p118">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3c48c-183">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="3c48c-183">Next steps</span></span>
- <span data-ttu-id="3c48c-184">Testen Sie die REST-API mithilfe des [Graph-Explorers](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="3c48c-184">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="3c48c-185">Beispiele allgemeiner Vorgänge sowohl für REST- als auch für SDK-Operationen finden Sie in dem Beispiel [Microsoft Graph iOS Objective C Code Snippets](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="3c48c-185">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="3c48c-186">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="3c48c-186">See also</span></span>
- [<span data-ttu-id="3c48c-187">Azure AD v2.0-Protokolle</span><span class="sxs-lookup"><span data-stu-id="3c48c-187">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="3c48c-188">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="3c48c-188">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-tokens/)
