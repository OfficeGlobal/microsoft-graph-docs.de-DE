# <a name="get-started-with-microsoft-graph-in-an-objectve-c-ios-app"></a><span data-ttu-id="5fc66-101">Erste Schritte mit Microsoft Graph in einer Ziel-C-iOS-App</span><span class="sxs-lookup"><span data-stu-id="5fc66-101">Get started with Microsoft Graph in an Objectve C iOS App</span></span>

> <span data-ttu-id="5fc66-p101">**Sie erstellen Apps für Unternehmenskunden?** Ihre App funktioniert möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfunktionen wie <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">bedingten Gerätezugriff</a> aktiviert. In diesem Fall treten bei Ihren Kunden möglicherweise Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="5fc66-p102">Zur Unterstützung **aller Unternehmenskunden** über **alle Unternehmensszenarien** hinweg müssen Sie den Azure AD-Endpunkt verwenden und Ihr Apps mithilfe des [Azure-Portals](https://aka.ms/aadapplist) verwalten. Weitere Informationen finden Sie unter [Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="5fc66-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="5fc66-p103">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom [Azure AD v2.0-Endpunkt](https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth) und zum Aufrufen von Microsoft Graph. Er führt Sie durch den Code im [Office 365 Connect-Beispiel für iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) und erläutert die wichtigsten Konzepte, die in einer App implementiert werden müssen, die Microsoft Graph verwendet. In diesem Artikel wird auch beschrieben, wie Sie mithilfe des [Microsoft Graph SDK für iOS](https://github.com/microsoftgraph/msgraph-sdk-ios) auf Microsoft Graph zugreifen.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="5fc66-110">Sie können die Version der App, die Sie erstellen, aus diesem GitHub Repository herunterladen:</span><span class="sxs-lookup"><span data-stu-id="5fc66-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="5fc66-111">Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs</span><span class="sxs-lookup"><span data-stu-id="5fc66-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="5fc66-112">In der folgenden Abbildung ist die App dargestellt, die Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="5fc66-112">The following image shows the app you'll create.</span></span>

![Die exemplarische Vorgehensweise im Connect-Beispiel zeigt die Herstellung einer Verbindung und das Senden einer E-Mail in der App.](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="5fc66-114">Der Workflow beinhaltet das Herstellen einer Verbindung zu Microsoft Graph sowie die Authentifizierung, das Anmelden mit Ihrem Büro- oder persönlichen Konto und schließlich das Senden einer E-Mail an einen Empfänger.</span><span class="sxs-lookup"><span data-stu-id="5fc66-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="5fc66-p104">**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Schnellstart Microsoft Graph](https://graph.microsoft.io/de-DE/getting-started).</span><span class="sxs-lookup"><span data-stu-id="5fc66-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/de-DE/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fc66-117">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5fc66-117">Prerequisites</span></span>

<span data-ttu-id="5fc66-118">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="5fc66-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="5fc66-119">[Xcode](https://developer.apple.com/xcode/downloads/) von Apple</span><span class="sxs-lookup"><span data-stu-id="5fc66-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="5fc66-120">Installation von [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) als ein Abhängigkeits-Manager.</span><span class="sxs-lookup"><span data-stu-id="5fc66-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="5fc66-121">Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="5fc66-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="5fc66-122">Das [Microsoft Graph Startprojekt für iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="5fc66-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="5fc66-123">Diese Vorlage enthält Klassen, denen Sie Code hinzufügen müssen.</span><span class="sxs-lookup"><span data-stu-id="5fc66-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="5fc66-124">Sie rufen dieses Projekt ab, indem Sie das Beispielprojekt von diesem Speicherort aus klonen oder herunterladen. Dann arbeiten Sie mit dem Arbeitsbereich innerhalb des Ordners **Startprojekt** (**ios-objectivec-connect-sample.xcworkspace**).</span><span class="sxs-lookup"><span data-stu-id="5fc66-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="5fc66-125">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="5fc66-125">Register the app</span></span>
 
1. <span data-ttu-id="5fc66-126">Melden Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="5fc66-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="5fc66-127">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="5fc66-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="5fc66-128">Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="5fc66-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="5fc66-129">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="5fc66-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="5fc66-130">Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="5fc66-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="5fc66-131">Wählen Sie **Systemeigene Plattform**.</span><span class="sxs-lookup"><span data-stu-id="5fc66-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="5fc66-p106">Kopieren Sie die Client-ID in die Zwischenablage. Sie müssen diesen Wert in die Beispiel-App eingeben.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="5fc66-134">Die App-ID ist ein eindeutiger Bezeichner für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="5fc66-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="5fc66-135">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="5fc66-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="5fc66-136">Importieren der Projekt-Abhängigkeiten</span><span class="sxs-lookup"><span data-stu-id="5fc66-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="5fc66-137">Klonen Sie dieses Repository, [Office 365 Connect-Beispiel für iOS unter Verwendung des Microsoft Graph-SDKs](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="5fc66-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="5fc66-138">WICHTIG: Verwenden Sie das Beispiel im Startprojekt-Ordner und nicht im Beispiel auf der Stammebene des Projekts.</span><span class="sxs-lookup"><span data-stu-id="5fc66-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="5fc66-p107">Verwenden Sie CocoaPods, um das Microsoft Graph-SDK und Authentifizierungsabhängigkeiten zu importieren: Diese Beispiel-App enthält bereits eine POD-Datei, die die Pods in das Projekt überträgt. Navigieren Sie zu dem Ordner **Startprojekt** in der **Terminal** -App und führen Sie von **Terminal** folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="5fc66-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="5fc66-p108">Sie erhalten eine Bestätigung, dass die Pods in das Projekt importiert wurden. Weitere Informationen finden Sie unter [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span><span class="sxs-lookup"><span data-stu-id="5fc66-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="5fc66-144">Aktivieren der Schlüsselbundfreigabe</span><span class="sxs-lookup"><span data-stu-id="5fc66-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="5fc66-p109">Für Xcode 8 müssen Sie die Schlüsselbundgruppe hinzufügen, sonst kann Ihre App nicht auf den Schlüsselbund zugreifen. So fügen Sie die Schlüsselbundgruppe hinzu:</span><span class="sxs-lookup"><span data-stu-id="5fc66-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="5fc66-p110">Wählen Sie im Projekt-Manager-Bereich in Xcode das Projekt aus. (⌘ + 1).</span><span class="sxs-lookup"><span data-stu-id="5fc66-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="5fc66-149">Wählen Sie **iOS-ObjectiveC-Connect-Sample**.</span><span class="sxs-lookup"><span data-stu-id="5fc66-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="5fc66-150">Aktivieren Sie auf der Registerkarte „Funktionen“ die Option **Schlüsselbundfreigabe**.</span><span class="sxs-lookup"><span data-stu-id="5fc66-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="5fc66-151">Fügen Sie **com.microsoft.ios-objectivec-connect-sample** zu den Schlüsselbundgruppen hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>
 

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="5fc66-152">Authentifizieren mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5fc66-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="5fc66-p111">Für den Zugriff auf den Benutzeroberflächenworkflow muss die App den Benutzer authentifizieren, sodass dieser dann eine E-Mail an einen bestimmten Benutzer senden kann. Für Anforderungen beim Microsoft Graph-Dienst muss ein Authentifizierungsanbieter bereitgestellt werden, der HTTPS-Anforderungen mit einem entsprechenden OAuth 2.0-Bearertoken authentifizieren kann. Im Beispielprojekt liegt eine Authentifizierungsklasse mit der Bezeichnung **AuthenticationProvider.m.** bereits als Stub vor. Wir fügen eine Funktion zum Anfordern und Erwerben eines Zugriffstokens für den Aufruf der Microsoft Graph-API hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p111">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user. To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token. In the sample project there's an authentication class already stubbed out called **AuthenticationProvider.m.** We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="5fc66-157">Öffnen Sie den Projektarbeitsbereich Xcode (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) im Ordner **Startprojekt** und navigieren Sie zum Ordner **Authentifizierung** und öffnen Sie die Datei **AuthenticationProvider.m.**</span><span class="sxs-lookup"><span data-stu-id="5fc66-157">Open the Xcode project workspace (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) in the **starter-project** folder, and navigate to the **Authentication** folder and open the file **AuthenticationProvider.m.**</span></span> <span data-ttu-id="5fc66-158">Fügen Sie dieser Klasse den folgenden Code hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-158">Add the following code to that class.</span></span>

```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)    (NSError *))completion{
      [NXOAuth2AuthenticationProvider setClientId:kClientId scopes:scopes];
      /**
      Obtains access token by performing login with UI, where viewController specifies the parent view controller.
      @param viewController The view controller to present the UI on.
      @param completionHandler The completion handler to be called when the authentication has completed.
      error should be non nil if there was no error, and should contain any error(s) that occurred.
      */

      if ([[NXOAuth2AuthenticationProvider sharedAuthProvider] loginSilent]) {
         completion(nil);
      }
      else {
         [[NXOAuth2AuthenticationProvider sharedAuthProvider] loginWithViewController:nil completion:^(NSError *error) {
            if (!error) {
               NSLog(@"Authentication successful.");
               completion(nil);
            }
            else {
               NSLog(@"Authentication failed - %@", error.localizedDescription);
               completion(error);
            }
         }];
      }
   }
```     

2. <span data-ttu-id="5fc66-p113">Als Nächstes fügen Sie die Methode in der Header-Datei hinzu. Öffnen Sie die Datei **AuthenticationProvider.h** und fügen Sie dieser Klasse den folgenden Code hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p113">Next add the method to the header file. Open the file **AuthenticationProvider.h** and add the following code to this class.</span></span>
   ```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId
                               scopes:(NSArray *)scopes
                           completion:(void (^)(NSError *error))completion;
   ```

2. <span data-ttu-id="5fc66-p114">Abschließend rufen wir diese Methode aus **ConnectViewController.m**  heraus auf. Dieser Controller ist die Standardansicht, die die App lädt, und es gibt eine einzelne Schaltfläche mit dem Namen **Verbinden**, die der Benutzer antippt, um den Authentifizierungsprozess zu initiieren. Diese Methode beinhaltet zwei Parameter, die **Client-ID** und **Bereiche**, die wir nachfolgend im Detail besprechen. Fügen Sie die folgende Aktion zu **ConnectViewController.m** hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p114">Finally we'll call this method from **ConnectViewController.m**. This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process. This method takes in two parameters, the **Client ID** and **scopes**, we'll discuss these in more detail below. Add the following action to **ConnectViewController.m**.</span></span>

```objectivec
- (IBAction)connectTapped:(id)sender {
   [self showLoadingUI:YES];
   NSArray *scopes = [kScopes componentsSeparatedByString:@","];
   [self.authProvider connectToGraphWithClientId:kClientId scopes:scopes completion:^(NSError *error) {
   if (!error) {
      [self performSegueWithIdentifier:@"showSendMail" sender:nil];
      [self showLoadingUI:NO];
      NSLog(@"Authentication successful.");
   }
   else{
      NSLog(NSLocalizedString(@"CHECK_LOG_ERROR", error.localizedDescription));
      [self showLoadingUI:NO];
   };
  }];
}
```     

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="5fc66-165">Senden einer E-Mail mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5fc66-165">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="5fc66-p115">Nach dem Konfigurieren des Projekts für die Authentifizierung wird in den nächsten Aufgaben mithilfe der Microsoft Graph-API eine E-Mail an einen Benutzer gesendet. Standardmäßig ist der angemeldete Benutzer der Empfänger, aber Sie haben die Möglichkeit, einen beliebigen anderen Empfänger anzugeben. Der Code, mit dem wir hier arbeiten, befindet sich im Ordner **Controller** und in der Klasse **SendMailViewController.m.** Sie werden sehen, dass es hier noch anderen Code für die Benutzeroberfläche und eine Hilfsmethode zum Abrufen von Benutzerprofildaten aus dem Microsoft Graph-Dienst gibt. Wir werden uns auf die Methoden zum Erstellen einer E-Mail-Nachricht und das Senden dieser Nachricht konzentrieren.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p115">After configuring the project to be able to authenticate, the next tasks are sending a mail to a user using the Microsoft Graph API. By default the logged in user will be the recipient, but you have the ability to change it to any other recipient. The code we'll work with here is located in the **Controllers** folder and in the class **SendMailViewController.m.** You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service. We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="5fc66-171">Öffnen Sie **SendMailViewController.m.** im Ordner „Controller“ und fügen Sie den folgenden Code  **viewDidLoad** nach `self.graphClient = [MSGraphClient client]` zu der Methode hinzu:</span><span class="sxs-lookup"><span data-stu-id="5fc66-171">Open **SendMailViewController.m** in the Controllers folder and add the following code to the **viewDidLoad** method, after `self.graphClient = [MSGraphClient client]`</span></span>
   ```objectivec
       [self getUserInfo:(self.emailAddress) completion:^( NSError *error) {
        if (!error) {
            [self getUserPicture:(self.emailAddress)  completion:^(UIImage *image, NSError *error) {
                if (!error) {
                    self.userPicture = image;
                } else {
                    //get the test image out of the project resources
                    self.userPicture = [UIImage imageNamed:(@"test.png")];
                }
                [self uploadPictureToOneDrive:(self.userPicture) completion:^(NSString *webUrl, NSError *error) {
                    if (!error) {
                        self.pictureWebUrl = webUrl;
                        dispatch_async(dispatch_get_main_queue(), ^{
                            self.sendMailButton.enabled = true;
                        });
                    } else {
                        dispatch_async(dispatch_get_main_queue(), ^{
                            NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                            self.statusTextView.text = NSLocalizedString(@"PICTURE_UPLOAD_FAILURE", comment: "");
                        });
                    }
                }];
            }];
        }
    }];
   ```

1. <span data-ttu-id="5fc66-172">Öffnen Sie **SendMailViewController.m.**</span><span class="sxs-lookup"><span data-stu-id="5fc66-172">Open **SendMailViewController.m.**</span></span> <span data-ttu-id="5fc66-173">im Ordner „Controller“ und fügen Sie die folgende Hilfsmethode zu der Klasse hinzu:</span><span class="sxs-lookup"><span data-stu-id="5fc66-173">in the Controllers folder and add the following helper method to the class</span></span>
```objectivec
  //Create a sample test message to send to specified user account
  -(MSGraphMessage*) getSampleMessage{
      MSGraphMessage *message = [[MSGraphMessage alloc]init];
      MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
      MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
      //need to get email text field for send to!
    
      email.address = self.emailAddress;
      toRecipient.emailAddress = email;
    
      NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
      [toRecipients addObject:toRecipient];
    
      message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
      MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
      NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
      NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
      emailBody.content = htmlContentString;
      NSString *replaceString = @"a href=";
      replaceString = [replaceString stringByAppendingString:(self.pictureWebUrl)];
      emailBody.content = [emailBody.content stringByReplacingOccurrencesOfString:(@"a href=%s") withString:(replaceString)];
      emailBody.contentType = [MSGraphBodyType html];
      message.body = emailBody;
    
      message.toRecipients = toRecipients;
    
      MSGraphFileAttachment *fileAttachment= [[MSGraphFileAttachment alloc]init];
      fileAttachment.oDataType = @"#microsoft.graph.fileAttachment";
      fileAttachment.contentType = @"image/png";
    
      NSString *decodedString = [UIImagePNGRepresentation(self.userPicture) base64EncodedStringWithOptions:NSDataBase64EncodingEndLineWithCarriageReturn];
    
      fileAttachment.contentBytes = decodedString;
      fileAttachment.name = @"me.png";
      message.attachments = [message.attachments arrayByAddingObject:(fileAttachment)];
      return message;
    
    }
```
3. <span data-ttu-id="5fc66-174">Öffnen Sie **SendMailViewController.m.** Fügen Sie die folgende Methode zu der Klasse hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-174">Open **SendMailViewController.m** Add the following method to the class.</span></span>
<span data-ttu-id="5fc66-175">Mit **UploadPictureToOneDrive** wird das Profilbild des [Benutzers](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user) aus den [Benutzerinformationen](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user) hochgeladen. Die URL für die Webfreigabe wird in den Textkörper der E-Mail eingebettet, die vom Beispiel zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="5fc66-175">**uploadPictureToOneDrive** uploads the [user](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user)'s profile picture from their [user](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user) information and returns the web sharing Url to be embedded in the body of the email that is sent by the sample.</span></span>

  ```objectivec
  -(void) uploadPictureToOneDrive: (UIImage *) image completion:(void(^) (NSString*, NSError*))completionBlock{
    
    NSData *data = UIImagePNGRepresentation(image);
    [[[[[[[self.graphClient me]
          drive]
         root]
        children]
       driveItem:(@"me.png")]
      contentRequest]
     uploadFromData:(data) completion:^(MSGraphDriveItem *response, NSError *error) {
         
         if (!error) {
             NSString *webUrl = response.webUrl;
             completionBlock(webUrl, error);
         } else {
             dispatch_async(dispatch_get_main_queue(), ^{
                 self.statusTextView.text =  NSLocalizedString(@"USER_GET_PICTURE_FAILURE", comment: "");
                 NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
             });
         }
     }];
    }
  ```
4. <span data-ttu-id="5fc66-176">Öffnen Sie **SendMailViewController.m.** und fügen Sie die folgende Methode zu der Klasse hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-176">Open **SendMailViewController.m** and add the following method to the class.</span></span> 
<span data-ttu-id="5fc66-177">**getUserPicture** gibt das Profilbild des [Benutzers](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user) zurück, falls dieses verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="5fc66-177">**getUserPicture** returns the [user](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user)'s profile picture if it is available.</span></span>
   ```objectivec
   -(void) getUserPicture: (NSString *)url completion:(void(^) (UIImage*, NSError*))completionBlock {
    
    [[[self.graphClient me] photoValue] downloadWithCompletion:^(NSURL *location, NSURLResponse *response, NSError *error) {
        //code
        if (!error) {
            NSData *data = [NSData dataWithContentsOfURL:location];
            UIImage *img = [[UIImage alloc] initWithData:data];
            completionBlock(img, error);
        } else{
            completionBlock(nil, error);

        }
    }];
    }

   ```
3. <span data-ttu-id="5fc66-178">Öffnen Sie **SendMailViewcontroller.m.** und fügen Sie die folgende Methode zu der Klasse hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-178">Open **SendMailViewcontroller.m** and add the following method to the class.</span></span>
<span data-ttu-id="5fc66-179">Diese Methode ruft die [Benutzerressource](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user) ab, die den authentifizierten Benutzer repräsentiert, speichert die zum Abrufen des Profilbilds des Benutzers notwendigen Felder zwischen und versendet eine E-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="5fc66-179">This method gets the [user](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/user) resource representing the authenticated user and caches the fields necessary to get the user's profile picture and send an email.</span></span>
   ```objectivec
   //Retrieve the logged in user's display name and email address
   -(void) getUserInfo: (NSString *)url completion:(void(^) ( NSError*))completionBlock{
    
    [[[self.graphClient me]request]getWithCompletion:^(MSGraphUser *response, NSError *error) {
        if(!error){
            dispatch_async(dispatch_get_main_queue(), ^{
                self.emailAddress = response.userPrincipalName;
                self.emailTextField.text = self.emailAddress;
                self.headerLabel.text = [NSString stringWithFormat:(NSLocalizedString(@"HI_USER", comment "")), response.displayName];
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_SUCCESS", comment: "");
            });

            completionBlock(nil);
        }
        else{
            dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_FAILURE", comment: "");
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            });
            completionBlock(error);
        }
    }];
    
   }

   ```
3. <span data-ttu-id="5fc66-180">Öffnen Sie **SendMailViewController.m.** Fügen Sie die folgende Methode für das Senden von E-Mails zu der Klasse hinzu.</span><span class="sxs-lookup"><span data-stu-id="5fc66-180">Open **SendMailViewController.m** Add the following send mail method to the class.</span></span>
<span data-ttu-id="5fc66-181">**getSampleMessage** erstellt einen Entwurf einer HTML-Beispiel-E-Mail für Demozwecke.</span><span class="sxs-lookup"><span data-stu-id="5fc66-181">**getSampleMessage** creates a draft HTML sample mail to use for demo purposes.</span></span> <span data-ttu-id="5fc66-182">Die nächste Methode, **sendMail**, nimmt die Nachricht auf und führt die Anforderung zum Senden der Nachricht aus.</span><span class="sxs-lookup"><span data-stu-id="5fc66-182">The next method, **sendMail**, then takes that message and executes the request to send it.</span></span> <span data-ttu-id="5fc66-183">Der Standardempfänger ist auch hier der angemeldete Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5fc66-183">Again the default recipient is the signed-in user.</span></span>


  ```objectivec
   //Send mail to the specified user in the email text field
   -(void) sendMail {
    MSGraphMessage *message = [self getSampleMessage];
    MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
    NSLog(@"%@", requestBuilder);
    MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
    [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
        if(!error){
            NSLog(@"response %@", response);
             dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                self.descriptionLabel.text = @"Check your inbox. You have a new message :)";
            });
        }
        else {
            dispatch_async(dispatch_get_main_queue(), ^{
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
            });
        }
    }];
   }
   ```



## <a name="run-the-app"></a><span data-ttu-id="5fc66-184">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="5fc66-184">Run the app</span></span>
1. <span data-ttu-id="5fc66-p121">Vor dem Ausführen des Beispiels müssen Sie die Client-ID angeben, die Sie bei dem Registrierungsvorgang im Abschnitt **Registrieren der App** erhalten haben. Öffnen Sie **AuthenticationConstants.m** unter dem Ordner **Anwendung**. Sie werden sehen, dass die ClientID aus dem Registrierungsprozess am Anfang der Datei hinzugefügt werden kann:</span><span class="sxs-lookup"><span data-stu-id="5fc66-p121">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.** Open **AuthenticationConstants.m** under the **Application** folder. You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  
   ```objectivec
   // You will set your application's clientId
   NSString * const kClientId    = @"ENTER_YOUR_CLIENT_ID";
   NSString * const kScopes = @"https://graph.microsoft.com/User.Read, https://graph.microsoft.com/Mail.ReadWrite, https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/Files.ReadWrite";
   ```      

><span data-ttu-id="5fc66-p122">Hinweis: Sie sehen, dass die folgenden Berechtigungsbereiche für dieses Projekt konfiguriert wurden: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "Offline_access"**. Die in diesem Projekt verwendeten Dienstaufrufe, also das Senden einer E-Mail an Ihr E-Mail-Konto und das Abrufen einiger Profilinformationen (Anzeigename, E-Mail-Adresse), benötigen diese Berechtigungen, damit die App ordnungsgemäß ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p122">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="5fc66-190">Führen Sie das Beispiel aus, tippen Sie auf **Verbinden**, melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an und gewähren Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="5fc66-190">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="5fc66-p123">Klicken Sie auf die Schaltfläche **E-Mail senden**.
 Nachdem die E-Mail gesendet wurde, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5fc66-p123">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5fc66-193">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="5fc66-193">Next steps</span></span>
- <span data-ttu-id="5fc66-194">Testen Sie die REST-API mithilfe des [Graph-Explorers](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="5fc66-194">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="5fc66-195">Beispiele allgemeiner Vorgänge sowohl für REST- als auch für SDK-Operationen finden Sie in dem Beispiel [Microsoft Graph iOS Objective C Code Snippets](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="5fc66-195">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="5fc66-196">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5fc66-196">See also</span></span>
- [<span data-ttu-id="5fc66-197">Microsoft Graph SDK für iOS</span><span class="sxs-lookup"><span data-stu-id="5fc66-197">Microsoft Graph SDK for iOS</span></span>](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [<span data-ttu-id="5fc66-198">Protokolle für Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="5fc66-198">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="5fc66-199">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="5fc66-199">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-tokens/)
