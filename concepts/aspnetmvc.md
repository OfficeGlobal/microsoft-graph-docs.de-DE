# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a>Erste Schritte mit Microsoft Graph in einer ASP.NET 4.6 MVC-App

Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstoken vom Azure AD v2.0-Endpunkt und zum Aufrufen von Microsoft Graph. Sie werden durch die Erstellung des [Microsoft Graph Connect-Beispiels für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) geführt und erhalten Informationen zu den Hauptkonzepten, die Sie zur Verwendung von Microsoft Graph implementieren.

In der folgenden Abbildung ist die App dargestellt, die Sie erstellen. 

![Die Web-App mit den Schaltfläche "E-Mail-Adresse abrufen" und "E-Mail senden" ](images/aspnet-connect-sample.png "Die Web-App mit den Schaltfläche 'E-Mail-Adresse abrufen' und 'E-Mail senden'")

Der [Azure AD Version 2.0-Endpunkt](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview) ermöglicht Benutzern, sich mit einem Microsoft-Konto (MSA) oder einem Geschäfts-, Schul- oder Unikonto anzumelden. Die App verwendet die [ASP.Net OpenID Connect OWIN Middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) und die [Microsoft Authentication Library (MSAL) für .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) für die Anmeldung und die Token-Verwaltung.

