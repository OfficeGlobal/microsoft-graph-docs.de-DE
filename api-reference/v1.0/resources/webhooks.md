---
title: Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern
description: Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert. Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren. Weitere Einzelheiten, einschließlich das Abonnieren und behandeln eingehende Benachrichtigungen Set finden Sie unter Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten.
ms.openlocfilehash: c7d468b7c5064911d27d3a93bc3160d03c2a4dc3
ms.sourcegitcommit: 02ead22efd4f10cd50f89c9f5aa3b6dfda96aeec
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/01/2018
ms.locfileid: "27123945"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="1618f-106">Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern</span><span class="sxs-lookup"><span data-stu-id="1618f-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="1618f-107">Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients.</span><span class="sxs-lookup"><span data-stu-id="1618f-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="1618f-108">Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="1618f-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="1618f-109">Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="1618f-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="1618f-110">Weitere Informationen zum Abonnieren und behandeln eingehende Benachrichtigungen finden Sie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks), einschließlich.</span><span class="sxs-lookup"><span data-stu-id="1618f-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="1618f-111">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="1618f-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="1618f-112">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="1618f-112">Messages</span></span>
- <span data-ttu-id="1618f-113">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="1618f-113">Events</span></span>
- <span data-ttu-id="1618f-114">Kontakte</span><span class="sxs-lookup"><span data-stu-id="1618f-114">Contacts</span></span>
- <span data-ttu-id="1618f-115">Benutzer</span><span class="sxs-lookup"><span data-stu-id="1618f-115">Users</span></span>
- <span data-ttu-id="1618f-116">Gruppen</span><span class="sxs-lookup"><span data-stu-id="1618f-116">Groups</span></span>
- <span data-ttu-id="1618f-117">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="1618f-117">Group conversations</span></span>
- <span data-ttu-id="1618f-118">OneDrive, einschließlich SharePoint-Websites zugeordneten Laufwerke freigegebenen Inhalt</span><span class="sxs-lookup"><span data-stu-id="1618f-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="1618f-119">Persönliche OneDrive-Ordner von Benutzern</span><span class="sxs-lookup"><span data-stu-id="1618f-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="1618f-120">Sicherheitshinweise</span><span class="sxs-lookup"><span data-stu-id="1618f-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="1618f-121">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1618f-121">Permissions</span></span>

<span data-ttu-id="1618f-p103">In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription-post-subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="1618f-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="1618f-126">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1618f-126">Permission type</span></span>                        | <span data-ttu-id="1618f-127">Unterstützten Ressourcentypen</span><span class="sxs-lookup"><span data-stu-id="1618f-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="1618f-128">Delegiert – Geschäfts-, Schul- oder Unikonto</span><span class="sxs-lookup"><span data-stu-id="1618f-128">Delegated - work or school account</span></span>     | <span data-ttu-id="1618f-129">[wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][], [Benachrichtigung][]</span><span class="sxs-lookup"><span data-stu-id="1618f-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="1618f-130">Delegiert – persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="1618f-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="1618f-131">[wenden Sie sich an][], [Laufwerk][], [Ereignis][], [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="1618f-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="1618f-132">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1618f-132">Application</span></span>                            | <span data-ttu-id="1618f-133">[wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][], [Benachrichtigung][]</span><span class="sxs-lookup"><span data-stu-id="1618f-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="1618f-134">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1618f-134">See also</span></span>

- [<span data-ttu-id="1618f-135">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1618f-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="1618f-136">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="1618f-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="1618f-137">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="1618f-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="1618f-138">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="1618f-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="1618f-139">Update subscription</span><span class="sxs-lookup"><span data-stu-id="1618f-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="1618f-140">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="1618f-140">Delete subscription</span></span>](../api/subscription-delete.md)

[Kontakt]: ./contact.md
[contact]: ./contact.md
[Unterhaltung]: ./conversation.md
[conversation]: ./conversation.md
[Laufwerk]: ./drive.md
[drive]: ./drive.md
[Ereignis]: ./event.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[Benutzer]: ./user.md
[user]: ./user.md
[Benachrichtigung]: ./alert.md
[alert]: ./alert.md