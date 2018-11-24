# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="2b057-101">Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern</span><span class="sxs-lookup"><span data-stu-id="2b057-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="2b057-102">Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients.</span><span class="sxs-lookup"><span data-stu-id="2b057-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="2b057-103">Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="2b057-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="2b057-104">Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2b057-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="2b057-105">Weitere Informationen zum Abonnieren und behandeln eingehende Benachrichtigungen finden Sie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](../../../concepts/webhooks.md), einschließlich.</span><span class="sxs-lookup"><span data-stu-id="2b057-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="2b057-106">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="2b057-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="2b057-107">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2b057-107">Messages</span></span>
- <span data-ttu-id="2b057-108">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="2b057-108">Events</span></span>
- <span data-ttu-id="2b057-109">Kontakte</span><span class="sxs-lookup"><span data-stu-id="2b057-109">Contacts</span></span>
- <span data-ttu-id="2b057-110">Benutzer</span><span class="sxs-lookup"><span data-stu-id="2b057-110">Users</span></span>
- <span data-ttu-id="2b057-111">Gruppen</span><span class="sxs-lookup"><span data-stu-id="2b057-111">Groups</span></span>
- <span data-ttu-id="2b057-112">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="2b057-112">Group conversations</span></span>
- <span data-ttu-id="2b057-113">OneDrive, einschließlich SharePoint-Websites zugeordneten Laufwerke freigegebenen Inhalt</span><span class="sxs-lookup"><span data-stu-id="2b057-113">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="2b057-114">Persönliche OneDrive-Ordner von Benutzern</span><span class="sxs-lookup"><span data-stu-id="2b057-114">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="2b057-115">Sicherheitshinweise</span><span class="sxs-lookup"><span data-stu-id="2b057-115">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="2b057-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b057-116">Permissions</span></span>

<span data-ttu-id="2b057-p102">In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription_post_subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="2b057-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="2b057-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b057-121">Permission type</span></span>                        | <span data-ttu-id="2b057-122">Unterstützte Ressourcentypen in v1.0</span><span class="sxs-lookup"><span data-stu-id="2b057-122">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="2b057-123">Delegiert – Geschäfts-, Schul- oder Unikonto</span><span class="sxs-lookup"><span data-stu-id="2b057-123">Delegated - work or school account</span></span>     | <span data-ttu-id="2b057-124">[wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Nachricht][], [Benachrichtigung][]</span><span class="sxs-lookup"><span data-stu-id="2b057-124">[contact][], [conversation][], [drive][], [event][], [message][], [alert][]</span></span> |
| <span data-ttu-id="2b057-125">Delegiert – persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="2b057-125">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="2b057-126">Keine</span><span class="sxs-lookup"><span data-stu-id="2b057-126">None</span></span>                                                             |
| <span data-ttu-id="2b057-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b057-127">Application</span></span>                            | <span data-ttu-id="2b057-128">[wenden Sie sich an][], [Unterhaltung][], [Ereignis][], [Nachricht][], [Benachrichtigung][]</span><span class="sxs-lookup"><span data-stu-id="2b057-128">[contact][], [conversation][], [event][], [message][], [alert][]</span></span>           |

## <a name="see-also"></a><span data-ttu-id="2b057-129">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2b057-129">See also</span></span>

- [<span data-ttu-id="2b057-130">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2b057-130">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="2b057-131">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="2b057-131">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="2b057-132">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="2b057-132">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="2b057-133">Update subscription</span><span class="sxs-lookup"><span data-stu-id="2b057-133">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="2b057-134">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="2b057-134">Delete subscription</span></span>](../api/subscription_delete.md)

[Kontakt]: ./contact.md
[contact]: ./contact.md
[Unterhaltung]: ./conversation.md
[conversation]: ./conversation.md
[Laufwerk]: ./drive.md
[drive]: ./drive.md
[Ereignis]: ./event.md
[event]: ./event.md
[Nachricht]: ./message.md
[message]: ./message.md
[Benachrichtigung]: ./alert.md
[alert]: ./alert.md