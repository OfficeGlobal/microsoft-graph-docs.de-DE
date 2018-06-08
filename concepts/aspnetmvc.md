# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a><span data-ttu-id="8d31d-101">Erste Schritte mit Microsoft Graph in einer ASP.NET 4.6 MVC-App</span><span class="sxs-lookup"><span data-stu-id="8d31d-101">Get started with Microsoft Graph in an ASP.NET 4.6 MVC app</span></span>

<span data-ttu-id="8d31d-p101">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstoken vom Azure AD v2.0-Endpunkt und zum Aufrufen von Microsoft Graph. Sie werden durch die Erstellung des [Microsoft Graph Connect-Beispiels für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) geführt und erhalten Informationen zu den Hauptkonzepten, die Sie zur Verwendung von Microsoft Graph implementieren.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) and explains the main concepts that you implement to use Microsoft Graph.</span></span>

<span data-ttu-id="8d31d-104">In der folgenden Abbildung ist die App dargestellt, die Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="8d31d-104">The following image shows the app you'll create.</span></span> 

<span data-ttu-id="8d31d-105">![Die Web-App mit den Schaltfläche "E-Mail-Adresse abrufen" und "E-Mail senden" ](images/aspnet-connect-sample.png "Die Web-App mit den Schaltfläche 'E-Mail-Adresse abrufen' und 'E-Mail senden'")</span><span class="sxs-lookup"><span data-stu-id="8d31d-105">![The web app with "Get email address" and "Send email" buttons](images/aspnet-connect-sample.png "The web app with 'Get email address' and 'Send email' buttons")</span></span>

<span data-ttu-id="8d31d-p102">Der [Azure AD Version 2.0-Endpunkt](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-appmodel-v2-overview) ermöglicht Benutzern, sich mit einem Microsoft-Konto (MSA) oder einem Geschäfts-, Schul- oder Unikonto anzumelden. Die App verwendet die [ASP.Net OpenID Connect OWIN Middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) und die [Microsoft Authentication Library (MSAL) für .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) für die Anmeldung und die Token-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p102">The [Azure AD v2.0 endpoint](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-appmodel-v2-overview) lets users sign in with a Microsoft account (MSA) or a work or school account. The app uses the [ASP.Net OpenID Connect OWIN middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) and the [Microsoft Authentication Library (MSAL) for .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) for sign in and token management.</span></span>

