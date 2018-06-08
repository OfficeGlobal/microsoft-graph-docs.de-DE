# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="379f1-101">Erste Schritte mit Microsoft Graph in einer Swift iOS-App</span><span class="sxs-lookup"><span data-stu-id="379f1-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="379f1-p101">**Sie erstellen Apps für Unternehmenskunden?** Ihre App funktioniert möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfunktionen wie <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">bedingten Gerätezugriff</a> aktiviert. In diesem Fall treten bei Ihren Kunden möglicherweise Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="379f1-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="379f1-p102">Zur Unterstützung **aller Unternehmenskunden** über **alle Unternehmensszenarien** hinweg müssen Sie den Azure AD-Endpunkt verwenden und Ihre Apps mithilfe des [Azure-Portals](https://aka.ms/aadapplist) verwalten. Weitere Informationen finden Sie unter [Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="379f1-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="379f1-p103">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom [Azure AD v2.0-Endpunkt](https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth) und zum Aufrufen von Microsoft Graph. Er führt Sie durch den Code im [Office 365 Connect-Beispiel für iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) und erläutert die wichtigsten Konzepte, die in einer App implementiert werden müssen, die Microsoft Graph verwendet. In diesem Artikel wird auch beschrieben, wie Sie mit REST-Vorgängen in einem asynchronen **Zusagenkette**-Muster auf Microsoft Graph zugreifen. Zusagen im Beispiel werden mit dem [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPod implementiert.</span><span class="sxs-lookup"><span data-stu-id="379f1-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the **Microsoft Graph SDK for iOS**.</span></span> 

<span data-ttu-id="379f1-111">Das Beispiel wurde mit **XCode 9.2** und **Swift 3.2** erstellt.</span><span class="sxs-lookup"><span data-stu-id="379f1-111">The sample was created using **XCode 9.2** and **Swift 3.2**.</span></span>

<span data-ttu-id="379f1-112">Sie können die Version der App, die Sie erstellen, aus diesem GitHub Repository herunterladen:</span><span class="sxs-lookup"><span data-stu-id="379f1-112">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="379f1-113">Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs</span><span class="sxs-lookup"><span data-stu-id="379f1-113">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

<span data-ttu-id="379f1-114">In der folgenden Abbildung ist die App dargestellt, die Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="379f1-114">The following image shows the app you'll create.</span></span>

