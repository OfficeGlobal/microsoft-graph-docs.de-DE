# <a name="get-started-with-microsoft-graph-in-a-universal-windows-10-app"></a><span data-ttu-id="749bd-101">Erste Schritte mit Microsoft Graph in einer universellen Windows 10-App</span><span class="sxs-lookup"><span data-stu-id="749bd-101">Get started with Microsoft Graph in a universal Windows 10 app</span></span>

> <span data-ttu-id="749bd-p101">**Sie erstellen Apps für Unternehmenskunden?** Ihre App funktioniert möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfunktionen wie <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">bedingten Gerätezugriff</a> aktiviert. In diesem Fall treten bei Ihren Kunden möglicherweise Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="749bd-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="749bd-p102">Zur Unterstützung **aller Unternehmenskunden** über **alle Unternehmensszenarien** hinweg müssen Sie den Azure AD-Endpunkt verwenden und Ihr Apps mithilfe des [Azure-Verwaltungsportals]((https://aka.ms/aadapplist)) verwalten. Weitere Informationen finden Sie unter [Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="749bd-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal]((https://aka.ms/aadapplist)). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="749bd-p103">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom [Azure AD v2.0-Endpunkt]((https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth)) und zum Aufrufen von Microsoft Graph. Er führt Sie schrittweise durch den Code im [Microsoft Graph Connect-Beispiel für UWP (Bibliothek)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) und erläutert die wichtigsten Konzepte, die in eine App implementiert werden müssen, die Microsoft Graph verwendet.</span><span class="sxs-lookup"><span data-stu-id="749bd-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint]((https://developer.microsoft.com/de-DE/graph/docs/concepts/converged_auth)) and call Microsoft Graph. It walks you through the code inside the [Microsoft Graph Connect Sample for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) samples to explain the main concepts that you have to implement in an app that uses Microsoft Graph.</span></span>

<span data-ttu-id="749bd-p104">**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Microsoft Graph-Schnellstart]((https://developer.microsoft.com/graph/quick-start)), oder laden Sie das [Microsoft Graph Connect-Beispiel für UWP (Bibliothek)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) herunter, auf dem dieser Artikel basiert. Beachten Sie auch, dass es eine [REST-Version dieses Beispiels]((https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample)) gibt.</span><span class="sxs-lookup"><span data-stu-id="749bd-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start]((https://developer.microsoft.com/graph/quick-start)) to get up and running fast, or download the [Microsoft Graph Connect Sample for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) that this article is based on. Also note that we have a [REST version of this sample]((https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample)).</span></span>

## <a name="sample-user-interface"></a><span data-ttu-id="749bd-112">Beispielbenutzeroberfläche</span><span class="sxs-lookup"><span data-stu-id="749bd-112">Sample user interface</span></span>

<span data-ttu-id="749bd-113">Das Beispiel enthält eine sehr einfache Benutzeroberfläche, die aus einer oberen Befehlsleiste, einer **Schaltfläche zum Herstellen einer Verbindung**, einer Schaltfläche zum **Senden von E-Mails** und aus einem Textfeld besteht, in das die E-Mail-Adresse des angemeldeten Benutzers automatisch eingetragen wird, die jedoch bearbeitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="749bd-113">The sample contains a very simple user interface, consisting of a top command bar, a **connect button**, a **send mail** button, and a text box that is automatically populated with the signed-in user's e-mail address but that can be edited.</span></span>

<span data-ttu-id="749bd-114">Die Schaltfläche zum **Senden von E-Mails** ist deaktiviert, wenn der Benutzer keine Verbindung hergestellt hat:</span><span class="sxs-lookup"><span data-stu-id="749bd-114">The **send mail** button is disabled when the user has not connected:</span></span>

![Bildschirm mit aktivierter Schaltfläche zum Verbinden und deaktivierter Schaltfläche zum Senden von E-Mails](images/SignedOut.png)

<span data-ttu-id="749bd-116">Die obere Befehlsleiste enthält eine Schaltfläche zum Trennen der Verbindung, wenn der Benutzer eine Verbindung hergestellt hat:</span><span class="sxs-lookup"><span data-stu-id="749bd-116">The top command bar contains a disconnect button when the user has connected:</span></span>

![Bildschirm mit der E-Mail-Adresse des verbundenen Benutzers und aktivierter Schaltfläche zum Senden von E-Mails](images/SignedIn.png)

<span data-ttu-id="749bd-118">Die gesamten Zeichenfolgen der Beispielbenutzeroberfläche werden in der Datei „Resources.resw“ innerhalb des Objektordners gespeichert.</span><span class="sxs-lookup"><span data-stu-id="749bd-118">All of the sample's UI strings are stored in the Resources.resw file inside the Assets folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="749bd-119">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="749bd-119">Prerequisites</span></span>

<span data-ttu-id="749bd-120">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="749bd-120">To get started, you'll need:</span></span> 

- <span data-ttu-id="749bd-121">Ein [Microsoft-Konto]((https://www.outlook.com/)) oder ein [Geschäfts-, Schul- oder Unikonto]((http://dev.office.com/devprogram))</span><span class="sxs-lookup"><span data-stu-id="749bd-121">A [Microsoft account]((https://www.outlook.com/)) or a [work or school account]((http://dev.office.com/devprogram))</span></span>
- <span data-ttu-id="749bd-122">Visual Studio 2017</span><span class="sxs-lookup"><span data-stu-id="749bd-122">Using Visual Studio 2017</span></span> 
- <span data-ttu-id="749bd-p105">Das [Microsoft Graph-Startprojekt für UWP (Bibliothek)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)/tree/master/starter). Beide Vorlagen enthalten leere Klassen, denen Sie Code hinzufügen müssen. Außerdem enthalten sie Ressourcenzeichenfolgen. Um dieses Projekt abzurufen, müssen Sie das [Microsoft Graph Connect-Beispiel für UWP (Bibliothek)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) klonen oder herunterladen und dann die Projektmappe im Ordner **starter** öffnen.</span><span class="sxs-lookup"><span data-stu-id="749bd-p105">The [Microsoft Graph Starter Project for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)/tree/master/starter). Both templates contain empty classes that you'll add code to. They also contains resource strings. To get this project, clone or download the [Microsoft Graph Connect Sample for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) and then open the solution inside the **starter** folder.</span></span>


## <a name="register-the-app"></a><span data-ttu-id="749bd-127">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="749bd-127">Register the app</span></span>
 
1. <span data-ttu-id="749bd-128">Melden Sie sich beim [App-Registrierungsportal]((https://apps.dev.microsoft.com/)) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="749bd-128">Sign into the [App Registration Portal]((https://apps.dev.microsoft.com/)) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="749bd-129">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="749bd-129">Select **Add an app**.</span></span>
3. <span data-ttu-id="749bd-130">Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="749bd-130">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="749bd-131">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="749bd-131">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="749bd-132">Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="749bd-132">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="749bd-133">Wählen Sie **Systemeigene Anwendung**.</span><span class="sxs-lookup"><span data-stu-id="749bd-133">Select **Native Application**.</span></span>
6. <span data-ttu-id="749bd-p106">Kopieren Sie die Werte für die Client-ID (App-ID) und den Umleitungs-URI in die Zwischenablage. Sie müssen diese Werte in die Beispiel-App eingeben.</span><span class="sxs-lookup"><span data-stu-id="749bd-p106">Copy both the Client Id (App Id) and Redirect URI values to the clipboard. You'll need to enter these values into the sample app.</span></span>

    <span data-ttu-id="749bd-p107">Die App-ID ist ein eindeutiger Bezeichner für Ihre App. Der Umleitungs-URI ist ein eindeutiger, von Windows 10 für jede Anwendung bereitgestellter URI, der sicherstellt, dass an diesen URI gesendete Nachrichten nur an diese Anwendung gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="749bd-p107">The app id is a unique identifier for your app. The redirect URI is a unique URI provided by Windows 10 for each application to ensure that messages sent to that URI are only sent to that application.</span></span> 

7. <span data-ttu-id="749bd-138">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="749bd-138">Select **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="749bd-139">Konfigurieren des Projekts</span><span class="sxs-lookup"><span data-stu-id="749bd-139">Configure the project</span></span>

1. <span data-ttu-id="749bd-140">Öffnen Sie die Projektmappendatei für das Startprojekt in Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="749bd-140">Open the solution file for the starter project in Visual Studio.</span></span>
2. <span data-ttu-id="749bd-p108">Öffnen Sie die Datei **App.xaml** des Projekts, und suchen Sie den Knoten `Application.Resources`. Ersetzen Sie die Platzhalter der Anwendungs-ID und des Umleitungs-URI durch die entsprechenden Werte der App, die Sie registriert haben.</span><span class="sxs-lookup"><span data-stu-id="749bd-p108">Open the project's **App.xaml** file and locate the `Application.Resources` node. Replace the application ID and redirect URI placeholders with the corresponding values of the app you registered.</span></span>


```xml
    <Application.Resources>
        <!-- Add your Client Id here. -->
        <x:String x:Key="ida:ClientID">ENTER_YOUR_CLIENT_ID</x:String>
        <!-- Add your Redirect URI here. -->
        <x:String x:Key="ida:ReturnUrl">ENTER_YOUR_REDIRECT_URI</x:String>
    </Application.Resources>
```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="749bd-143">Senden einer E-Mail mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="749bd-143">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="749bd-p109">Öffnen Sie die Datei MailHelper.cs in Ihrem Startprojekt. Diese Datei enthält den Code, durch den eine E-Mail erstellt und gesendet wird. Er besteht aus einer einzigen Methode – ``ComposeAndSendMailAsync`` –, die eine POST-Anforderung konstruiert und an den Endpunkt **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** sendet.</span><span class="sxs-lookup"><span data-stu-id="749bd-p109">Open the MailHelper.cs file in your starter project. This file contains the code that constructs and sends an email. It consists of a single method -- ``ComposeAndSendMailAsync`` -- that constructs and sends a POST request to the **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** endpoint.</span></span> 

<span data-ttu-id="749bd-p110">Die ``ComposeAndSendMailAsync``-Methode verwendet die drei Zeichenfolgenwerte ``subject``, ``bodyContent`` und ``recipients``, die von der Datei „MainPage.xaml.cs“ an sie übergeben werden. Die Zeichenfolgen ``subject`` und ``bodyContent`` werden zusammen mit allen anderen Benutzeroberflächenzeichenfolgen in der Datei „Resources.resw“ gespeichert. Die Zeichenfolge ``recipients`` stammt aus dem Adressfeld in der App-Schnittstelle.</span><span class="sxs-lookup"><span data-stu-id="749bd-p110">The ``ComposeAndSendMailAsync`` method takes three string values -- ``subject``, ``bodyContent``, and ``recipients`` -- that are passed to it by the MainPage.xaml.cs file. The ``subject`` and ``bodyContent`` strings are stored, along with all other UI strings, in the Resources.resw file. The ``recipients`` string comes from the address box in the app's interface.</span></span> 

<span data-ttu-id="749bd-p111">Die erste Aufgabe innerhalb der Methode ``ComposeAndSendMailAsync`` besteht darin, das Foto des aktuellen Benutzers aus Microsoft Graph abzurufen. Diese Zeile ruft die Methode `GetCurrentUserPhotoStreamAsync` auf:</span><span class="sxs-lookup"><span data-stu-id="749bd-p111">The first task inside the ``ComposeAndSendMailAsync`` method is to get the current user's photo from Microsoft Graph. This line calls the `GetCurrentUserPhotoStreamAsync` method:</span></span>

```
            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();
```

<span data-ttu-id="749bd-152">Die vollständige Methode `GetCurrentUserPhotoStreamAsync` sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="749bd-152">This is what the complete `GetCurrentUserPhotoStreamAsync` method looks like:</span></span>

```
        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }
```

<span data-ttu-id="749bd-153">Wenn der Benutzer kein Foto hat, wird mit dieser Logik eine andere Bilddatei abgerufen, die in das Projekt eingeschlossen wurde:</span><span class="sxs-lookup"><span data-stu-id="749bd-153">If the user doesn't have a photo, this logic gets another image file that has been included with the project:</span></span>

```
            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                StorageFile file = await Windows.ApplicationModel.Package.Current.InstalledLocation.GetFileAsync("test.jpg");
                photoStream = (await file.OpenReadAsync()).AsStreamForRead();
            }
```

<span data-ttu-id="749bd-154">Nachdem nun ein Bilddatenstrom vorliegt, kann die Datei in OneDrive hochgeladen werden, indem die Methode `UploadFileToOneDriveAsync` aufgerufen wird:</span><span class="sxs-lookup"><span data-stu-id="749bd-154">Now that we have an image stream, we can upload the file to OneDrive by calling the `UploadFileToOneDriveAsync` method:</span></span>

```
            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());
```

<span data-ttu-id="749bd-155">Die vollständige Methode `UploadFileToOneDriveAsync` sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="749bd-155">This is what the complete `UploadFileToOneDriveAsync` method looks like:</span></span>

```
        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }
```

<span data-ttu-id="749bd-156">Dieser Datenstrom kann auch zum Erstellen eines `MessageAttachmentsCollectionPage`-Objekts verwendet werden, das zusammen mit der Nachricht übergeben werden kann:</span><span class="sxs-lookup"><span data-stu-id="749bd-156">We can also use this stream to create a `MessageAttachmentsCollectionPage` object that we can pass along with the message:</span></span>

```
            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });
```

<span data-ttu-id="749bd-p112">Durch Aufruf der Methode `GetSharingLinkAsync` kann ein Freigabelink für die neu hochgeladene OneDrive-Datei abgerufen werden. Die Zeichenfolge `bodyContent` enthält einen Platzhalter für den Freigabelink:</span><span class="sxs-lookup"><span data-stu-id="749bd-p112">We can get a sharing link for the newly uploaded OneDrive file by calling the `GetSharingLinkAsync` method. The `bodyContent` string contains a placeholder for the sharing link:</span></span>

```
            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);
```

<span data-ttu-id="749bd-159">Die vollständige Methode `GetSharingLinkAsync` sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="749bd-159">This is what the complete `GetSharingLinkAsync` method looks like:</span></span>

```
        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }
```

<span data-ttu-id="749bd-160">Da der Benutzer mehrere Adressen übergeben kann, besteht die nächste Aufgabe darin, die Zeichenfolge ``recipients`` in einen Satz von `EmailAddress`-Objekten zu unterteilen, die dann verwendet werden können, um die Liste der `Recipients`-Objekte zu erstellen, die im POST-Text der Anforderung übergeben werden.</span><span class="sxs-lookup"><span data-stu-id="749bd-160">Since the user can potentially pass more than one address, the next task is to split the ``recipients`` string into a set of `EmailAddress` objects that can then be used to construct the list of `Recipients` objects that will be passed in the POST body of the request:</span></span>

```
            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }
```

<span data-ttu-id="749bd-p113">Die letzte Aufgabe besteht darin, ein `Message`-Objekt zu erstellen und dieses über den `GraphServiceClient` an den Endpunkt **me/microsoft.graph.SendMail** zu senden. Da die Zeichenfolge ``bodyContent`` ein HTML-Dokument ist, legt die Anforderung den Wert **ContentType** auf HTML fest.</span><span class="sxs-lookup"><span data-stu-id="749bd-p113">The last task is to construct a `Message` object and send it to the **me/microsoft.graph.SendMail** endpoint through the `GraphServiceClient`. Since the ``bodyContent`` string is an HTML document, the request sets the **ContentType** value to HTML.</span></span>

```
            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
```

<span data-ttu-id="749bd-163">Die vollständige Klasse sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="749bd-163">The complete class will look like this:</span></span>

```
    public class MailHelper
    {
        /// <summary>
        /// Compose and send a new email.
        /// </summary>
        /// <param name="subject">The subject line of the email.</param>
        /// <param name="bodyContent">The body of the email.</param>
        /// <param name="recipients">A semicolon-separated list of email addresses.</param>
        /// <returns></returns>
        public async Task ComposeAndSendMailAsync(string subject,
                                                            string bodyContent,
                                                            string recipients)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                StorageFile file = await Windows.ApplicationModel.Package.Current.InstalledLocation.GetFileAsync("test.jpg");
                photoStream = (await file.OpenReadAsync()).AsStreamForRead();
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);

            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
        }


        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
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
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }

    }
``` 

 
<span data-ttu-id="749bd-164">Sie haben nun die erforderlichen Schritte für die Interaktion mit Microsoft Graph durchgeführt: App-Registrierung, Benutzerauthentifizierung und Ausführen der Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="749bd-164">You've now performed the steps required for interacting with Microsoft Graph: app registration, user authentication, and making the requests.</span></span> 

## <a name="run-the-app"></a><span data-ttu-id="749bd-165">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="749bd-165">Run the app</span></span>
1. <span data-ttu-id="749bd-166">Drücken Sie zum Erstellen und Ausführen der App F5.</span><span class="sxs-lookup"><span data-stu-id="749bd-166">Press F5 to build and run the app.</span></span> 

2. <span data-ttu-id="749bd-167">Melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an, und gewähren Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="749bd-167">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

3. <span data-ttu-id="749bd-p114">Klicken Sie auf die Schaltfläche **E-Mail senden**. Wenn die E-Mail gesendet wird, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt. Die E-Mail-Nachricht enthält das Foto als Anlage und stellt außerdem einen Freigabelink zur hochgeladenen Datei in OneDrive bereit.</span><span class="sxs-lookup"><span data-stu-id="749bd-p114">Choose the **Send email** button. When the mail is sent, a Success message is displayed below the button. the mail message includes the photo as an attachment and also provides a sharing link to the uploaded file in OneDrive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="749bd-171">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="749bd-171">Next steps</span></span>
- <span data-ttu-id="749bd-172">Testen Sie die REST-API mithilfe des [Graph-Explorers]((https://developer.microsoft.com/de-DE/graph/graph-explorer)).</span><span class="sxs-lookup"><span data-stu-id="749bd-172">Try out the REST API using the [Graph explorer]((https://developer.microsoft.com/de-DE/graph/graph-explorer)).</span></span>
- <span data-ttu-id="749bd-173">Beispiele allgemeiner Vorgänge sowohl für REST- als auch für SDK-Operationen finden Sie im [Microsoft Graph UWP Snippets-Beispiel (SDK)]((https://github.com/microsoftgraph/uwp-csharp-snippets-sample)) und im [Microsoft Graph UWP Snippets-Beispiel (REST)]((https://github.com/microsoftgraph/uwp-csharp-snippets-rest-sample)), oder erforschen Sie unsere [UWP-Bespiele](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=uwp) auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="749bd-173">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph UWP Snippets Sample (SDK)]((https://github.com/microsoftgraph/uwp-csharp-snippets-sample)) and the [Microsoft Graph UWP Snippets Sample (REST)]((https://github.com/microsoftgraph/uwp-csharp-snippets-rest-sample)), or explore our other [UWP samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=uwp) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="749bd-174">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="749bd-174">See also</span></span>
- <span data-ttu-id="749bd-175">[Microsoft Graph .NET Clientbibliothek]((https://github.com/microsoftgraph/msgraph-sdk-dotnet))</span><span class="sxs-lookup"><span data-stu-id="749bd-175">[Microsoft Graph .NET Client Library]((https://github.com/microsoftgraph/msgraph-sdk-dotnet))</span></span>
- <span data-ttu-id="749bd-176">[Protokolle für Azure AD v2.0]((https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-protocols/))</span><span class="sxs-lookup"><span data-stu-id="749bd-176">[Azure AD v2.0 protocols]((https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-protocols/))</span></span>
- <span data-ttu-id="749bd-177">[Azure AD v2.0-Tokens]((https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-tokens/))</span><span class="sxs-lookup"><span data-stu-id="749bd-177">[Azure AD v2.0 tokens]((https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-tokens/))</span></span>

