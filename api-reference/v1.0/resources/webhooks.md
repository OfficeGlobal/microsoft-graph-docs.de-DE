---
title: Verwenden der Microsoft Graph-API, um Änderungsbenachrichtigungen zu erhalten
description: Die Microsoft Graph-REST-API verwendet einen Webhook-Mechanismus zum Übermitteln von Änderungsbenachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren. Weitere Informationen, einschließlich der Vorgehensweise zum Abonnieren und Behandeln eingehender Benachrichtigungen, finden Sie unter "Einrichten von Benachrichtigungen für Änderungen an Benutzerdaten".
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 60def6f31ac13ad5417ad3d00e48e700550f6efe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159374"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="777d0-106">Verwenden der Microsoft Graph-API, um Änderungsbenachrichtigungen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="777d0-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="777d0-107">Die Microsoft Graph-REST-API verwendet einen Webhook-Mechanismus zum Übermitteln von Änderungsbenachrichtigungen an Clients.</span><span class="sxs-lookup"><span data-stu-id="777d0-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="777d0-108">Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="777d0-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="777d0-109">Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="777d0-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="777d0-110">Weitere Informationen, einschließlich der Vorgehensweise zum Abonnieren und Behandeln eingehender Benachrichtigungen, finden Sie unter [Einrichten von Benachrichtigungen für Änderungen an Benutzerdaten](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="777d0-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="777d0-111">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="777d0-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="777d0-112">Outlook-[Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="777d0-112">Outlook [message][]</span></span>
- <span data-ttu-id="777d0-113">Outlook-[Ereignis][]</span><span class="sxs-lookup"><span data-stu-id="777d0-113">Outlook [event][]</span></span>
- <span data-ttu-id="777d0-114">Persönlicher Outlook-[Kontakt][]</span><span class="sxs-lookup"><span data-stu-id="777d0-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="777d0-115">[Benutzer][]</span><span class="sxs-lookup"><span data-stu-id="777d0-115">[user][]</span></span>
- <span data-ttu-id="777d0-116">[Gruppe][]</span><span class="sxs-lookup"><span data-stu-id="777d0-116">[group][]</span></span>
- <span data-ttu-id="777d0-117">Office 365-[Gruppenunterhaltung][]</span><span class="sxs-lookup"><span data-stu-id="777d0-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="777d0-118">Inhalt in der Hierarchie des [driveItem][]-Objekts eines _beliebigen Ordners_ auf dem persönlichen OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="777d0-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="777d0-119">Inhalt in der Hierarchie des [driveItem][]-Objekts eines _Stammordners_ auf OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="777d0-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="777d0-120">[Sicherheitswarnung][]</span><span class="sxs-lookup"><span data-stu-id="777d0-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="777d0-121">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="777d0-121">Permissions</span></span>

<span data-ttu-id="777d0-p103">In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription-post-subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="777d0-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="777d0-126">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="777d0-126">Permission type</span></span>                        | <span data-ttu-id="777d0-127">Unterstützte Ressourcentypen</span><span class="sxs-lookup"><span data-stu-id="777d0-127">Supported resource types in v1.0</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="777d0-128">Delegiert – Geschäfts-, Schul- oder Unikonto</span><span class="sxs-lookup"><span data-stu-id="777d0-128">Delegated - work or school account</span></span>     | <span data-ttu-id="777d0-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span><span class="sxs-lookup"><span data-stu-id="777d0-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="777d0-130">Delegiert – persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="777d0-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="777d0-131">[contact][], [driveItem][], [event][], [message][]</span><span class="sxs-lookup"><span data-stu-id="777d0-131">[contact][], [conversation][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="777d0-132">Anwendung</span><span class="sxs-lookup"><span data-stu-id="777d0-132">Application</span></span>                            | <span data-ttu-id="777d0-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span><span class="sxs-lookup"><span data-stu-id="777d0-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|


## <a name="see-also"></a><span data-ttu-id="777d0-134">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="777d0-134">See also</span></span>

- [<span data-ttu-id="777d0-135">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="777d0-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="777d0-136">Abonnements auflisten</span><span class="sxs-lookup"><span data-stu-id="777d0-136">List current subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="777d0-137">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="777d0-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="777d0-138">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="777d0-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="777d0-139">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="777d0-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="777d0-140">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="777d0-140">Delete subscription</span></span>](../api/subscription-delete.md)

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[Alert]: ./alert.md
