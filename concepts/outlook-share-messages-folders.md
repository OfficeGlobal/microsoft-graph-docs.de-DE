# <a name="share-outlook-message-folders-between-users"></a><span data-ttu-id="ba06a-101">Freigeben von Outlook-Nachrichtenordnern zwischen Benutzern</span><span class="sxs-lookup"><span data-stu-id="ba06a-101">Share Outlook message folders between users</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="ba06a-102">In Outlook können Kunden Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner oder das gesamte Postfach gewähren.</span><span class="sxs-lookup"><span data-stu-id="ba06a-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="ba06a-103">Dies wird in Outlook auch als „Delegierung“ bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="ba06a-103">This is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="ba06a-104">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Nachrichten in E-Mail-Ordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst.</span><span class="sxs-lookup"><span data-stu-id="ba06a-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span>

<span data-ttu-id="ba06a-105">Beispielsweise hat Garth John Lesezugriff auf den Posteingang von Garth erteilt.</span><span class="sxs-lookup"><span data-stu-id="ba06a-105">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="ba06a-106">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Mail und Posteingang zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="ba06a-106">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="ba06a-107">Abrufen einer Nachricht im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="ba06a-107">Get a message in the shared folder</span></span>

<span data-ttu-id="ba06a-108">Sie können eine bestimmte Nachricht in Garths Posteingang abrufen:</span><span class="sxs-lookup"><span data-stu-id="ba06a-108">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="ba06a-109">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und die [message](../api-reference/v1.0/resources/message.md)-Instanz mit der ID `{id}` aus Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="ba06a-109">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="ba06a-110">Abrufen aller Nachrichten im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="ba06a-110">Get all messages in the shared folder</span></span>

<span data-ttu-id="ba06a-111">So rufen Sie alle Nachrichten in Garths Posteingang ab:</span><span class="sxs-lookup"><span data-stu-id="ba06a-111">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="ba06a-112">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine Sammlung der [message](../api-reference/v1.0/resources/message.md)-Instanzen in Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="ba06a-112">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="ba06a-113">Abrufen des freigegebenen Ordners</span><span class="sxs-lookup"><span data-stu-id="ba06a-113">Get the shared folder</span></span>

<span data-ttu-id="ba06a-114">Rufen Sie den Ordner (Posteingang) ab, den Garth für John freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="ba06a-114">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="ba06a-115">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine [mailFolder](../api-reference/v1.0/resources/mailfolder.md)-Instanz, die den Ordner „Posteingang“ von Garth darstellt.</span><span class="sxs-lookup"><span data-stu-id="ba06a-115">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="ba06a-116">Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Posteingang delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="ba06a-116">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="ba06a-117">Wenn Garth weder seinen Nachrichtenordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba06a-117">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="ba06a-118">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ba06a-118">Next steps</span></span>

<span data-ttu-id="ba06a-119">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="ba06a-119">Find out more about:</span></span>

- [<span data-ttu-id="ba06a-120">Gründe für die Integration in Outlook-Mail</span><span class="sxs-lookup"><span data-stu-id="ba06a-120">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="ba06a-121">[Verwenden der Mail-API](../api-reference/v1.0/resources/mail_api_overview.md) und [Anwendungsfälle](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) für diese in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="ba06a-121">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>