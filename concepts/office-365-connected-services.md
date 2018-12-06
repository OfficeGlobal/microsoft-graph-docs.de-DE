---
title: Aufrufen von Office 365-Diensten in Visual Studio 2017 mit der Microsoft Graph-API
description: Sie können Connected Services in Visual Studio verwenden, um Ihre App für den Aufruf der Microsoft Graph-API zu konfigurieren. In diesem Artikel wird beschrieben, wie Sie das Profilfoto eines angemeldeten Benutzers abrufen, in OneDrive hochladen und eine E-Mail mit einem Freigabelink zum Foto senden.
ms.openlocfilehash: 33469dec7014d81ed55c2efceb96a26c2651d239
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092233"
---
# <a name="call-office-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a><span data-ttu-id="fbecf-104">Aufrufen von Office 365-Diensten in Visual Studio 2017 mit der Microsoft Graph-API</span><span class="sxs-lookup"><span data-stu-id="fbecf-104">Call Office 365 services in Visual Studio 2017 with the Microsoft Graph API</span></span>

<span data-ttu-id="fbecf-p102">Sie können Connected Services in Visual Studio verwenden, um Ihre App für den Aufruf der Microsoft Graph-API zu konfigurieren. In diesem Artikel wird beschrieben, wie Sie das Profilfoto eines angemeldeten Benutzers abrufen, in OneDrive hochladen und eine E-Mail mit einem Freigabelink zum Foto senden.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p102">You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API. This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.</span></span>

## <a name="get-set-up"></a><span data-ttu-id="fbecf-107">Einrichten</span><span class="sxs-lookup"><span data-stu-id="fbecf-107">Get set up</span></span>

<span data-ttu-id="fbecf-108">Um Office 365 Connected Services mit Microsoft Graph zu verwenden, müssen Sie die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="fbecf-108">To use the Office 365 Connected Services with Microsoft Graph, you'll need to do the following:</span></span>

