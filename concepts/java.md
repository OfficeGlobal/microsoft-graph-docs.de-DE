# <a name="get-started-with-microsoft-graph-in-a-java-app"></a>Erste Schritte mit Microsoft Graph in einer Java-App

In diesem Artikel wird das [console-java-connect-sample](https://github.com/microsoftgraph/console-java-connect-sample) verwendet, um Sie durch das Senden von E-Mails über Microsoft Graph von einer Java-Konsolenanwendung aus zu führen. In dem Artikel wird der Code veranschaulicht, den Sie zu Ihrer Java-App hinzufügen müssen, damit Sie die Microsoft Graph-API verwenden können. Die App greift mithilfe des [Microsoft Graph-SDKs für Java](https://github.com/microsoftgraph/msgraph-sdk-java) auf Microsoft Graph zu.

## <a name="choose-an-authentication-library"></a>Auswählen einer Authentifizierungsbibliothek

In Microsoft Graph wurden die Standards OAuth 2.0 and Open ID Connect eingeführt, mit denen Sie eine Auswahl aus vielen verfügbaren OAuth2-Java-Bibliotheken (Open Source) treffen können. Das Azure AD-Team empfiehlt die Verwendung von [ScribeJava](https://github.com/scribejava/scribejava), eine einfache OAuth2-Bibliothek für Java.

Das Beispiel implementiert den Fluss zum Erteilen eines Autorisierungscodes, was die richtige Wahl für ein Clientauthentifizierungsszenario, einen Benutzer und einen OAuth2-fähigen Endpunkt ist. In Server-zu-Server-Java-Anwendungen in der Produktion wird der Fluss zu Autorisierung von Clientanmeldeinformationen verwendet. **ScribeJava** verarbeitet beide Autorisierungsflüsse. Damit dieses Beispiel einfach registriert, authentifiziert und ausgeführt werden kann, wird der einfachste Fluss veranschaulicht.

Bevor Ihre App Aufrufe von Microsoft Graph tätigen kann, muss die App ein Zugriffstoken aus Azure Active Directory (Azure AD) abrufen. Dieses Token muss bei jedem Aufruf von Microsoft Graph in einem HTTP-Authentifizierungsheader vorhanden sein. Das **Microsoft Graph-SDK** übernimmt das Einfügen des Headers und das Hinzufügen des Tokens für jeden Aufruf, wenn Sie [IAuthenticationProvider](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/authentication/IAuthenticationProvider.java) implementieren. **ScribeJava** verarbeitet die Authentifizierung und das Abrufen eines Zugriffstokens. Ihre App stellt das Zugriffstoken für das Microsoft Graph-SDK über die **IAuthenticationProvider**-Schnittstelle bereit.

## <a name="install-and-run-the-sample"></a>Installieren und Ausführen des Beispiels

Anweisungen zum Installieren und Konfigurieren der Beispiel-App finden Sie in der [Infodatei](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md) im **console-java-connect-sample**-Repository auf GitHub. Sie können das Beispiel klonen und den Code in Ihrer bevorzugten Java-IDE mithilfe des folgenden Befehls zum Klonen des Repositorys durchlaufen:

```
git@github.com:microsoftgraph/console-java-connect-sample.git
```

Wenn Sie [Java Connect-Konsolen-App registrieren](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#register-your-app), weisen Sie dem Beispiel delegierte Bereiche (Berechtigungen) zu. Achten Sie dabei auf Bereiche wie in der folgenden Abbildung dargestellt:

![Berechtigungen des Java Connect-Konsolenbeispiels](../concepts/images/console-java-connnect-sample-permissions.JPG)

Nachdem Sie die Anwendung registriert und [das Beispiel](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#configure-your-app) für die **Anwendungs-ID konfiguriert** haben, die Sie von der Anwendungsregistrierung erhalten, können Sie das Beispiel ausführen.

## <a name="console-java-connect-code"></a>Code für Console-Java-Connect 

Bevor Sie sich den logischen Fluss des Beispiels ansehen, sollten Sie sich einige Minuten Zeit nehmen, um mehr über die [Struktur des Beispielprojekts](#sample-project-structure) zu erfahren. Wenn Sie fertig sind, können Sie sich die Logik in dem Beispiel näher ansehen:


   
### <a name="walk-through-the-code"></a>Durchlaufen des Codes
Wir werden uns den Beispielcode auf einer allgemeinen Ebene ansehen und dann die Details des Erstellens und Sendens einer E-Mail näher betrachten.

#### <a name="the-user-experience"></a>Die Benutzererfahrung

In diesem Abschnitt wird ein Blick auf die Logik geworfen, die die Anwendung startet und Ihnen dann die Beispielausgabe anzeigt, die dem Benutzer angezeigt wird, wenn er das Beispiel ausführt.

Die statische Methode [PublicClient](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/PublicClient.java) **main** erstellt eine Instanz von **PublicClient** und startet dann den Anmelde- und Authentifizierungsprozess.  

[AuthenticationManager](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager) stellt eine einzelne Instanz bereit, die verwendet wird, um den Benutzer mit Microsoft Graph zu verbinden. **AuthenticationManager** macht ein **Zugriffstoken** als Zeichenfolgeneigenschaft verfügbar. Das Zugriffstoken wird von **Azure AD** zurückgegeben, wenn der Benutzer authentifiziert ist, und gibt der Beispielberechtigung Zugriff auf angeforderte Microsoft Graph-Ressourcen. 

Die **PublicClient.startSendMail**-Methode führt die folgenden Schritte aus:

- Erstellt eine neue Instanz der [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java)-Klasse. 
- Ruft **GraphSendMail.getMeUser()** auf, um das **Azure AD**-Profil des aktuellen Benutzers zurückzugeben, damit das Beispielkonsolenobjekt die Aufforderungen personalisieren kann, die für den Benutzer angezeigt werden. 
- In der Konsole wird Folgendes angezeigt:

   `Hello, Laura Steele. Would you like to send an email to yourself or someone else?`

   `Enter the address to which you'd like to send a message. If you enter nothing, the message will go to your address`

- Ruft die **GraphSendMail.sendMail**-Methode auf, die die Benutzereingabe verwendet. Wenn eine E-Mail-Adresse bereitgestellt wird, sendet **sendMail** eine Nachricht an diese Adresse. Andernfalls wird die Nachricht an den aktuellen Benutzer gesendet. 

- Fordert den Benutzer auf, eine weitere E-Mail zu senden oder die Konsolen-App zu schließen.

   `Email sent!`

   `Want to send another message? Type 'y' for yes and any other key to exit.`

#### <a name="the-send-mail-logic"></a>Die Logik zum Senden von E-Mails

Die Logik zum Senden von E-Mails besteht aus den folgenden Schritten:



1. **Abrufen des Profilbilds**:<br/> Ruft **GraphServiceController.getUserProfilePicture()** auf, um ein Array von Bytes abzurufen, das das Profilbild des **Azure AD**-Benutzers darstellt, der sich bei dem Beispiel angemeldet hat.

   **Der API-Aufruf**

```java
            photoStream = mGraphServiceClient
                    .me()
                    .photo()
                    .content()
                    .buildRequest()
                    .get();

```
2. **Hochladen des Bilds in OneDrive**:
<br/>Ruft **GraphServiceController.uploadPictureToOneDrive(bytes)** auf, um das Profilbild im OneDrive-Stammordner des Benutzers zu veröffentlichen. Ein **DriveItem**-Objekt des Microsoft Graph-SDKs wird zurückgegeben. 

   **Der API-Aufruf**
```java
            driveItem = mGraphServiceClient
                    .me()
                    .drive()
                    .root()
                    .itemWithPath("me2.png")
                    .content()
                    .buildRequest()
                    .put(picture);

```
3. **Abrufen des OneDrive-Freigabelinks für das Bild**:<br/>Ruft **GraphServiceController.getPermissionSharingLink** auf, um einen neuen Freigabelink zu erstellen. Ein **Permission**-Objekt des Microsoft Graph-SDKs wird zurückgegeben.

   **Der API-Aufruf**
```java
            permission = mGraphServiceClient
                    .me()
                    .drive()
                    .items(id)
                    .createLink("view", "organization")
                    .buildRequest()
                    .post();

```
4. **Ersetzen des Inhalts des Anchortags der HTML-Vorlage** durch die **WebUrl** für den Freigabelink im vorherigen Schritt. 
> **Hinweis:** Der Text der von der Anwendung gesendeten Nachricht wird aus einer HTML-Vorlage erstellt, die in [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java) als statische Zeichenfolge gespeichert wird. Nach dem Senden enthält der Text der Nachricht einen öffentlichen Freigabe-Hyperlink zu einem Bild, das das Beispiel in den OneDrive-Stammordner hochlädt. 
5. **Erstellen eines Nachrichtenentwurfs**: <br/>Ruft **GraphServiceController.createDraftMail** auf und übergibt die E-Mail-Adresse des Empfängers, den Betreffstext sowie die aktualisierte HTML-Vorlage. Es wird eine Entwurfsnachricht erstellt, die an den Entwurfsordner des Benutzers gesendet wird.

   **Der API-Aufruf**
```java
            message = mGraphServiceClient
                    .me()
                    .messages()
                    .buildRequest()
                    .post(message);

```
6. **Anfügen eines Bilds an die Entwurfsnachricht**: <br/>Ruft **GraphServiceController.addPictureToDraftMessage** auf, um die Entwurfsnachricht abzurufen und das Bild zu der Nachricht als Objektanlage hinzuzufügen.

   **Der API-Aufruf**
```java
            FileAttachment fileAttachment = new FileAttachment();
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment";
            fileAttachment.contentBytes = attachementBytes;
            fileAttachment.name = "me.png";
            fileAttachment.size = attachementBytes.length;
            fileAttachment.isInline = false;
            fileAttachment.id = "my profile picture";

            attachment = mGraphServiceClient
                    .me()
                    .messages(messageId)
                    .attachments()
                    .buildRequest()
                    .post(fileAttachment);

```
7. **Senden der Entwurfsnachricht**:<br/>Ruft **GraphServiceController.sendDraftMessage** auf, um die aktualisierte Entwurfsnachricht an den gewünschten Empfänger zu senden.

   **Der API-Aufruf**
```java
            mGraphServiceClient
                    .me()
                    .mailFolders("Drafts")
                    .messages(messageId)
                    .send()
                    .buildRequest()
                    .post();

```



### <a name="sample-project-structure"></a>Beispielprojektstruktur

### <a name="connect-package"></a>connect-Paket
Dieses Paket enthält die Logik des OAuth2-Authentifizierunsflusses und die Konfiguration, die Sie aktualisieren.

- [AuthenticationManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager.java): Diese Klasse importiert die **ScribeJava**-Objekte, die für den Fluss der Autorisierungscodegenehmigung verwendet werden.
- [Constants.Java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java): Speichert öffentliche statische Zeichenfolgen zur Bereitstellung von Werten im Zusammenhang mit der App-Registrierung und die Vorlage für die E-Mail-Nachricht, die die Anwendung sendet.
- [Debug.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Debug.java): Öffentliches Flag auf Debugebene. Legen Sie diesen Wert so fest, dass das Protokollierungsverhalten der Beispiel-App geändert wird.
- [DebugLogger.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/DebugLogger.java): Protokollierungsdienstprogramm, das Informationen gemäß der festgelegten Debugebene in die Konsole schreibt.
- [IConnectCallback](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/IConnectCallback.java): Definiert die Rückrufmethode, die Sie beim Aufrufen der asynchronen Überladung der **ScribeJava.getAccessToken**-Methode verwenden würden.
- [SendMailException](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/SendMailException.java): Eine Klasse, die von **Exception** abgeleitet wird und Microsoft Graph-spezifische Ausnahmeinformationen kapselt. Klassen im **GraphSendMail**-Paket können Sie diese Art von Ausnahme auslösen.

### <a name="msgraph-package"></a>msgraph-Paket

Dieses Paket enthält die gesamte Logik, die Aufrufe von Microsoft Graph ausführt.

- [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java): Verkettet Aufrufe in **GraphServiceController** (eine Beispielhelferklasse der Microsoft Graph-API) zum Erstellen und Senden einer E-Mail-Nachricht mit einer Bildanlage.
- [GraphServiceClientManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceClientManager.java): Instanziiert den [GraphServiceClient](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/requests/extensions/GraphServiceClient.java) des Microsoft Graph-SDKs und fügt ein Zugriffstoken mit allen ausgehenden API-Aufrufen am Microsoft Graph-Endpunkt hinzu.

- [GraphServiceController.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceController.java): Verwendet das Microsoft Graph-SDK für Aufrufe des **GraphServiceClient**. Anrufe umfassen Folgendes:

   - **createDraftMail**: Erstellt eine Entwurfs-E-Mail-Nachricht und speichert diese im Entwurfsordner.
   - **sendNewMessageAsync**: Erstellt und sendet eine E-Mail-Nachricht.
   - **AddPictureToDraftMessage**: Stellt eine Dateianlage in einer Entwurfsnachricht anhand der Nachrichten-ID bereit.
   - **addAttachmentToDraftAsync**: Fügt eine Anlage zu der Entwurfsnachricht hinzu.
   - **sendDraftMessage**: Sendet eine Nachricht aus dem Entwurfsordner.
   - **getDraftMessage**: Ruft eine Nachricht aus der Nachrichtensammlung des Benutzers anhand der Nachrichten-ID ab.
   - **getUser**: Ruft den lokalen Benutzer ab, der beim Microsoft Graph-API-Endpunkt registriert ist.
   - **getUserProfilePicture**: Ruft das Profilbild des angemeldeten Benutzers aus Microsoft Graph ab.
   - **uploadPictureToOneDrive**: Lädt ein Bild als Bytearray in den OneDrive-Stammordner des Benutzers hoch.
   - **getPermissionSharingLink**: Fordert OneDrive auf, einen öffentlichen Freigabelink zu einem in OneDrive gespeicherten Bild zu erstellen.

## <a name="other-microsoft-graph-samples"></a>Weitere Beispiele für Microsoft Graph

Wenn Sie nach einem bestimmten Beispiel suchen, teilen Sie uns das mit, indem Sie uns [ein Problem übermitteln](https://github.com/microsoftgraph/console-java-connect-sample/issues). Wir schätzen Ihr Feedback zu allen Microsoft Graph-Szenarien, die Sie in Java entwickeln möchten!

Die Microsoft Graph-API ist eine leistungsfähige einheitliche API, die für die Interaktion mit beliebigen Microsoft-Daten verwendet werden kann. Schauen Sie sich die [Entwicklerdokumentationen](https://developer.microsoft.com/de-DE/graph/docs/concepts/overview) oder den [Graph-Explorer](https://developer.microsoft.com/de-DE/graph/graph-explorer) an, um sich von den Vorteilen von Microsoft Graph zu überzeugen.
