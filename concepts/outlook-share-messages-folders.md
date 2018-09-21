# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="aebe1-101">Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner</span><span class="sxs-lookup"><span data-stu-id="aebe1-101">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="aebe1-102">Mit Outlook können Benutzer Ordner freigeben und den Zugriff auf einzelne Kontaktordner „lesen“, „erstellen“, „ändern“ oder „löschen“ aktivieren.</span><span class="sxs-lookup"><span data-stu-id="aebe1-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="aebe1-103">Outlook ermöglicht es einem Kunden auch, einen anderen Benutzer zu delegieren, um im Auftrag des Kunden zu handeln und auf bestimmte Ordner oder das gesamte Postfach des Kunden zuzugreifen. Dies wird in Outlook auch als „Delegierung“ bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="aebe1-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="aebe1-104">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Nachrichten in E-Mail-Ordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst.</span><span class="sxs-lookup"><span data-stu-id="aebe1-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="aebe1-105">Die Unterstützung gilt auch für Ordner, die delegiert wurden.</span><span class="sxs-lookup"><span data-stu-id="aebe1-105">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="aebe1-106">Beispielsweise hat Garth John Lesezugriff auf den Posteingang von Garth erteilt.</span><span class="sxs-lookup"><span data-stu-id="aebe1-106">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="aebe1-107">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Mail und Posteingang zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="aebe1-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="aebe1-108">Abrufen einer Nachricht im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="aebe1-108">Get a message in the shared folder</span></span>

<span data-ttu-id="aebe1-109">Sie können eine bestimmte Nachricht in Garths Posteingang abrufen:</span><span class="sxs-lookup"><span data-stu-id="aebe1-109">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="aebe1-110">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und die [message](../api-reference/v1.0/resources/message.md)-Instanz mit der ID `{id}` aus Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="aebe1-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="aebe1-111">Abrufen aller Nachrichten im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="aebe1-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="aebe1-112">So rufen Sie alle Nachrichten in Garths Posteingang ab:</span><span class="sxs-lookup"><span data-stu-id="aebe1-112">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="aebe1-113">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine Sammlung der [message](../api-reference/v1.0/resources/message.md)-Instanzen in Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="aebe1-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="aebe1-114">Abrufen des freigegebenen Ordners</span><span class="sxs-lookup"><span data-stu-id="aebe1-114">Get the shared folder</span></span>

<span data-ttu-id="aebe1-115">Rufen Sie den Ordner (Posteingang) ab, den Garth für John freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="aebe1-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="aebe1-116">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine [mailFolder](../api-reference/v1.0/resources/mailfolder.md)-Instanz, die den Ordner „Posteingang“ von Garth darstellt.</span><span class="sxs-lookup"><span data-stu-id="aebe1-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="aebe1-117">Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Posteingang delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="aebe1-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="aebe1-118">Wenn Garth weder seinen Kalender für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aebe1-118">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="aebe1-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="aebe1-119">Next steps</span></span>

<span data-ttu-id="aebe1-120">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="aebe1-120">Find out more about:</span></span>

- [<span data-ttu-id="aebe1-121">Gründe für die Integration in Outlook-Mail</span><span class="sxs-lookup"><span data-stu-id="aebe1-121">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="aebe1-122">[Verwenden der Mail-API](../api-reference/v1.0/resources/mail_api_overview.md) und [Anwendungsfälle](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) für diese in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="aebe1-122">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>