![Die exemplarische Vorgehensweise im Connect-Beispiel zeigt die Herstellung einer Verbindung und das Senden einer E-Mail in der App](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="379f1-116">Der Workflow authentifiziert und autorisiert das Beispiel für den Zugriff auf Microsoft Graph-Ressourcen, meldet sich mit Ihrem Geschäfts- oder persönlichen Konto an und sendet schließlich eine E-Mail an einen Empfänger.</span><span class="sxs-lookup"><span data-stu-id="379f1-116">The workflow authenticates and authorizes the sample to access  Microsoft Graph resources, signs in with your work or personal account, and finally sends a mail to a recipient.</span></span>

<span data-ttu-id="379f1-p104">**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Microsoft Graph-Schnellstart](https://developer.microsoft.com/de-DE/graph/quick-start).</span><span class="sxs-lookup"><span data-stu-id="379f1-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/de-DE/graph/quick-start) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="379f1-119">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="379f1-119">Prerequisites</span></span>

<span data-ttu-id="379f1-120">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="379f1-120">To get started, you'll need:</span></span> 

* <span data-ttu-id="379f1-121">[Xcode](https://developer.apple.com/xcode/downloads/) von Apple</span><span class="sxs-lookup"><span data-stu-id="379f1-121">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="379f1-122">Installation von [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) als ein Abhängigkeits-Manager.</span><span class="sxs-lookup"><span data-stu-id="379f1-122">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="379f1-123">Installation von [Carthage](https://github.com/Carthage/Carthage) zum Importieren und Erstellen der **MSAL**-Bibliothek.</span><span class="sxs-lookup"><span data-stu-id="379f1-123">Installation of [Carthage](https://github.com/Carthage/Carthage) to import and build the **MSAL** library.</span></span>
* <span data-ttu-id="379f1-124">Installation von [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod.</span><span class="sxs-lookup"><span data-stu-id="379f1-124">Installation of the [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod.</span></span> 
* <span data-ttu-id="379f1-125">Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="379f1-125">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span></span>

## <a name="register-the-app"></a><span data-ttu-id="379f1-126">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="379f1-126">Register the app</span></span>
 
1. <span data-ttu-id="379f1-127">Melden Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="379f1-127">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="379f1-128">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="379f1-128">Select **Add an app**.</span></span>
3. <span data-ttu-id="379f1-129">Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="379f1-129">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="379f1-130">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="379f1-130">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="379f1-131">Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="379f1-131">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="379f1-132">Wählen Sie **Systemeigene Plattform**.</span><span class="sxs-lookup"><span data-stu-id="379f1-132">Select **Native platform**.</span></span>
6. <span data-ttu-id="379f1-p105">Kopieren Sie die Client-ID in die Zwischenablage. Sie müssen diesen Wert in die Beispiel-App eingeben.</span><span class="sxs-lookup"><span data-stu-id="379f1-p105">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="379f1-135">Die App-ID ist ein eindeutiger Bezeichner für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="379f1-135">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="379f1-136">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="379f1-136">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="379f1-137">Importieren der Projekt-Abhängigkeiten</span><span class="sxs-lookup"><span data-stu-id="379f1-137">Importing the project dependencies</span></span>

1. <span data-ttu-id="379f1-138">Klonen Sie dieses Repository: [Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="379f1-138">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span></span> 


2. <span data-ttu-id="379f1-139">Verwenden Sie CocoaPods, um die PromiseKit-Abhängigkeiten zu importieren.</span><span class="sxs-lookup"><span data-stu-id="379f1-139">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies:</span></span> <span data-ttu-id="379f1-140">Diese Beispiel-App enthält bereits eine POD-Datei, die die Pods in das Projekt überträgt.</span><span class="sxs-lookup"><span data-stu-id="379f1-140">This sample app already contains a podfile that will get the pods into the project.</span></span> <span data-ttu-id="379f1-141">Navigieren Sie zum Stammordner des Projekts in der **Terminal**-App, und führen Sie über **Terminal** Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="379f1-141">Navigate to the root folder of the project in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="379f1-p107">Sie erhalten eine Bestätigung, dass die Pods in das Projekt importiert wurden. Weitere Informationen finden Sie unter [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span><span class="sxs-lookup"><span data-stu-id="379f1-p107">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>

## <a name="install-the-msal-authentication-framework"></a><span data-ttu-id="379f1-144">Installieren des MSAL-Authentifizierungsframeworks</span><span class="sxs-lookup"><span data-stu-id="379f1-144">Install the MSAL authentication framework</span></span>

<span data-ttu-id="379f1-145">Die Vorschauversion von MSAL wird als Header- und Symboldateien über Carthage verteilt.</span><span class="sxs-lookup"><span data-stu-id="379f1-145">The preview version of MSAL is distributed as header and symbol files using Carthage.</span></span> <span data-ttu-id="379f1-146">Gehen Sie wie folgt vor, um MSAL im Projekt zu installieren:</span><span class="sxs-lookup"><span data-stu-id="379f1-146">To install MSAL in the project, do these steps:</span></span>

1. <span data-ttu-id="379f1-147">Öffnen Sie das Bash-Terminal, und gehen Sie zum App-Stammordner.</span><span class="sxs-lookup"><span data-stu-id="379f1-147">Open the Bash terminal and go to the app root folder.</span></span>
2. <span data-ttu-id="379f1-148">Erstellen Sie eine **cartfile**: Kopieren Sie `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` in das Terminal, und führen Sie den Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="379f1-148">Create a **cartfile**: Copy `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile`  into the terminal and run the command.</span></span>
3. <span data-ttu-id="379f1-149">Erstellen Sie eine MSAL-Bibliothek: Kopieren Sie `carthage update` in das Terminal, und führen Sie den Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="379f1-149">Build the MSAL library: Copy `carthage update` into the terminal and run the command.</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="379f1-150">Aktivieren der Schlüsselbundfreigabe</span><span class="sxs-lookup"><span data-stu-id="379f1-150">Enable keychain sharing</span></span>
 
<span data-ttu-id="379f1-p109">Für Xcode 8 müssen Sie die Schlüsselbundgruppe hinzufügen, sonst kann Ihre App nicht auf den Schlüsselbund zugreifen. So fügen Sie die Schlüsselbundgruppe hinzu:</span><span class="sxs-lookup"><span data-stu-id="379f1-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="379f1-153">Wählen Sie das Projekt im Projekt-Manager-Bereich in Xcode aus.</span><span class="sxs-lookup"><span data-stu-id="379f1-153">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span> <span data-ttu-id="379f1-154">(⌘ + 1).</span><span class="sxs-lookup"><span data-stu-id="379f1-154">(⌘ + 1).</span></span>
 
2. <span data-ttu-id="379f1-155">Wählen Sie das Ziel **O365-iOS-Microsoft-Graph-Connect-swift** aus.</span><span class="sxs-lookup"><span data-stu-id="379f1-155">Select the **O365-iOS-Microsoft-Graph-Connect-swift** target.</span></span>

3. <span data-ttu-id="379f1-156">Stellen Sie sicher, dass auf der Registerkarte **Allgemein** und im Abschnitt **Signatur** die Option für die **automatische Verwaltung von Signaturen** aktiviert ist und Sie über ein gültiges Signaturzertifikat verfügen.</span><span class="sxs-lookup"><span data-stu-id="379f1-156">On the **General** tab and **Signing** section, verify that **Automatically manage signing** is checked and you have a valid signing certificate.</span></span>
 
3. <span data-ttu-id="379f1-157">Aktivieren Sie auf der Registerkarte **Funktionen** die Option **Schlüsselbundfreigabe**.</span><span class="sxs-lookup"><span data-stu-id="379f1-157">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="379f1-158">Wenn sich **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** nicht in der Liste der Schlüsselbundgruppen befindet, fügen Sie es hinzu.</span><span class="sxs-lookup"><span data-stu-id="379f1-158">If **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** is not in the list of Keychain Groups, add it.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="379f1-159">Authentifizieren mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="379f1-159">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="379f1-160">Der Workflow für die Benutzeroberfläche sieht wie folgt aus: Die App fordert den Benutzer zur Authentifizierung auf.</span><span class="sxs-lookup"><span data-stu-id="379f1-160">The UI workflow is as follows: The app asks the user to authenticate.</span></span> <span data-ttu-id="379f1-161">Nach der Authentifizierung kann der Benutzer eine E-Mail an einen anderen Benutzer senden.</span><span class="sxs-lookup"><span data-stu-id="379f1-161">After authentication, the user can send a mail to another user.</span></span> <span data-ttu-id="379f1-162">Um Abfragen in Microsoft Graph durchzuführen, verwendet das Beispiel die **MSAL**-Authentifizierungsbibliothek für HTTPS-Authentifizierungsanforderungen mit einem entsprechenden OAuth 2.0-Bearertoken.</span><span class="sxs-lookup"><span data-stu-id="379f1-162">To make requests against Microsoft Graph, the sample uses the **MSAL** authentication library to authenticate HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="379f1-163">Im Beispielprojekt importiert die **AuthenticationClass.swift.**</span><span class="sxs-lookup"><span data-stu-id="379f1-163">In the sample project the **AuthenticationClass.swift.**</span></span> <span data-ttu-id="379f1-164">die **MSAL**-Bibliothek und erwirbt das Zugriffstoken, das für Microsoft Graph-REST-Operationen erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="379f1-164">class imports the **MSAL** library and acquires the access token needed for Microsoft Graph REST operations.</span></span>

1. <span data-ttu-id="379f1-165">Öffnen Sie den **Xcode**-Projektarbeitsbereich (**Graph-iOS-Swift-Connect.xcworkspace**), und öffnen Sie die Klassendatei **AuthenticationClas.swift**. Suchen Sie den folgenden Code in dieser Klasse.</span><span class="sxs-lookup"><span data-stu-id="379f1-165">Open the Xcode project workspace (Graph-iOS-Swift-Connect.xcworkspace), and open the structure extension file Authentication.swift Find the following code in that extension.</span></span>


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


2. <span data-ttu-id="379f1-166">Wir rufen die **connectToGraph**-Funktion von **ConnectViewController.swift** auf.</span><span class="sxs-lookup"><span data-stu-id="379f1-166">We'll call the **connectToGraph** function from **ConnectViewController.swift**.</span></span> <span data-ttu-id="379f1-167">Dieser Controller ist die Standardansicht, die die App mit einer einzelnen Schaltfläche mit dem Namen **Verbinden** lädt. Der Benutzer tippt darauf, um den Authentifizierungsprozess zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="379f1-167">This controller is the default view that the app loads with a single button named **Connect** that the user taps to start authenticating.</span></span> 

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

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="379f1-168">Senden einer E-Mail mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="379f1-168">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="379f1-169">Nachdem der Benutzer mit Microsoft Graph verbunden wurde, ruft das Beispiel die E-Mail-Adresse, den Anzeigenamen und das Profilfoto des authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="379f1-169">After connecting the user to Microsoft Graph, the sample gets the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="379f1-170">Das Beispiel lädt das Profilfoto in den OneDrive-Stammordner des Benutzers hoch und fragt OneDrive nach der Freigabe-URL des Bilds.</span><span class="sxs-lookup"><span data-stu-id="379f1-170">The sample uploads the profile photo to the user's OneDrive root folder and asks OneDrive for the sharing Url of the picture.</span></span> <span data-ttu-id="379f1-171">Zum Schluss sendet das Beispiel eine REST-Anforderung an Microsoft Graph zum Senden einer E-Mail-Nachricht an die angegebene E-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="379f1-171">Finally, the sample posts a REST request to Microsoft Graph to send a mail message to the provided email address.</span></span> 

<span data-ttu-id="379f1-172">Der Nachrichtentext enthält den Freigabelink für das Bild sowie das Bild selbst als angefügte Bilddatei.</span><span class="sxs-lookup"><span data-stu-id="379f1-172">The message body contains the picture sharing link and the picture itself as an attached image file.</span></span> <span data-ttu-id="379f1-173">Der Standardempfänger ist der authentifizierte Benutzer, wobei das Beispiel dem Benutzer jedoch auch ermöglicht, die E-Mail-Adresse eines anderen Benutzers anzugeben.</span><span class="sxs-lookup"><span data-stu-id="379f1-173">The default recipient is the authenticated user, but the sample allows the user to provide the email address of any other user.</span></span> 

<span data-ttu-id="379f1-174">Der Code, den wir hier verwenden, befindet sich in der Klasse **SendMailViewController_WithPromise.swift.**</span><span class="sxs-lookup"><span data-stu-id="379f1-174">The code we'll work with here is in the class **SendMailViewController.swift.**</span></span> <span data-ttu-id="379f1-175">Die `viewDidLoad()`-Funktion liest den `self.emailTextField.text`-Wert, um die E-Mail-Adresse des Empfängers abzurufen, und beginnt dann eine **Zusagenkette**, um das Profilbild des authentifizierten Benutzers abzurufen.</span><span class="sxs-lookup"><span data-stu-id="379f1-175">The `viewDidLoad()` function reads the `self.emailTextField.text` value to get the mail recipient's email address and then starts a **promise chain** to get the authenticated user's profile picture.</span></span> <span data-ttu-id="379f1-176">Wenn die Zusage abgelehnt wird, wird `sendMailButton` nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="379f1-176">If the promise is rejected, the `sendMailButton` is not enabled.</span></span>

1. <span data-ttu-id="379f1-177">Öffnen Sie **SendMailViewController_WithPromise.swift.**,</span><span class="sxs-lookup"><span data-stu-id="379f1-177">Open **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="379f1-178">und suchen Sie die Funktion `viewDidLoad`.</span><span class="sxs-lookup"><span data-stu-id="379f1-178">and find the `viewDidLoad` function.</span></span> <span data-ttu-id="379f1-179">Die Funktion `self.userPictureWork` wird aufgerufen, um die Zusagenkette zu starten.</span><span class="sxs-lookup"><span data-stu-id="379f1-179">The `self.userPictureWork` function is called to start the promise chain.</span></span>

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

   

1. <span data-ttu-id="379f1-180">Suchen Sie die Hilfsfunktion für Mailanforderungserstellungen in der Klasse:</span><span class="sxs-lookup"><span data-stu-id="379f1-180">Find the mail request creation helper function in the class:</span></span>

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
2. <span data-ttu-id="379f1-181">Suchen Sie die folgenden Hilfsfunktionen zum Abrufen des Benutzerprofilbilds, zum Hochladen des Fotos in OneDrive und zum Anfordern eines Freigabelinks für das Bild:</span><span class="sxs-lookup"><span data-stu-id="379f1-181">Find the following helper functions for getting the user's profile picture,  uploading the photograph to OneDrive, and requesting a sharing link for the picture:</span></span>

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

3. <span data-ttu-id="379f1-182">Suchen Sie die folgende Methode zum Senden von E-Mail in der Klasse.</span><span class="sxs-lookup"><span data-stu-id="379f1-182">Find the following send mail method in the class.</span></span>  
 
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


## <a name="run-the-app"></a><span data-ttu-id="379f1-183">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="379f1-183">Run the app</span></span>
1. <span data-ttu-id="379f1-184">Vor dem Ausführen des Beispiels müssen Sie die Client-ID angeben, die Sie bei dem Registrierungsvorgang im Abschnitt **Registrieren der App** erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="379f1-184">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="379f1-185">Öffnen Sie **Info.plist** als Quellcode.</span><span class="sxs-lookup"><span data-stu-id="379f1-185">Open **Info.plist** as source code.</span></span> 

   - <span data-ttu-id="379f1-186">Ersetzen Sie `ENTER_CLIENT_ID_HERE` durch die **ClientID** aus dem Registrierungsprozess.</span><span class="sxs-lookup"><span data-stu-id="379f1-186">Replace  `ENTER_CLIENT_ID_HERE` with the **ClientID** from the registration process.</span></span> <span data-ttu-id="379f1-187">Stellen Sie sicher, dass `msal` nicht ersetzt wird.</span><span class="sxs-lookup"><span data-stu-id="379f1-187">Be sure that `msal` is not replaced.</span></span> <span data-ttu-id="379f1-188">Nachdem Sie die Zeichenfolge ersetzt haben, sieht der Array-Zeichenfolgenwert so aus: `msal48d31887-5fad-4d73-a9f5-3c356e68a038`. Hierbei ist der GUID-Teil **Ihre** Client-ID:</span><span class="sxs-lookup"><span data-stu-id="379f1-188">After you replace the string, the array string value looks like `msal48d31887-5fad-4d73-a9f5-3c356e68a038` where the GUID portion is **your** client Id:</span></span>  

   <span data-ttu-id="379f1-189">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="379f1-189">For example,</span></span> 

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

     <span data-ttu-id="379f1-190">wird zu...</span><span class="sxs-lookup"><span data-stu-id="379f1-190">becomes...</span></span> 

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

> <span data-ttu-id="379f1-191">**Hinweis:** Sie stellen fest, dass dei folgenden Berechtigungsumfänge für dieses Projekt konfiguriert wurden: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` .</span><span class="sxs-lookup"><span data-stu-id="379f1-191">Note: You'll notice that the following permission scopes have been configured for this project: "https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"`["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]`.</span></span> <span data-ttu-id="379f1-192">Die in diesem Projekt verwendeten Dienstaufrufe, also das Senden einer E-Mail an Ihr E-Mail-Konto und das Abrufen einiger Profilinformationen (Anzeigename, E-Mail-Adresse) sowie das Schreiben in das OneDrive-Stammverzeichnis des Benutzers erfordern diese Berechtigungen, damit die App ohne Berechtigungsfehler ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="379f1-192">The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="379f1-193">Führen Sie das Beispiel aus, tippen Sie auf **Verbinden**, melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an und gewähren Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="379f1-193">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="379f1-p120">Klicken Sie auf die Schaltfläche **E-Mail senden**.
 Nachdem die E-Mail gesendet wurde, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="379f1-p120">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="379f1-196">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="379f1-196">Next steps</span></span>
- <span data-ttu-id="379f1-197">Testen Sie die REST-API mithilfe des [Graph-Testers](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="379f1-197">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="379f1-198">Beispiele allgemeiner Vorgänge für SDK-Operationen finden Sie in dem Beispiel [Microsoft Graph iOS Objective C Snippets](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="379f1-198">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="379f1-199">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="379f1-199">See also</span></span>
- [<span data-ttu-id="379f1-200">Azure AD v2.0-Protokolle</span><span class="sxs-lookup"><span data-stu-id="379f1-200">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="379f1-201">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="379f1-201">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-tokens/)
