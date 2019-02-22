---
title: Verwenden der Microsoft Graph-API zum Abrufen von Änderungsbenachrichtigungen
description: Die Microsoft Graph-REST-API verwendet einen webhook-Mechanismus, um Änderungsbenachrichtigungen an Clients zu übermitteln. Ein Client ist ein Webdienst, der seine eigene URL für den Empfang von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um Ihren Status bei Änderungen zu aktualisieren. Weitere Informationen, einschließlich des Abonnierens und behandeln eingehender Benachrichtigungen, finden Sie unter Einrichten von Benachrichtigungen für Änderungen in Benutzerdaten.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1d7a3d868ffc640f7659623942ac102575fb94fc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151492"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="45548-106">Verwenden der Microsoft Graph-API zum Abrufen von Änderungsbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="45548-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45548-107">Die Microsoft Graph-REST-API verwendet einen webhook-Mechanismus, um Änderungsbenachrichtigungen an Clients zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="45548-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="45548-108">Ein Client ist ein Webdienst, der seine eigene URL für den Empfang von Benachrichtigungen konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="45548-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="45548-109">Client-Apps verwenden Benachrichtigungen, um Ihren Status bei Änderungen zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="45548-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="45548-110">Weitere Informationen, einschließlich des Abonnierens und behandeln eingehender Benachrichtigungen, finden Sie unter [Einrichten von Benachrichtigungen für Änderungen in Benutzerdaten](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="45548-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="45548-111">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="45548-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="45548-112">Outlook- [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="45548-112">Outlook [message][]</span></span>
- <span data-ttu-id="45548-113">Outlook- [Ereignis][]</span><span class="sxs-lookup"><span data-stu-id="45548-113">Outlook [event][]</span></span>
- <span data-ttu-id="45548-114">Persönlicher Outlook- [Kontakt][]</span><span class="sxs-lookup"><span data-stu-id="45548-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="45548-115">[user][]</span><span class="sxs-lookup"><span data-stu-id="45548-115">[user][]</span></span>
- <span data-ttu-id="45548-116">[Gruppe][]</span><span class="sxs-lookup"><span data-stu-id="45548-116">[group][]</span></span>
- <span data-ttu-id="45548-117">Office 365-Gruppen [Unterhaltung][]</span><span class="sxs-lookup"><span data-stu-id="45548-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="45548-118">Inhalt innerhalb der Hierarchie eines _beliebigen Ordners_ [DriveItem][] auf persönliche OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="45548-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="45548-119">Inhalt in der Hierarchie des _Stammordners_ [driveItem][] auf OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="45548-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="45548-120">Sicherheits [Warnung][]</span><span class="sxs-lookup"><span data-stu-id="45548-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="45548-121">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45548-121">Permissions</span></span>

<span data-ttu-id="45548-p103">In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription-post-subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="45548-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="45548-126">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45548-126">Permission type</span></span>                        | <span data-ttu-id="45548-127">Unterstützte Ressourcentypen</span><span class="sxs-lookup"><span data-stu-id="45548-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="45548-128">Delegiert – Geschäfts-, Schul- oder Unikonto</span><span class="sxs-lookup"><span data-stu-id="45548-128">Delegated - work or school account</span></span>     | <span data-ttu-id="45548-129">[Warnung][], [Kontakt][], unter [Haltung][], [driveItem][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][]</span><span class="sxs-lookup"><span data-stu-id="45548-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="45548-130">Delegiert – persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="45548-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="45548-131">[Kontakt][], [driveItem][], [Ereignis][], [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="45548-131">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="45548-132">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45548-132">Application</span></span>                            | <span data-ttu-id="45548-133">[Alert][], [Contact][], [driveItem][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][]</span><span class="sxs-lookup"><span data-stu-id="45548-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="45548-134">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="45548-134">See also</span></span>

- [<span data-ttu-id="45548-135">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="45548-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="45548-136">Listen Abonnements</span><span class="sxs-lookup"><span data-stu-id="45548-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="45548-137">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="45548-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="45548-138">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="45548-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="45548-139">Update subscription</span><span class="sxs-lookup"><span data-stu-id="45548-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="45548-140">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="45548-140">Delete subscription</span></span>](../api/subscription-delete.md)

[Kontakt]: ./contact.md
[contact]: ./contact.md
[Unterhaltung]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[Warnung]: ./alert.md
[alert]: ./alert.md
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