<span data-ttu-id="8d31d-p103">**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Microsoft Graph-Schnellstart](https://developer.microsoft.com/de-DE/graph/quick-start). Beachten Sie auch, dass es eine [REST-Version dieses Beispiels](https://github.com/microsoftgraph/aspnet-connect-rest-sample) gibt.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p103">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/de-DE/graph/quick-start) to get up and running fast. Also note that we have a [REST version of this sample](https://github.com/microsoftgraph/aspnet-connect-rest-sample).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d31d-111">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d31d-111">Prerequisites</span></span>

<span data-ttu-id="8d31d-112">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="8d31d-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="8d31d-113">Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="8d31d-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="8d31d-114">Visual Studio 2015</span><span class="sxs-lookup"><span data-stu-id="8d31d-114">Visual Studio 2015</span></span> 
- <span data-ttu-id="8d31d-p104">[Microsoft Graph Connect-Beispiel für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). Sie verwenden den Ordner **Startprojekt** in den Beispieldateien.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p104">The [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). You'll use the **starter-project** folder in the sample files.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="8d31d-117">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="8d31d-117">Register the application</span></span>

<span data-ttu-id="8d31d-p105">In diesem Schritt registrieren Sie eine App im Microsoft App-Registrierungsportal. Dadurch werden die APP-ID und das Kennwort generiert, mit der bzw. dem Sie die App in Visual Studio konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p105">In this step, you'll register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="8d31d-120">Melden Sie sich beim [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="8d31d-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="8d31d-121">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="8d31d-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="8d31d-122">Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="8d31d-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="8d31d-123">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="8d31d-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="8d31d-p106">Kopieren Sie die Anwendungs-ID: Dies ist der eindeutige Bezeichner für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p106">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="8d31d-p107">Wählen Sie unter **Anwendungsgeheimnisse** die Option **Neues Kennwort generieren** aus. Kopieren Sie das Kennwort aus dem Dialogfeld **Neues Kennwort wurde generiert**.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p107">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="8d31d-128">Sie werden die Anwendungs-ID und das Kennwort verwenden, um die App zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="8d31d-128">You'll use the application ID and password to configure the app.</span></span> 

6. <span data-ttu-id="8d31d-129">Klicken Sie unter **Plattformen** auf **Plattform hinzufügen** > **Web**.</span><span class="sxs-lookup"><span data-stu-id="8d31d-129">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="8d31d-130">Vergewissern Sie sich, dass das Kontrollkästchen **Allow Implicit Flow** aktiviert ist, und geben Sie als Umleitungs-URI *http://localhost:55065/* ein.</span><span class="sxs-lookup"><span data-stu-id="8d31d-130">Make sure the Allow Implicit Flow check box is selected, and enter http://localhost:55065/ as the Redirect URI.</span></span> 

    <span data-ttu-id="8d31d-p108">Die Option **Impliziten Fluss zulassen** ermöglicht den OpenID Connect-Hybridfluss. Während der Authentifizierung ermöglicht dies der App, sowohl Anmeldeinformationen (das **id_token**) als auch Artefakte (in diesem Fall ein Autorisierungscode) abzurufen, den die App zum Abrufen eines Zugriffstokens verwendet.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p108">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow. During authentication, this enables the app to receive both sign-in info (the **id_token**) and artifacts (in this case, an authorization code) that the app uses to obtain an access token.</span></span>

8. <span data-ttu-id="8d31d-133">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="8d31d-133">Choose **Save**.</span></span>

### <a name="configure-the-project"></a><span data-ttu-id="8d31d-134">Konfigurieren des Projekts</span><span class="sxs-lookup"><span data-stu-id="8d31d-134">Configure the project</span></span>

1. <span data-ttu-id="8d31d-135">Öffnen Sie die Projektmappendatei für das Startprojekt in Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="8d31d-135">Open the solution file for the starter project in Visual Studio.</span></span>

2. <span data-ttu-id="8d31d-136">Öffnen Sie die Datei Web.config des Projekts.</span><span class="sxs-lookup"><span data-stu-id="8d31d-136">Open the project's Web.config file.</span></span>

3. <span data-ttu-id="8d31d-p109">Suchen Sie die App-Konfigurationsschlüssel im Element **AppSettings**. Ersetzen Sie die Platzhalterwerte ENTER_YOUR_CLIENT_ID und ENTER_YOUR_SECRET durch die Werte, die Sie soeben kopiert haben.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p109">Locate the app configuration keys in the **appSettings** element. Replace the ENTER_YOUR_CLIENT_ID and ENTER_YOUR_SECRET placeholder values with the values you just copied.</span></span>

<span data-ttu-id="8d31d-p110">Der Umleitung-URI ist die URL des Projekts, das Sie registriert haben. Die angeforderten [Berechtigungsbereiche](https://developer.microsoft.com/de-DE/graph/docs/concepts/permission_scopes) ermöglichen der App das Abrufen der Benutzerprofilinformationen und das Senden einer E-Mail.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p110">The redirect URI is the URL of the project that you registered. The requested [permission scopes](https://developer.microsoft.com/de-DE/graph/docs/concepts/permission_scopes) allow the app to get user profile information and send an email.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="8d31d-141">Aufrufen von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d31d-141">Call Microsoft Graph</span></span>

<span data-ttu-id="8d31d-142">In diesem Schritt liegt der Schwerpunkt auf den Klassen **SDKHelper**, **GraphService** und **HomeController**.</span><span class="sxs-lookup"><span data-stu-id="8d31d-142">In this step, you'll focus on the **SDKHelper**, **GraphService**, and **HomeController** classes.</span></span> 

 - <span data-ttu-id="8d31d-p111">**SDKHelper** Initialisiert eine Instanz von **GraphServiceClient** aus der Bibliothek vor jedem Aufruf von Microsoft Graph. Zu diesem Zeitpunkt wir der Zugriffstoken der Anforderung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p111">**SDKHelper** intializes an instance of the **GraphServiceClient** from the library before each call to the Microsoft Graph. This is when the access token is added to the request.</span></span> 
 - <span data-ttu-id="8d31d-145">**GraphService** erstellt und sendet mithilfe der Bibliothek Anfragen an Microsoft Graph und verarbeitet die Antworten.</span><span class="sxs-lookup"><span data-stu-id="8d31d-145">**GraphService** builds and sends requests to the Microsoft Graph using the library, and processes the responses.</span></span>
 - <span data-ttu-id="8d31d-146">**HomeController** enthält Aktionen, die Bibliotheksaufrufe als Antwort auf Benutzeroberflächenereignisse auslösen.</span><span class="sxs-lookup"><span data-stu-id="8d31d-146">**HomeController** contains actions that initiate the calls to the library in response to UI events.</span></span>

<span data-ttu-id="8d31d-147">Das Startprojekt deklariert bereits eine Abhängigkeit für das Microsoft Graph .NET Client Library NuGet-Paket:  *Microsoft.Graph*.</span><span class="sxs-lookup"><span data-stu-id="8d31d-147">The starter project already declares a dependency for the Microsoft Graph .NET Client Library NuGet package:  *Microsoft.Graph*.</span></span>

1. <span data-ttu-id="8d31d-148">Klicken Sie mit der rechten Maustaste in den Ordner **Hilfsprogramme** Ordner, und wählen Sie **Hinzufügen** > **Klasse**.</span><span class="sxs-lookup"><span data-stu-id="8d31d-148">Right-click the **Helpers** folder and choose **Add** > **Class**.</span></span> 

1. <span data-ttu-id="8d31d-149">Nennen Sie die neue Klasse *SDKHelper*, und wählen Sie **Hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="8d31d-149">Name the new class *SDKHelper* and choose **Add**.</span></span>

1. <span data-ttu-id="8d31d-150">Ersetzen Sie den Inhalt durch den folgenden Code.</span><span class="sxs-lookup"><span data-stu-id="8d31d-150">Replace the contents with the following code.</span></span>

        using System.Net.Http.Headers;
        using Microsoft.Graph;

        namespace Microsoft_Graph_SDK_ASPNET_Connect.Helpers
        {
            public class SDKHelper
            {   
                private static GraphServiceClient graphClient = null;

                // Get an authenticated Microsoft Graph Service client.
                public static GraphServiceClient GetAuthenticatedClient()
                {
                    GraphServiceClient graphClient = new GraphServiceClient(
                        new DelegateAuthenticationProvider(
                            async (requestMessage) =>
                            {
                                string accessToken = await SampleAuthProvider.Instance.GetUserAccessTokenAsync();

                                // Append the access token to the request.
                                requestMessage.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);
                            }));
                    return graphClient;
                }

                public static void SignOutClient()
                {
                    graphClient = null;
                }
            }
        }

  <span data-ttu-id="8d31d-151">Beachten Sie den Aufruf von **SampleAuthProvider**, um den Token abzurufen, wenn der Client initialisiert wird.</span><span class="sxs-lookup"><span data-stu-id="8d31d-151">Note the call to **SampleAuthProvider** to get the token when the client is initialized.</span></span>

1. <span data-ttu-id="8d31d-p112">Im Ordner **Modelle** öffnen Sie GraphService.cs. Der Dienst verwendet die Bibliothek zur Interaktion mit dem Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p112">In the **Models** folder, open GraphService.cs. The service uses the library to interact with the Microsoft Graph.</span></span>

1. <span data-ttu-id="8d31d-154">Fügen Sie die folgende **using**-Anweisung hinzu.</span><span class="sxs-lookup"><span data-stu-id="8d31d-154">Add the following **using** statement.</span></span>

        using Microsoft.Graph;

1. <span data-ttu-id="8d31d-p113">Ersetzen Sie */ / GetMyEmailAddress* durch die folgende Methode. Dadurch wird die E-Mail-Adresse des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p113">Replace *// GetMyEmailAddress* with the following method. This gets the current user's email address.</span></span> 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  <span data-ttu-id="8d31d-p114">Beachten Sie das **Select**-Segment, mit dem nur **mail** und **UserPrinicipalName** zurückgegeben werden. Sie können mit **Select** und **Filter** die Größe der Antwortdaten-Nutzlast verringern.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p114">Note the **Select** segment, which requests only the **mail** and **userPrinicipalName** to be returned. You can use **Select** and **Filter** to reduce the size of the response data payload.</span></span>

1. <span data-ttu-id="8d31d-159">Ersetzen Sie */ / SendEmail* mit den folgenden Methoden zum Erstellen und Senden der E-Mail.</span><span class="sxs-lookup"><span data-stu-id="8d31d-159">Replace *// SendEmail* with the following methods to build and send the email.</span></span>

        // Send an email message from the current user.
        public async Task SendEmail(GraphServiceClient graphClient, Message message)
        {
            await graphClient.Me.SendMail(message, true).Request().PostAsync();
        }

        public async Task<Message> BuildEmailMessage(GraphServiceClient graphClient, string recipients, string subject)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync(graphClient);


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if ( photoStream == null)
            {
                photoStream = System.IO.File.OpenRead(System.Web.Hosting.HostingEnvironment.MapPath("/Content/test.jpg"));
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDrive(graphClient, photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            Permission sharingLink = await GetSharingLinkAsync(graphClient, photoFile.Id);

            // Add the sharing link to the email body.
            string bodyContent = string.Format(Resource.Graph_SendMail_Body_Content, sharingLink.Link.WebUrl);

            // Prepare the recipient list.
            string[] splitter = { ";" };
            string[] splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();
            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient
                {
                    EmailAddress = new EmailAddress
                    {
                        Address = recipient.Trim()
                    }
                });
            }

            // Build the email message.
            Message email = new Message
            {
                Body = new ItemBody
                {
                    Content = bodyContent,
                    ContentType = BodyType.Html,
                },
                Subject = subject,
                ToRecipients = recipientList,
                Attachments = attachments
            };
            return email;
        }

        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync(GraphServiceClient graphClient)
        {
            Stream currentUserPhotoStream = null;

            try
            {
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }

        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(GraphServiceClient graphClient, string Id)
        {
            Permission permission = null;

            try
            {
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }

1. <span data-ttu-id="8d31d-160">Im Ordner **Controller** öffnen Sie HomeController.cs.</span><span class="sxs-lookup"><span data-stu-id="8d31d-160">In the **Controllers** folder, open HomeController.cs.</span></span>

1. <span data-ttu-id="8d31d-161">Fügen Sie die folgende **using**-Anweisung hinzu.</span><span class="sxs-lookup"><span data-stu-id="8d31d-161">Add the following **using** statement.</span></span>

        using Microsoft.Graph;
  
1. <span data-ttu-id="8d31d-162">Ersetzen Sie *// Controller actions* durch die folgenden Aktionen.</span><span class="sxs-lookup"><span data-stu-id="8d31d-162">Replace *// Controller actions* with the following actions.</span></span>

        [Authorize]
        // Get the current user's email address from their profile.
        public async Task<ActionResult> GetMyEmailAddress()
        {
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Get the current user's email address. 
                ViewBag.Email = await graphService.GetMyEmailAddress(graphClient);
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

        [Authorize]
        // Send mail on behalf of the current user.
        public async Task<ActionResult> SendEmail()
        {
            if (string.IsNullOrEmpty(Request.Form["email-address"]))
            {
                ViewBag.Message = Resource.Graph_SendMail_Message_GetEmailFirst;
                return View("Graph");
            }

            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Build the email message.
                Message message = await graphService.BuildEmailMessage(graphClient, Request.Form["recipients"], Request.Form["subject"]);

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Code == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

<span data-ttu-id="8d31d-163">Jetzt können Sie [die App ausführen](#run-the-app).</span><span class="sxs-lookup"><span data-stu-id="8d31d-163">Now you're ready to [run the app](#run-the-app).</span></span>

## <a name="run-the-app"></a><span data-ttu-id="8d31d-164">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="8d31d-164">Run the app</span></span>
1. <span data-ttu-id="8d31d-165">Drücken Sie zum Erstellen und Ausführen der App F5.</span><span class="sxs-lookup"><span data-stu-id="8d31d-165">Press F5 to build and run the app.</span></span> 

2. <span data-ttu-id="8d31d-166">Melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an, und gewähren Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="8d31d-166">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

3. <span data-ttu-id="8d31d-p115">Klicken Sie auf die Schaltfläche **E-Mail-Adresse abrufen**. Wenn der Vorgang abgeschlossen ist, wird die E-Mail-Adresse des angemeldeten Benutzers auf der Seite angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p115">Choose the **Get email address** button. When the operation completes, the email address of the signed-in user is displayed on the page.</span></span>

4. <span data-ttu-id="8d31d-p116">Optional können Sie die Empfängerliste und den Betreff der E-Mail bearbeiten. Klicken Sie dann auf die Schaltfläche **E-Mail senden**. Nachdem die E-Mail gesendet wurde, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8d31d-p116">Optionally edit the recipient list and email subject, and then choose the **Send email** button. When the mail is sent, a Success message is displayed below the button.</span></span>


## <a name="next-steps"></a><span data-ttu-id="8d31d-171">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="8d31d-171">Next steps</span></span>
- <span data-ttu-id="8d31d-172">Testen Sie die REST-API mithilfe des [Graph-Explorers](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="8d31d-172">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="8d31d-173">Suchen Sie nach Beispielen für allgemeine Vorgänge im [Microsoft Graph-Codeausschnittbeispiel für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample). Sie können auch unsere anderen [ASP.NET-Beispiele](http://aka.ms/aspnetgraphsamples) auf GitHub erkunden.</span><span class="sxs-lookup"><span data-stu-id="8d31d-173">Find examples of common operations in the [Microsoft Graph Snippets Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample), or explore our other [ASP.NET samples](http://aka.ms/aspnetgraphsamples) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="8d31d-174">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="8d31d-174">See also</span></span>
- [<span data-ttu-id="8d31d-175">Microsoft Graph .NET Clientbibliothek</span><span class="sxs-lookup"><span data-stu-id="8d31d-175">Microsoft Graph .NET Client Library</span></span>](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [<span data-ttu-id="8d31d-176">Webanwendung mit Web-API-Authentifizierungsszenario</span><span class="sxs-lookup"><span data-stu-id="8d31d-176">Web application to web API authentication scenario</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [<span data-ttu-id="8d31d-177">Integrieren einer Microsoft-Identität und von Microsoft Graph in eine Webanwendung mithilfe von OpenID Connect</span><span class="sxs-lookup"><span data-stu-id="8d31d-177">Integrate Microsoft identity and the Microsoft Graph into a web application using OpenID Connect</span></span>](https://azure.microsoft.com/de-DE/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [<span data-ttu-id="8d31d-178">Azure AD v2.0-Protokolle</span><span class="sxs-lookup"><span data-stu-id="8d31d-178">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="8d31d-179">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="8d31d-179">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-tokens/)
