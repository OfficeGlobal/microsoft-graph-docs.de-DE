---
title: Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern
description: Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert. Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren. Weitere Einzelheiten, einschließlich das Abonnieren und behandeln eingehende Benachrichtigungen Set finden Sie unter Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten.
localization_priority: Normal
ms.openlocfilehash: 9b1907d37115e21b41a9e957de9b7ae0a32fd311
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816471"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="8665d-106">Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern</span><span class="sxs-lookup"><span data-stu-id="8665d-106">Use the Microsoft Graph API to get change notifications</span></span>

> <span data-ttu-id="8665d-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8665d-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8665d-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8665d-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8665d-109">Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients.</span><span class="sxs-lookup"><span data-stu-id="8665d-109">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="8665d-110">Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="8665d-110">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="8665d-111">Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="8665d-111">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="8665d-112">Weitere Informationen zum Abonnieren und behandeln eingehende Benachrichtigungen finden Sie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks), einschließlich.</span><span class="sxs-lookup"><span data-stu-id="8665d-112">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="8665d-113">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="8665d-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="8665d-114">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="8665d-114">Messages</span></span>
- <span data-ttu-id="8665d-115">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="8665d-115">Events</span></span>
- <span data-ttu-id="8665d-116">Kontakte</span><span class="sxs-lookup"><span data-stu-id="8665d-116">Contacts</span></span>
- <span data-ttu-id="8665d-117">Benutzer</span><span class="sxs-lookup"><span data-stu-id="8665d-117">Users</span></span>
- <span data-ttu-id="8665d-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="8665d-118">Groups</span></span>
- <span data-ttu-id="8665d-119">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="8665d-119">Group conversations</span></span>
- <span data-ttu-id="8665d-120">OneDrive, einschließlich SharePoint-Websites zugeordneten Laufwerke freigegebenen Inhalt</span><span class="sxs-lookup"><span data-stu-id="8665d-120">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="8665d-121">Persönliche OneDrive-Ordner von Benutzern</span><span class="sxs-lookup"><span data-stu-id="8665d-121">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="8665d-122">Sicherheitshinweise</span><span class="sxs-lookup"><span data-stu-id="8665d-122">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="8665d-123">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8665d-123">Permissions</span></span>

<span data-ttu-id="8665d-p104">In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription-post-subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="8665d-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="8665d-128">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8665d-128">Permission type</span></span>                        | <span data-ttu-id="8665d-129">Unterstützten Ressourcentypen</span><span class="sxs-lookup"><span data-stu-id="8665d-129">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="8665d-130">Delegiert – Geschäfts-, Schul- oder Unikonto</span><span class="sxs-lookup"><span data-stu-id="8665d-130">Delegated - work or school account</span></span>     | <span data-ttu-id="8665d-131">[wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][], [Benachrichtigung][]</span><span class="sxs-lookup"><span data-stu-id="8665d-131">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="8665d-132">Delegiert – persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="8665d-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="8665d-133">[wenden Sie sich an][], [Laufwerk][], [Ereignis][], [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="8665d-133">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="8665d-134">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8665d-134">Application</span></span>                            | <span data-ttu-id="8665d-135">[wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][], [Benachrichtigung][]</span><span class="sxs-lookup"><span data-stu-id="8665d-135">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="8665d-136">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="8665d-136">See also</span></span>

- [<span data-ttu-id="8665d-137">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8665d-137">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="8665d-138">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="8665d-138">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="8665d-139">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="8665d-139">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="8665d-140">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="8665d-140">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="8665d-141">Update subscription</span><span class="sxs-lookup"><span data-stu-id="8665d-141">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="8665d-142">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="8665d-142">Delete subscription</span></span>](../api/subscription-delete.md)

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