**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Microsoft Graph-Schnellstart](https://developer.microsoft.com/en-us/graph/quick-start). Beachten Sie auch, dass es eine [REST-Version dieses Beispiels](https://github.com/microsoftgraph/aspnet-connect-rest-sample) gibt.

## <a name="prerequisites"></a>Voraussetzungen

Für die ersten Schritte benötigen Sie: 

- Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](http://dev.office.com/devprogram)
- Visual Studio 2015 
- [Microsoft Graph Connect-Beispiel für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). Sie verwenden den Ordner **Startprojekt** in den Beispieldateien.


## <a name="register-the-application"></a>Registrieren der App

In diesem Schritt registrieren Sie eine App im Microsoft App-Registrierungsportal. Dadurch werden die APP-ID und das Kennwort generiert, mit der bzw. dem Sie die App in Visual Studio konfigurieren.

1. Melden Sie sich beim [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.

2. Klicken Sie auf **App hinzufügen**.

3. Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus. 
    
    Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.

4. Kopieren Sie die Anwendungs-ID: Dies ist der eindeutige Bezeichner für Ihre App. 

5. Wählen Sie unter **Anwendungsgeheimnisse** die Option **Neues Kennwort generieren** aus. Kopieren Sie das Kennwort aus dem Dialogfeld **Neues Kennwort wurde generiert**.

    Sie werden die Anwendungs-ID und das Kennwort verwenden, um die App zu konfigurieren. 

6. Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** > ** Web** aus.

7. Stellen Sie sicher, dass das Kontrollkästchen **Impliziten Fluss zulassen** aktiviert ist, und geben Sie *http://localhost:55065/* als Umleitungs-URI ein. 

    Die Option **Impliziten Fluss zulassen** ermöglicht den OpenID Connect-Hybridfluss. Während der Authentifizierung ermöglicht dies der App, sowohl Anmeldeinformationen (das **id_token**) als auch Artefakte (in diesem Fall ein Autorisierungscode) abzurufen, den die App zum Abrufen eines Zugriffstokens verwendet.

8. Wählen Sie **Speichern** aus.

### <a name="configure-the-project"></a>Konfigurieren des Projekts

1. Öffnen Sie die Projektmappendatei für das Startprojekt in Visual Studio.

2. Öffnen Sie die Datei Web.config des Projekts.

3. Suchen Sie die App-Konfigurationsschlüssel im Element **AppSettings**. Ersetzen Sie die Platzhalterwerte ENTER_YOUR_CLIENT_ID und ENTER_YOUR_SECRET durch die Werte, die Sie soeben kopiert haben.

Der Umleitung-URI ist die URL des Projekts, das Sie registriert haben. Die angeforderten [Berechtigungsbereiche](https://developer.microsoft.com/en-us/graph/docs/concepts/permission_scopes) ermöglichen der App das Abrufen der Benutzerprofilinformationen und das Senden einer E-Mail.

## <a name="call-microsoft-graph"></a>Aufrufen von Microsoft Graph

In diesem Schritt liegt der Schwerpunkt auf den Klassen **SDKHelper**, **GraphService** und **HomeController**. 

 - **SDKHelper** Initialisiert eine Instanz von **GraphServiceClient** aus der Bibliothek vor jedem Aufruf von Microsoft Graph. Zu diesem Zeitpunkt wir der Zugriffstoken der Anforderung hinzugefügt. 
 - **GraphService** erstellt und sendet mithilfe der Bibliothek Anfragen an Microsoft Graph und verarbeitet die Antworten.
 - **HomeController** enthält Aktionen, die Bibliotheksaufrufe als Antwort auf Benutzeroberflächenereignisse auslösen.

Das Startprojekt deklariert bereits eine Abhängigkeit für das Microsoft Graph .NET Client Library NuGet-Paket:  *Microsoft.Graph*.

1. Klicken Sie mit der rechten Maustaste in den Ordner **Hilfsprogramme** Ordner, und wählen Sie **Hinzufügen** > **Klasse**. 

1. Nennen Sie die neue Klasse *SDKHelper*, und wählen Sie **Hinzufügen**.

1. Ersetzen Sie den Inhalt durch den folgenden Code.

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

  Beachten Sie den Aufruf von **SampleAuthProvider**, um den Token abzurufen, wenn der Client initialisiert wird.

1. Im Ordner **Modelle** öffnen Sie GraphService.cs. Der Dienst verwendet die Bibliothek zur Interaktion mit dem Microsoft Graph.

1. Fügen Sie die folgende **using**-Anweisung hinzu.

        using Microsoft.Graph;

1. Ersetzen Sie */ / GetMyEmailAddress* durch die folgende Methode. Dadurch wird die E-Mail-Adresse des aktuellen Benutzers abgerufen. 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  Beachten Sie das **Select**-Segment, mit dem nur **mail** und **UserPrinicipalName** zurückgegeben werden. Sie können mit **Select** und **Filter** die Größe der Antwortdaten-Nutzlast verringern.

1. Ersetzen Sie */ / SendEmail* mit den folgenden Methoden zum Erstellen und Senden der E-Mail.

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

1. Im Ordner **Controller** öffnen Sie HomeController.cs.

1. Fügen Sie die folgende **using**-Anweisung hinzu.

        using Microsoft.Graph;
  
1. Ersetzen Sie *// Controller actions* durch die folgenden Aktionen.

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

Jetzt können Sie [die App ausführen](#run-the-app).

## <a name="run-the-app"></a>Ausführen der App
1. Drücken Sie zum Erstellen und Ausführen der App F5. 

2. Melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an, und gewähren Sie die erforderlichen Berechtigungen.

3. Klicken Sie auf die Schaltfläche **E-Mail-Adresse abrufen**. Wenn der Vorgang abgeschlossen ist, wird die E-Mail-Adresse des angemeldeten Benutzers auf der Seite angezeigt.

4. Optional können Sie die Empfängerliste und den Betreff der E-Mail bearbeiten. Klicken Sie dann auf die Schaltfläche **E-Mail senden**. Nachdem die E-Mail gesendet wurde, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt.


## <a name="next-steps"></a>Nächste Schritte
- Testen Sie die REST-API mithilfe des [Graph-Explorers](https://graph.microsoft.io/graph-explorer).
- Suchen Sie nach Beispielen für allgemeine Vorgänge im [Microsoft Graph-Codeausschnittbeispiel für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample). Sie können auch unsere anderen [ASP.NET-Beispiele](http://aka.ms/aspnetgraphsamples) auf GitHub erkunden.

## <a name="see-also"></a>Siehe auch
- [Microsoft Graph .NET Clientbibliothek](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Webanwendung mit Web-API-Authentifizierungsszenario](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [Integrieren einer Microsoft-Identität und von Microsoft Graph in eine Webanwendung mithilfe von OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [Azure AD v2.0-Protokolle](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0-Tokens](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)