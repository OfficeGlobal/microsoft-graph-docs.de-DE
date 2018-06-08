# <a name="get-started-with-microsoft-graph-in-a-xamarin-forms-app"></a><span data-ttu-id="0819c-101">Erste Schritte mit Microsoft Graph in einer Xamarin Forms-App</span><span class="sxs-lookup"><span data-stu-id="0819c-101">Get started with Microsoft Graph in a Xamarin Forms app</span></span>

> <span data-ttu-id="0819c-p101">**Sie erstellen Apps für Unternehmenskunden?** Ihre App funktioniert möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfunktionen wie <a href="https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">bedingten Gerätezugriff</a> aktiviert. In diesem Fall treten bei Ihren Kunden möglicherweise Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="0819c-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

<span data-ttu-id="0819c-p102">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom [Azure AD v2.0-Endpunkt](https://developer.microsoft.com/graph/docs/concepts/converged_auth) und zum Aufrufen von Microsoft Graph. Er führt Sie durch den Code im [Microsoft Graph Connect-Beispiel für Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) und erläutert die wichtigsten Konzepte, die in einer App implementiert werden müssen, die Microsoft Graph verwendet. In diesem Artikel wird auch beschrieben, wie Sie mit der [Microsoft Graph Clientbibliothek](http://www.nuget.org/packages/Microsoft.Graph/) auf Microsoft Graph zugreifen.</span><span class="sxs-lookup"><span data-stu-id="0819c-p102">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) sample to explain the main concepts that you have to implement in an app that uses Microsoft Graph. The article also describes how to access Microsoft Graph by using the [Microsoft Graph Client Library](http://www.nuget.org/packages/Microsoft.Graph/).</span></span>

<span data-ttu-id="0819c-108">Dies ist die App, die Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="0819c-108">This is the app you'll create.</span></span>

| <span data-ttu-id="0819c-109">UWP</span><span class="sxs-lookup"><span data-stu-id="0819c-109">UWP</span></span> | <span data-ttu-id="0819c-110">Android</span><span class="sxs-lookup"><span data-stu-id="0819c-110">Android</span></span> | <span data-ttu-id="0819c-111">iOS</span><span class="sxs-lookup"><span data-stu-id="0819c-111">iOS</span></span> |
| --- | ------- | ----|
| <img src="images/UWP.png" alt="Connect sample on UWP" width="100%" /> | <img src="images/Droid.png" alt="Connect sample on Android" width="100%" /> | <img src="images/iOS.png" alt="Connect sample on iOS" width="100%" /> |

<span data-ttu-id="0819c-p103">**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Schnellstart Microsoft Graph](https://developer.microsoft.com/graph/quick-start), oder laden Sie das [Microsoft Graph Connect-Beispiel für Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) herunter, auf dem dieser Artikel basiert.</span><span class="sxs-lookup"><span data-stu-id="0819c-p103">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/graph/quick-start) to get up and running fast, or download the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) that this article is based on.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0819c-114">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0819c-114">Prerequisites</span></span>

<span data-ttu-id="0819c-115">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="0819c-115">To get started, you'll need:</span></span> 

- <span data-ttu-id="0819c-116">Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="0819c-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="0819c-117">Visual Studio 2015</span><span class="sxs-lookup"><span data-stu-id="0819c-117">Visual Studio 2015</span></span> 
- [<span data-ttu-id="0819c-118">Xamarin für Visual Studio</span><span class="sxs-lookup"><span data-stu-id="0819c-118">Xamarin for Visual Studio</span></span>](https://www.xamarin.com/visual-studio)
- <span data-ttu-id="0819c-119">Windows 10 (mit [aktiviertem Entwicklungsmodus](https://msdn.microsoft.com/library/windows/apps/xaml/dn706236.aspx))</span><span class="sxs-lookup"><span data-stu-id="0819c-119">Windows 10 ([development mode enabled](https://msdn.microsoft.com/library/windows/apps/xaml/dn706236.aspx))</span></span>
- <span data-ttu-id="0819c-p104">Das [Microsoft Graph Connect-Startprojekt für Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample/tree/master/starter). Diese Vorlage enthält verschiedene Klassen, denen Sie Code hinzufügen müssen. Darüber hinaus enthält sie vollständige Ansichten und Ressourcenzeichenfolgen. Um dieses Projekt abzurufen, müssen Sie das [Microsoft Graph Connect-Beispiel für Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) klonen oder herunterladen und dann die **XamarinConnect**-Projektmappe im **Start**ordner öffnen.</span><span class="sxs-lookup"><span data-stu-id="0819c-p104">The [Microsoft Graph Connect Starter Project for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample/tree/master/starter). This template contains several classes that you'll add code to. It also contains complete views and resource strings. To get this project, clone or download the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) and open the **XamarinConnect** solution inside the **starter** folder.</span></span> 

<span data-ttu-id="0819c-124">Wenn Sie das iOS-Projekt in diesem Beispiel ausführen möchten, benötigen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="0819c-124">If you want to run the iOS project in this sample, you'll need the following:</span></span>

- <span data-ttu-id="0819c-125">Das neueste iOS-SDK</span><span class="sxs-lookup"><span data-stu-id="0819c-125">The latest iOS SDK</span></span>
- <span data-ttu-id="0819c-126">Die neueste Version von Xcode</span><span class="sxs-lookup"><span data-stu-id="0819c-126">The latest version of Xcode</span></span>
- <span data-ttu-id="0819c-127">Mac OS X Sierra (10.12) und höher</span><span class="sxs-lookup"><span data-stu-id="0819c-127">Mac OS X Sierra(10.12) & above</span></span> 
- [<span data-ttu-id="0819c-128">Xamarin.iOS</span><span class="sxs-lookup"><span data-stu-id="0819c-128">Xamarin.iOS</span></span>](https://docs.microsoft.com/visualstudio/mac/installation)
- <span data-ttu-id="0819c-129">Einen mit [Visual Studio verbundenen Xamarin Mac-Agent](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)</span><span class="sxs-lookup"><span data-stu-id="0819c-129">A [Xamarin Mac agent connected to Visual Studio](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)</span></span>


## <a name="register-the-app"></a><span data-ttu-id="0819c-130">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="0819c-130">Register the app</span></span>
 
1. <span data-ttu-id="0819c-131">Melden Sie sich beim [App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="0819c-131">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="0819c-132">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="0819c-132">Select **Add an app**.</span></span>
3. <span data-ttu-id="0819c-133">Geben Sie einen Namen für die App ein, und wählen Sie dann **Erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="0819c-133">Enter a name for the app, and select **Create**.</span></span>
    
    <span data-ttu-id="0819c-134">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="0819c-134">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="0819c-135">Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="0819c-135">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="0819c-136">Wählen Sie **Systemeigene Anwendung**.</span><span class="sxs-lookup"><span data-stu-id="0819c-136">Select **Native Application**.</span></span>
6. <span data-ttu-id="0819c-p105">Kopieren Sie den ID-Wert der Anwendung und den Wert für den benutzerdefinierten Umleitungs-URI (unter **Systemeigene Anwendung**), der für Sie erstellt wurde, als Sie die Plattform **Systemeigene Anwendung** hinzugefügt haben. Dieser URI muss den Wert der Anwendungs-ID enthalten und das folgende Format aufweisen: `msal[Application Id]://auth` Sie müssen diese Werte in die Beispiel-App eingeben.</span><span class="sxs-lookup"><span data-stu-id="0819c-p105">Copy the Application Id value and the Custom Redirect URI value (under the **Native Application** header) that was created for you when you added the **Native Application** platform. This URI should contain your Application Id value and be in this form: `msal[Application Id]://auth` You'll need to enter these values into the sample app.</span></span>

    <span data-ttu-id="0819c-139">Die App-ID ist ein eindeutiger Bezeichner für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="0819c-139">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="0819c-140">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="0819c-140">Select **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="0819c-141">Konfigurieren des Projekts</span><span class="sxs-lookup"><span data-stu-id="0819c-141">Configure the project</span></span>

1. <span data-ttu-id="0819c-142">Öffnen Sie die Projektmappendatei für das Startprojekt in Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="0819c-142">Open the solution file for the starter project in Visual Studio.</span></span>
2. <span data-ttu-id="0819c-p106">Öffnen Sie die Datei **App.cs** innerhalb des Projekts **XamarinConnect (Portable)**, und suchen Sie das Feld `ClientId`. Ersetzen Sie den Platzhalter-der Anwendungs-ID durch die Anwendungs-ID der App, die Sie registriert haben.</span><span class="sxs-lookup"><span data-stu-id="0819c-p106">Open the **App.cs** file inside the **XamarinConnect (Portable)** project and locate the `ClientId` field. Replace the application ID placeholder with the application id of the app you registered.</span></span>

    ```
    public static string ClientID = "ENTER_YOUR_CLIENT_ID";
    public static string RedirectUri = "msal" + ClientID + "://auth";
    public static string[] Scopes = { "User.Read", "Mail.Send", "Files.ReadWrite" };
    ```
    <span data-ttu-id="0819c-p107">Im Wert `Scopes` sind die Microsoft Graph Berechtigungsbereiche gespeichert, die die App anfordern muss, wenn der Benutzer sich authentifiziert. Beachten Sie, dass der Klassenkonstruktor `App` den ClientID-Wert verwendet, um eine Instanz der MSAL-Klasse `PublicClientApplication` zu instanziieren. Sie verwenden diese Klasse später zum Authentifizieren des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="0819c-p107">The `Scopes` value stores the Microsoft Graph permission scopes that the app will need to request when the user authenticates. Note that the `App` class constructor uses the ClientID value to instantiate an instance of the MSAL `PublicClientApplication` class. You'll use this class later to authenticate the user.</span></span>
    
    ```
    IdentityClientApp = new PublicClientApplication(ClientID);
    ```

3. <span data-ttu-id="0819c-p108">Öffnen Sie die Datei „UserDetailsClient.iOS\info.plist“ in einem Texteditor. Sie können diese Datei leider nicht in Visual Studio bearbeiten. Suchen Sie das Element `<string>msalENTER_YOUR_CLIENT_ID</string>` unter dem Schlüssel `CFBundleURLSchemes`.</span><span class="sxs-lookup"><span data-stu-id="0819c-p108">Open the UserDetailsClient.iOS\info.plist file in a text editor. Unfortunately you can't edit this file in Visual Studio. Locate the `<string>msalENTER_YOUR_CLIENT_ID</string>` element under `CFBundleURLSchemes` key.</span></span>

4. <span data-ttu-id="0819c-p109">Ersetzen Sie `ENTER_YOUR_CLIENT_ID` durch den Wert der Anwendungs-ID, die Sie beim Registrieren der App erhalten haben. Sie müssen `msal` unbedingt vor der Anwendungs-ID beibehalten. Der resultierende Zeichenfolgenwert sollte wie folgt aussehen: `<string>msal[application id]</string>`.</span><span class="sxs-lookup"><span data-stu-id="0819c-p109">Replace `ENTER_YOUR_CLIENT_ID` with the application id value that you got when you registered your app. Be sure to retain `msal` before the application id. The resulting string value should look like this: `<string>msal[application id]</string>`.</span></span>

5. <span data-ttu-id="0819c-p110">Öffnen Sie die Datei „UserDetailsClient.Droid\Properties\AndroidManifest.xml“. Suchen Sie das folgende Element: `<data android:scheme="msalENTER_YOUR_CLIENT_ID" android:host="auth" />`.</span><span class="sxs-lookup"><span data-stu-id="0819c-p110">Open the UserDetailsClient.Droid\Properties\AndroidManifest.xml file. Locate this element: `<data android:scheme="msalENTER_YOUR_CLIENT_ID" android:host="auth" />`.</span></span>

6. <span data-ttu-id="0819c-p111">Ersetzen Sie `ENTER_YOUR_CLIENT_ID` durch den Wert der Anwendungs-ID, die Sie beim Registrieren der App erhalten haben. Sie müssen `msal` unbedingt vor der Anwendungs-ID beibehalten. Der resultierende Zeichenfolgenwert sollte wie folgt aussehen: `<data android:scheme="msal[application id]" android:host="auth" />`.</span><span class="sxs-lookup"><span data-stu-id="0819c-p111">Replace `ENTER_YOUR_CLIENT_ID` with the application id value that you got when you registered your app. Be sure to retain `msal` before the application id. The resulting string value should look like this: `<data android:scheme="msal[application id]" android:host="auth" />`.</span></span>

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="0819c-157">Senden einer E-Mail mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0819c-157">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="0819c-158">Öffnen Sie die Datei MailHelper.cs in Ihrem Startprojekt.</span><span class="sxs-lookup"><span data-stu-id="0819c-158">Open the MailHelper.cs file in your starter project.</span></span> <span data-ttu-id="0819c-159">Diese Datei enthält den Code, der E-Mails erstellt und sendet.</span><span class="sxs-lookup"><span data-stu-id="0819c-159">This file contains the code that constructs and sends an email.</span></span> <span data-ttu-id="0819c-160">Er besteht aus einer einzigen Methode (``ComposeAndSendMailAsync``), die eine POST-Anforderung erstellt und an den Endpunkt **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** sendet.</span><span class="sxs-lookup"><span data-stu-id="0819c-160">The MailHelper.cs file contains the code that constructs and sends an email. It consists of a single method --  -- that constructs and sends a POST request to the https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail endpoint.</span></span> 

<span data-ttu-id="0819c-p113">Die Methode ``ComposeAndSendMailAsync`` verwendet drei Zeichenfolgenwerte – ``subject``, ``bodyContent`` und ``recipients`` –, die von der Datei "MainPage.xaml.cs" an sie übergeben werden. Die Zeichenfolgen ``subject`` und ``bodyContent`` werden zusammen mit allen anderen Benutzeroberflächenzeichenfolgen in der Datei „AppResources.resx“ gespeichert. Die Zeichenfolge ``recipients`` stammt aus dem Adressfeld in der App-Schnittstelle.</span><span class="sxs-lookup"><span data-stu-id="0819c-p113">The ``ComposeAndSendMailAsync`` method takes three string values -- ``subject``, ``bodyContent``, and ``recipients`` -- that are passed to it by the MainPage.xaml.cs file. The ``subject`` and ``bodyContent`` strings are stored, along with all other UI strings, in the AppResources.resx file. The ``recipients`` string comes from the address box in the app's interface.</span></span> 

<span data-ttu-id="0819c-164">**Verwenden von Deklarationen**</span><span class="sxs-lookup"><span data-stu-id="0819c-164">**Using declarations**</span></span>

<span data-ttu-id="0819c-165">Stellen Sie sicher, dass diese Deklarationen am Anfang der Datei vorhanden sind:</span><span class="sxs-lookup"><span data-stu-id="0819c-165">Make sure you have these declarations at the top of the file:</span></span>

```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Reflection;
using System.Threading.Tasks;
using Microsoft.Graph;
```

<span data-ttu-id="0819c-p114">Die erste Aufgabe innerhalb der Methode ``ComposeAndSendMailAsync`` besteht darin, das Foto des aktuellen Benutzers aus Microsoft Graph abzurufen. Diese Zeile ruft die Methode `GetCurrentUserPhotoStreamAsync` auf, die als Stub vorliegt:</span><span class="sxs-lookup"><span data-stu-id="0819c-p114">The first task inside the ``ComposeAndSendMailAsync`` method is to get the current user's photo from Microsoft Graph. This line calls the stubbed-out `GetCurrentUserPhotoStreamAsync` method:</span></span>

```
            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();
```

<span data-ttu-id="0819c-168">Die vollständige Methode `GetCurrentUserPhotoStreamAsync` sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="0819c-168">This is what the complete `GetCurrentUserPhotoStreamAsync` method looks like:</span></span>

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

<span data-ttu-id="0819c-169">Wenn der Benutzer kein Foto hat, wird mit dieser Logik eine andere Bilddatei abgerufen, die in das Projekt eingeschlossen wurde:</span><span class="sxs-lookup"><span data-stu-id="0819c-169">If the user doesn't have a photo, this logic gets another image file that has been included with the project:</span></span>

```
            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
            }
```

<span data-ttu-id="0819c-170">Nachdem nun ein Bilddatenstrom vorliegt, kann die Datei in OneDrive hochgeladen werden, indem die als Stub vorliegende Methode `UploadFileToOneDriveAsync` aufgerufen wird:</span><span class="sxs-lookup"><span data-stu-id="0819c-170">Now that we have an image stream, we can upload the file to OneDrive by calling the stubbed-out `UploadFileToOneDriveAsync` method:</span></span>

```
            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());
```

<span data-ttu-id="0819c-171">Die vollständige Methode `UploadFileToOneDriveAsync` sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="0819c-171">This is what the complete `UploadFileToOneDriveAsync` method looks like:</span></span>

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

<span data-ttu-id="0819c-172">Dieser Datenstrom kann auch zum Erstellen eines `MessageAttachmentsCollectionPage`-Objekts verwendet werden, das zusammen mit der Nachricht übergeben werden kann:</span><span class="sxs-lookup"><span data-stu-id="0819c-172">We can also use this stream to create a `MessageAttachmentsCollectionPage` object that we can pass along with the message:</span></span>

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

<span data-ttu-id="0819c-p115">Durch Aufruf der als Stub vorliegenden Methode `GetSharingLinkAsync` kann ein Freigabelink für die neu hochgeladene OneDrive-Datei abgerufen werden. Die Zeichenfolge `bodyContent` enthält einen Platzhalter für den Freigabelink:</span><span class="sxs-lookup"><span data-stu-id="0819c-p115">We can get a sharing link for the newly uploaded OneDrive file by calling the stubbed-out `GetSharingLinkAsync` method. The `bodyContent` string contains a placeholder for the sharing link:</span></span>

```
            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);
```

<span data-ttu-id="0819c-175">Die vollständige Methode `GetSharingLinkAsync` sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="0819c-175">This is what the complete `GetSharingLinkAsync` method looks like:</span></span>

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

<span data-ttu-id="0819c-176">Da der Benutzer mehrere Adressen übergeben kann, besteht die nächste Aufgabe darin, die Zeichenfolge ``recipients`` in einen Satz von `EmailAddress`-Objekten zu unterteilen, die dann verwendet werden können, um die Liste der `Recipients`-Objekte zu erstellen, die im POST-Text der Anforderung übergeben werden.</span><span class="sxs-lookup"><span data-stu-id="0819c-176">Since the user can potentially pass more than one address, the next task is to split the ``recipients`` string into a set of `EmailAddress` objects that can then be used to construct the list of `Recipients` objects that will be passed in the POST body of the request:</span></span>

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

<span data-ttu-id="0819c-p116">Die letzte Aufgabe besteht darin, ein `Message`-Objekt zu erstellen und dieses über den `GraphServiceClient` an den Endpunkt **me/microsoft.graph.SendMail** zu senden. Da die Zeichenfolge ``bodyContent`` ein HTML-Dokument ist, legt die Anforderung den Wert **ContentType** auf HTML fest.</span><span class="sxs-lookup"><span data-stu-id="0819c-p116">The last task is to construct a `Message` object and send it to the **me/microsoft.graph.SendMail** endpoint through the `GraphServiceClient`. Since the ``bodyContent`` string is an HTML document, the request sets the **ContentType** value to HTML.</span></span>

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

<span data-ttu-id="0819c-179">Die vollständige Klasse sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="0819c-179">The complete class will look like this:</span></span>

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
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
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

<span data-ttu-id="0819c-180">Sie haben nun die drei erforderlichen Schritte für die Interaktion mit Microsoft Graph durchgeführt: App-Registrierung, Benutzerauthentifizierung und eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0819c-180">You've now performed the three steps required for interacting with Microsoft Graph: app registration, user authentication, and making a request.</span></span> 

## <a name="run-the-app"></a><span data-ttu-id="0819c-181">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="0819c-181">Run the app</span></span>
1. <span data-ttu-id="0819c-p117">Wählen Sie das auszuführende Projekt aus. Wenn Sie die Option für die universelle Windows-Plattform auswählen, können Sie das Beispiel auf dem lokalen Computer ausführen. Wenn Sie das iOS-Projekt ausführen möchten, müssen Sie eine Verbindung zu einem [Mac herstellen, auf dem die Xamarin-Tools installiert](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/) sind. (Sie können diese Projektmappe auch in Xamarin Studio auf einem Mac öffnen und das Beispiel direkt dort ausführen.) Sie können den [Visual Studio-Emulator für Android](https://www.visualstudio.com/features/msft-android-emulator-vs.aspx) verwenden, wenn Sie das Android-Projekt ausführen möchten.</span><span class="sxs-lookup"><span data-stu-id="0819c-p117">Select the project that you want to run. If you select the Universal Windows Platform option, you can run the sample on the local machine. If you want to run the iOS project, you'll need to connect to a [Mac that has the Xamarin tools](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/) installed on it. (You can also open this solution in Xamarin Studio on a Mac and run the sample directly from there.) You can use the [Visual Studio Emulator for Android](https://www.visualstudio.com/features/msft-android-emulator-vs.aspx) if you want to run the Android project.</span></span> 

    <span data-ttu-id="0819c-186">![](images/SelectProject.png "Auswählen eines Projekts in Visual Studio")</span><span class="sxs-lookup"><span data-stu-id="0819c-186">![](images/SelectProject.png "Select project in Visual Studio")</span></span>

2. <span data-ttu-id="0819c-p118">Drücken Sie F5 zum Erstellen und Debuggen. Führen Sie die Lösung aus, und melden Sie sich entweder mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts-, Schul- oder Unikonto an.</span><span class="sxs-lookup"><span data-stu-id="0819c-p118">Press F5 to build and debug. Run the solution and sign in with either your personal or work or school account.</span></span>
    > <span data-ttu-id="0819c-189">**Hinweis** Möglicherweise müssen Sie den Buildkonfigurations-Manager öffnen, um sicherzustellen, dass die Build- und Bereitstellungsschritte für das UWP-Projekt ausgewählt sind.</span><span class="sxs-lookup"><span data-stu-id="0819c-189">**Note** You might have to open the Build Configuration Manager to make sure that the Build and Deploy steps are selected for the UWP project.</span></span> 

3. <span data-ttu-id="0819c-190">Melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an, und gewähren Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="0819c-190">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

4. <span data-ttu-id="0819c-p119">Klicken Sie auf die Schaltfläche **E-Mail senden**. Nachdem die E-Mail gesendet wurde, wird eine Erfolgsmeldung angezeigt. Diese E-Mail-Nachricht enthält das Foto als Anlage und stellt außerdem einen Freigabelink zur hochgeladenen Datei in OneDrive bereit.</span><span class="sxs-lookup"><span data-stu-id="0819c-p119">Choose the **Send mail** button. When the mail is sent, a Success message is displayed. This mail message includes the photo as an attachment and also provides a sharing link to the uploaded file in OneDrive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0819c-194">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="0819c-194">Next steps</span></span>
- <span data-ttu-id="0819c-195">Testen Sie die REST-API mithilfe des [Graph-Explorers](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="0819c-195">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="0819c-196">Beispiele für allgemeine Vorgänge finden Sie in der [Microsoft Graph SDK Snippets-Bibliothek für Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-snippets-sample), oder erforschen Sie unsere anderen [Xamarin-Beispiele](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=xamarin) auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="0819c-196">Find examples of common operations in the [Microsoft Graph SDK Snippets Library for Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-snippets-sample), or explore our other [Xamarin samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=xamarin) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="0819c-197">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0819c-197">See also</span></span>
- [<span data-ttu-id="0819c-198">Microsoft Graph .NET Clientbibliothek</span><span class="sxs-lookup"><span data-stu-id="0819c-198">Microsoft Graph .NET Client Library</span></span>](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [<span data-ttu-id="0819c-199">Protokolle für Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="0819c-199">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="0819c-200">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="0819c-200">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-v2-tokens/)
