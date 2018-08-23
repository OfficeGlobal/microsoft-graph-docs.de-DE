# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="709e8-101">Verwenden der Microsoft Graph-API zum Erhalten von Änderungsbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="709e8-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="709e8-102">Die Microsoft Graph-REST-API sendet mithilfe eines Webhook-Mechanismuses Benachrichtigungen an Clients.</span><span class="sxs-lookup"><span data-stu-id="709e8-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="709e8-103">Ein Client ist ein Web-Service, der seine eigene URL konfiguriert, um Benachrichtigungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="709e8-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="709e8-104">Client-Apps nutzen Benachrichtigungen, um bei Änderung ihren Status zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="709e8-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="709e8-105">Weitere Informationen zum Abonnieren und Verwalten von eingehenden Benachrichtigungen finden Sie unter [Benachrichtigungen für Änderungen bei Benutzerdaten festlegen](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="709e8-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="709e8-106">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="709e8-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="709e8-107">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="709e8-107">Messages</span></span>
- <span data-ttu-id="709e8-108">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="709e8-108">Events</span></span>
- <span data-ttu-id="709e8-109">Kontakte</span><span class="sxs-lookup"><span data-stu-id="709e8-109">Contacts</span></span>
- <span data-ttu-id="709e8-110">Benutzer</span><span class="sxs-lookup"><span data-stu-id="709e8-110">Users</span></span>
- <span data-ttu-id="709e8-111">Gruppen</span><span class="sxs-lookup"><span data-stu-id="709e8-111">Groups</span></span>
- <span data-ttu-id="709e8-112">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="709e8-112">Group conversations</span></span>
- <span data-ttu-id="709e8-113">Inhalten, die in OneDrive freigegeben werden, einschließlich der diesen SharePoint-Websites zugeordneten Laufwerke</span><span class="sxs-lookup"><span data-stu-id="709e8-113">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="709e8-114">Persönliche OneDrive-Order von Benutzern</span><span class="sxs-lookup"><span data-stu-id="709e8-114">User's personal OneDrive folders</span></span>

## <a name="permissions"></a><span data-ttu-id="709e8-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="709e8-115">Permissions</span></span>

<span data-ttu-id="709e8-p102">In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription_post_subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="709e8-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="709e8-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="709e8-120">Permission type</span></span>                        | <span data-ttu-id="709e8-121">Unterstützte Ressourcentypen in v1.0</span><span class="sxs-lookup"><span data-stu-id="709e8-121">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="709e8-122">Delegiert – Geschäfts-, Schul- oder Unikonto</span><span class="sxs-lookup"><span data-stu-id="709e8-122">Delegated - work or school account</span></span>     | <span data-ttu-id="709e8-123">[Kontakt][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="709e8-123">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="709e8-124">Delegiert – persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="709e8-124">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="709e8-125">Keine</span><span class="sxs-lookup"><span data-stu-id="709e8-125">None</span></span>                                                             |
| <span data-ttu-id="709e8-126">Anwendung</span><span class="sxs-lookup"><span data-stu-id="709e8-126">Application</span></span>                            | <span data-ttu-id="709e8-127">[Kontakt][], [Unterhaltung][], [Ereignis][], [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="709e8-127">[contact][], [conversation][], [event][], [message][]</span></span>            |

## <a name="see-also"></a><span data-ttu-id="709e8-128">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="709e8-128">See also</span></span>

- [<span data-ttu-id="709e8-129">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="709e8-129">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="709e8-130">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="709e8-130">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="709e8-131">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="709e8-131">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="709e8-132">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="709e8-132">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="709e8-133">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="709e8-133">Delete subscription</span></span>](../api/subscription_delete.md)

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