- <span data-ttu-id="fbecf-p103">Laden Sie die [Vorschauversion von Visual Studio 2017 ](https://www.visualstudio.com/vs/preview/) herunter, sofern Sie dies noch nicht getan haben. Wenn Sie eine frühere Version von Visual Studio verwenden, können Sie die Vorschauversion Visual Studio 2017 parallel zu Ihrer aktuellen Version verwenden.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p103">Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already. If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.</span></span>

- <span data-ttu-id="fbecf-p104">Erwerben Sie ein Office 365-Abonnement. Um eine kostenlose Testversion zu erhalten, nehmen Sie am [Office 365-Entwicklerprogramm](https://dev.office.com/devprogram) teil.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p104">Get an Office 365 subscription. To get a free trial, join the [Office 365 Developer program](https://dev.office.com/devprogram).</span></span>

## <a name="get-the-starter-project"></a><span data-ttu-id="fbecf-113">Abrufen des Startprojekts</span><span class="sxs-lookup"><span data-stu-id="fbecf-113">Get the starter project</span></span>

<span data-ttu-id="fbecf-p105">Laden Sie das [Microsoft Graph ASP.NET-Beispiel für Connected Services](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip) herunter. Dieses Beispiel enthält die Referenzen, die Sie zum Authentifizieren bei Microsoft Graph benötigen. Nachdem Sie das Startprojekt herunterladen haben, entzippen Sie es, und öffnen Sie das Beispiel in der Vorschauversion von Visual Studio 2017.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p105">Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). This sample includes the references that you need to authenticate against Microsoft Graph. After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.</span></span>

## <a name="add-the-connected-service"></a><span data-ttu-id="fbecf-117">Hinzufügen des verbundenen Diensts</span><span class="sxs-lookup"><span data-stu-id="fbecf-117">Add the Connected Service</span></span>

<span data-ttu-id="fbecf-118">Nun können Sie den Microsoft Graph-Dienst zu Ihrem Visual Studio-Projekt hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="fbecf-118">You're now ready to add the Microsoft Graph service to your Visual Studio project.</span></span> 

1. <span data-ttu-id="fbecf-119">Wählen Sie im Projektmappen-Explorer **Verbundene Dienste** aus, um die Registerkarte „Verbundene Dienste“ zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="fbecf-119">In Solution Explorer, choose **Connected Services** to open the Connected Services tab.</span></span> 

2. <span data-ttu-id="fbecf-p106">Wählen Sie den Anbieter **Mit Microsoft Graph auf Office 365-Dienste zugreifen** aus. Folgen Sie den Anweisungen des Assistenten. Wählen Sie die folgenden Berechtigungen aus (Sie können sie später ändern):</span><span class="sxs-lookup"><span data-stu-id="fbecf-p106">Choose the **Access Office 365 Services with Microsoft Graph** provider. Follow the wizard. Select the following permissions (you can change the permisssions later):</span></span>

    - <span data-ttu-id="fbecf-123">Für die **Datei**-APIs legen Sie die Berechtigungen auf **Vollzugriff auf Ihre Dateien** fest.</span><span class="sxs-lookup"><span data-stu-id="fbecf-123">For the **File** APIs, set permissions to **Have full access to your files**.</span></span>
    - <span data-ttu-id="fbecf-124">Für die **E-Mail**-APIs legen Sie die Berechtigungen auf **E-Mails in Ihrem Namen senden** fest.</span><span class="sxs-lookup"><span data-stu-id="fbecf-124">For the **Mail** APIs, set permissions to **Send mail as you**.</span></span>
    - <span data-ttu-id="fbecf-125">Für die **Benutzer**-APIs legen Sie die Berechtigungen auf **Sie anmelden und Ihr Profil lesen** fest.</span><span class="sxs-lookup"><span data-stu-id="fbecf-125">For the **User** APIs, set permissions to **Sign you in and read your profile**.</span></span>

## <a name="call-the-microsoft-graph-api"></a><span data-ttu-id="fbecf-126">Aufrufen der Microsoft Graph-API</span><span class="sxs-lookup"><span data-stu-id="fbecf-126">Call the Microsoft Graph API</span></span>

<span data-ttu-id="fbecf-p107">Das Startbeispiel ist für den Versand einer einfachen E-Mail konfiguriert. Sie können Microsoft Graph verwenden, um das Beispiel zu aktualisieren und eine E-Mail mit einem Link zum Profilfoto des angemeldeten Benutzers in OneDrive zu senden.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p107">The starter sample is configured to send a simple email. You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.</span></span>

1. <span data-ttu-id="fbecf-129">Wechseln Sie zu „Models\GraphService.cs“. Diese Datei enthält den Code zum Aufrufen von Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fbecf-129">Go to 'Models\GraphService.cs', which hosts the code to call Microsoft Graph.</span></span>

2. <span data-ttu-id="fbecf-p108">Suchen Sie Aufrufe des SDK in den folgenden Methoden, und **kommentieren Sie sie aus**. Hier wird gezeigt, wie Sie Microsoft Graph aufrufen, um ein Profilfoto abzurufen, eine Datei in OneDrive hochzuladen und einen Freigabelink zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p108">Find and **Uncomment** calls to the SDK in the following methods. This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.</span></span>

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> <span data-ttu-id="fbecf-132">**Tipp:** Jeder Kommentar beginnt mit „//Uncomment:“</span><span class="sxs-lookup"><span data-stu-id="fbecf-132">**Tip:** Each comment starts with '//Uncomment:'</span></span>
 

## <a name="run-the-sample"></a><span data-ttu-id="fbecf-133">Ausführen des Beispiels</span><span class="sxs-lookup"><span data-stu-id="fbecf-133">Run the sample</span></span>
<span data-ttu-id="fbecf-p109">Erstellen Sie das Beispiel, und führen Sie es aus. Wählen Sie als Nächstes den Link **Anmelden** in der rechten oberen Ecke, und wählen Sie dann **E-Mail-Adresse abrufen** gefolgt von **E-Mail senden**.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p109">Build and run the sample. Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.</span></span>

<span data-ttu-id="fbecf-136">Hierdurch wird eine E-Mail gesendet, die einen Link zu Ihrem Profilfoto enthält.</span><span class="sxs-lookup"><span data-stu-id="fbecf-136">This will send an email that includes a link to your profile photo.</span></span>

><span data-ttu-id="fbecf-137">**Hinweise:**</span><span class="sxs-lookup"><span data-stu-id="fbecf-137">**Notes:**</span></span>

>- <span data-ttu-id="fbecf-138">Wenn Sie den Vorgang beenden und das Beispiel erneut in Visual Studio ausführen, müssen Sie sich möglicherweise explizit abmelden, damit das Beispiel funktioniert.</span><span class="sxs-lookup"><span data-stu-id="fbecf-138">If you stop and rerun the sample from Visual Studio, you might need to explicitly sign out for the sample to work.</span></span>
>- <span data-ttu-id="fbecf-139">Wenn Sie eine Ausnahme erhalten, die angibt, dass der Benutzer nicht authentifiziert ist, müssen Sie möglicherweise den Schritt [Hinzufügen des verbundenen Diensts](#add-the-connected-service) wiederholen.</span><span class="sxs-lookup"><span data-stu-id="fbecf-139">If you get an exception that indicates that the User is not authenticated, you might need to repeat the [Add the Connected Service](#add-the-connected-service) step.</span></span>
    

## <a name="explore-the-code"></a><span data-ttu-id="fbecf-140">Untersuchen des Codes</span><span class="sxs-lookup"><span data-stu-id="fbecf-140">Explore the code</span></span>

<span data-ttu-id="fbecf-p110">Sie können nun mithilfe von Visual Studio 2017 eine Verbindung mit Ihren Diensten herstellen und diese konfigurieren. Im Startbeispiel werden das Gerüst und die Verweise für Sie erstellt.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p110">You can now use Visual Studio 2017 to connect to and configure your services. The starter sample creates the scaffolding and references for you.</span></span>  

<span data-ttu-id="fbecf-143">Das Startbeispiel umfasst die folgenden Dateien:</span><span class="sxs-lookup"><span data-stu-id="fbecf-143">The starter sample includes the following files:</span></span>

- <span data-ttu-id="fbecf-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs): Authentifiziert den aktuellen Benutzer und initialisiert den Tokencache des Beispiels.</span><span class="sxs-lookup"><span data-stu-id="fbecf-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - Authenticates the current user and initializes the sample's token cache.</span></span>

- <span data-ttu-id="fbecf-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs): Enthält die Tokeninformationen des Benutzers. Sie können diesen durch Ihren eigenen benutzerdefinierten Tokencache ersetzen. Weitere Informationen finden Sie unter [Zwischenspeichern von Zugriffstoken in einer mehrinstanzenfähigen Anwendung](https://azure.microsoft.com/de-DE/documentation/articles/guidance-multitenant-identity-token-cache/).</span><span class="sxs-lookup"><span data-stu-id="fbecf-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information. You can replace this with your own custom token cache. For more information, see [Caching access tokens in a multitenant application](https://azure.microsoft.com/de-DE/documentation/articles/guidance-multitenant-identity-token-cache/).</span></span>

- <span data-ttu-id="fbecf-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs): Implementiert die lokale IAuthProvider-Schnittstelle und ruft ein Zugriffstoken ab.</span><span class="sxs-lookup"><span data-stu-id="fbecf-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - Implements the local IAuthProvider interface, and gets an access token.</span></span> 

- <span data-ttu-id="fbecf-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs): Initialisiert den **GraphServiceClient** aus der [Microsoft Graph .NET-Clientbibliothek](https://github.com/microsoftgraph/msgraph-sdk-dotnet), die für die Interaktion mit Microsoft Graph verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="fbecf-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - Initializes the **GraphServiceClient** from the [Microsoft Graph .NET Client Library](https://github.com/microsoftgraph/msgraph-sdk-dotnet) that is used to interact with the Microsoft Graph.</span></span>

- <span data-ttu-id="fbecf-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs): Enthält Methoden, die den **GraphServiceClient** zum Erstellen und Senden von Aufrufen des Microsoft Graph-Diensts und zum Verarbeiten der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="fbecf-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - Contains methods that use the **GraphServiceClient** to build and send calls to the Microsoft Graph service and to process the response.</span></span>

- <span data-ttu-id="fbecf-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml): Enthält die Benutzeroberfläche für das Beispiel.</span><span class="sxs-lookup"><span data-stu-id="fbecf-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - Contains the UI for the sample.</span></span> 


## <a name="need-help"></a><span data-ttu-id="fbecf-152">Benötigen Sie Hilfe?</span><span class="sxs-lookup"><span data-stu-id="fbecf-152">Need help?</span></span>

<span data-ttu-id="fbecf-p112">Wenn Sie Hilfe benötigen, veröffentlichen Sie Ihre Fragen in [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Taggen Sie Ihren Beitrag mit {microsoftgraph}.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p112">If you need help, post your questions on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your post with {microsoftgraph}.</span></span>

