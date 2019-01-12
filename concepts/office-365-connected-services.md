---
title: Aufrufen von Office 365-Diensten in Visual Studio 2017 mit der Microsoft Graph-API
description: Sie können Connected Services in Visual Studio verwenden, um Ihre App für den Aufruf der Microsoft Graph-API zu konfigurieren. In diesem Artikel wird beschrieben, wie Sie das Profilfoto eines angemeldeten Benutzers abrufen, in OneDrive hochladen und eine E-Mail mit einem Freigabelink zum Foto senden.
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: 0a084fd7c4fa946854e3f932586f52cdcce370fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979236"
---
# <a name="call-office-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a>Aufrufen von Office 365-Diensten in Visual Studio 2017 mit der Microsoft Graph-API

Sie können Connected Services in Visual Studio verwenden, um Ihre App für den Aufruf der Microsoft Graph-API zu konfigurieren. In diesem Artikel wird beschrieben, wie Sie das Profilfoto eines angemeldeten Benutzers abrufen, in OneDrive hochladen und eine E-Mail mit einem Freigabelink zum Foto senden.

## <a name="get-set-up"></a>Einrichten

Um Office 365 Connected Services mit Microsoft Graph zu verwenden, müssen Sie die folgenden Schritte ausführen:

- Laden Sie die [Vorschauversion von Visual Studio 2017 ](https://www.visualstudio.com/vs/preview/) herunter, sofern Sie dies noch nicht getan haben. Wenn Sie eine frühere Version von Visual Studio verwenden, können Sie die Vorschauversion Visual Studio 2017 parallel zu Ihrer aktuellen Version verwenden.

- Erwerben Sie ein Office 365-Abonnement. Um eine kostenlose Testversion zu erhalten, nehmen Sie am [Office 365-Entwicklerprogramm](https://dev.office.com/devprogram) teil.

## <a name="get-the-starter-project"></a>Abrufen des Startprojekts

Laden Sie das [Microsoft Graph ASP.NET-Beispiel für Connected Services](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip) herunter. Dieses Beispiel enthält die Referenzen, die Sie zum Authentifizieren bei Microsoft Graph benötigen. Nachdem Sie das Startprojekt herunterladen haben, entzippen Sie es, und öffnen Sie das Beispiel in der Vorschauversion von Visual Studio 2017.

## <a name="add-the-connected-service"></a>Hinzufügen des verbundenen Diensts

Nun können Sie den Microsoft Graph-Dienst zu Ihrem Visual Studio-Projekt hinzufügen. 

1. Wählen Sie im Projektmappen-Explorer **Verbundene Dienste** aus, um die Registerkarte „Verbundene Dienste“ zu öffnen. 

2. Wählen Sie den Anbieter **Mit Microsoft Graph auf Office 365-Dienste zugreifen** aus. Folgen Sie den Anweisungen des Assistenten. Wählen Sie die folgenden Berechtigungen aus (Sie können sie später ändern):

    - Für die **Datei**-APIs legen Sie die Berechtigungen auf **Vollzugriff auf Ihre Dateien** fest.
    - Für die **E-Mail**-APIs legen Sie die Berechtigungen auf **E-Mails in Ihrem Namen senden** fest.
    - Für die **Benutzer**-APIs legen Sie die Berechtigungen auf **Sie anmelden und Ihr Profil lesen** fest.

## <a name="call-the-microsoft-graph-api"></a>Aufrufen der Microsoft Graph-API

Das Startbeispiel ist für den Versand einer einfachen E-Mail konfiguriert. Sie können Microsoft Graph verwenden, um das Beispiel zu aktualisieren und eine E-Mail mit einem Link zum Profilfoto des angemeldeten Benutzers in OneDrive zu senden.

1. Wechseln Sie zu „Models\GraphService.cs“. Diese Datei enthält den Code zum Aufrufen von Microsoft Graph.

2. Suchen Sie Aufrufe des SDK in den folgenden Methoden, und **kommentieren Sie sie aus**. Hier wird gezeigt, wie Sie Microsoft Graph aufrufen, um ein Profilfoto abzurufen, eine Datei in OneDrive hochzuladen und einen Freigabelink zu erhalten.

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> **Tipp:** Jeder Kommentar beginnt mit „//Uncomment:“
 

## <a name="run-the-sample"></a>Ausführen des Beispiels
Erstellen Sie das Beispiel, und führen Sie es aus. Wählen Sie als Nächstes den Link **Anmelden** in der rechten oberen Ecke, und wählen Sie dann **E-Mail-Adresse abrufen** gefolgt von **E-Mail senden**.

Hierdurch wird eine E-Mail gesendet, die einen Link zu Ihrem Profilfoto enthält.

>**Hinweise:**

>- Wenn Sie den Vorgang beenden und das Beispiel erneut in Visual Studio ausführen, müssen Sie sich möglicherweise explizit abmelden, damit das Beispiel funktioniert.
>- Wenn Sie eine Ausnahme erhalten, die angibt, dass der Benutzer nicht authentifiziert ist, müssen Sie möglicherweise den Schritt [Hinzufügen des verbundenen Diensts](#add-the-connected-service) wiederholen.
    

## <a name="explore-the-code"></a>Untersuchen des Codes

Sie können nun mithilfe von Visual Studio 2017 eine Verbindung mit Ihren Diensten herstellen und diese konfigurieren. Im Startbeispiel werden das Gerüst und die Verweise für Sie erstellt.  

Das Startbeispiel umfasst die folgenden Dateien:

- [Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs): Authentifiziert den aktuellen Benutzer und initialisiert den Tokencache des Beispiels.

- Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs): Enthält die Tokeninformationen des Benutzers. Sie können diesen durch Ihren eigenen benutzerdefinierten Tokencache ersetzen. Weitere Informationen finden Sie unter [Zwischenspeichern von Zugriffstoken in einer mehrinstanzenfähigen Anwendung](https://azure.microsoft.com/de-DE/documentation/articles/guidance-multitenant-identity-token-cache/).

- Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs): Implementiert die lokale IAuthProvider-Schnittstelle und ruft ein Zugriffstoken ab. 

- Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs): Initialisiert den **GraphServiceClient** aus der [Microsoft Graph .NET-Clientbibliothek](https://github.com/microsoftgraph/msgraph-sdk-dotnet), die für die Interaktion mit Microsoft Graph verwendet wird.

- Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs): Enthält Methoden, die den **GraphServiceClient** zum Erstellen und Senden von Aufrufen des Microsoft Graph-Diensts und zum Verarbeiten der Antwort verwenden.

- Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml): Enthält die Benutzeroberfläche für das Beispiel. 


## <a name="need-help"></a>Benötigen Sie Hilfe?

Wenn Sie Hilfe benötigen, veröffentlichen Sie Ihre Fragen in [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Taggen Sie Ihren Beitrag mit {microsoftgraph}.

