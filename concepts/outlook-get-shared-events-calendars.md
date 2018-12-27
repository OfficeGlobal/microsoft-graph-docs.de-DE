---
title: Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender
description: In Outlook können Kunden einen Kalender mit anderen Benutzern teilen und sie Ereignisse in diesem Kalender anzeigen oder ändern lassen. Kunden können außerdem eine Stellvertretung für das Handeln in ihrem Auftrag erteilen, um Besprechungsanfragen zu empfangen oder zu beantworten oder um Elemente im Kalender zu erstellen oder zu ändern.
author: angelgolfer-ms
ms.openlocfilehash: ef4de6cedeeb9a5688f250652eef0cd6cd5f5183
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413148"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="daeb5-104">Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender</span><span class="sxs-lookup"><span data-stu-id="daeb5-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="daeb5-105">In Outlook können Kunden einen Kalender mit anderen Benutzern teilen und sie Ereignisse in diesem Kalender anzeigen oder ändern lassen.</span><span class="sxs-lookup"><span data-stu-id="daeb5-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="daeb5-106">Kunden können außerdem eine Stellvertretung für das Handeln in ihrem Auftrag erteilen, um Besprechungsanfragen zu empfangen oder zu beantworten oder um Elemente im Kalender zu erstellen oder zu ändern.</span><span class="sxs-lookup"><span data-stu-id="daeb5-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="daeb5-107">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Ereignissen in Kalendern, die von anderen Benutzern geteilt wurden, sowie das Abrufen der Kalender selbst.</span><span class="sxs-lookup"><span data-stu-id="daeb5-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="daeb5-108">Die Unterstützung gilt auch für Kalender, die delegiert wurden.</span><span class="sxs-lookup"><span data-stu-id="daeb5-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="daeb5-109">Beispielsweise hat Adrian für John seinen Standardkalender freigegeben und John Lesezugriff erteilt.</span><span class="sxs-lookup"><span data-stu-id="daeb5-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="daeb5-110">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Calendars.Read.Shared oder Calendars.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Adrians Standardkalender und auf die Ereignisse in diesem Kalender zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="daeb5-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

> <span data-ttu-id="daeb5-111">**Hinweis** Mithilfe der Freigabeberechtigungen (Calendars.Read.Shared oder Calendars.ReadWrite.Shared) können Sie Ereignisse in einem freigegebenen oder delegierten Kalender lesen oder schreiben.</span><span class="sxs-lookup"><span data-stu-id="daeb5-111">**Note** The sharing permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared) allow you to read or write events in a shared or delegated calendar.</span></span> <span data-ttu-id="daeb5-112">[Das Abonnieren von Änderungsbenachrichtigungen](webhooks.md) wird für Elemente in solchen Ordnern nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="daeb5-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="daeb5-113">Verwenden Sie zum Einrichten von Änderungsbenachrichtigungsabonnements für Ereignisse in einem freigegebenen, delegierten oder einem anderen Benutzer- oder Ressourcenkalender im Mandanten die Berechtigung „Calendars.Read“.</span><span class="sxs-lookup"><span data-stu-id="daeb5-113">To set up change notification subscriptions on events in a shared, delegated, or any other user or resource calendar in the tenant, use the application permission, Calendars.Read.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="daeb5-114">Abrufen eines Ereignisses im freigegebenen Kalender</span><span class="sxs-lookup"><span data-stu-id="daeb5-114">Get an event in the shared calendar</span></span>

<span data-ttu-id="daeb5-115">Sie können ein bestimmtes Ereignis in Adrians freigegebenem Standardkalender abrufen:</span><span class="sxs-lookup"><span data-stu-id="daeb5-115">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="daeb5-116">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und die [event](/graph/api/resources/event?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Adrians Posteingang.</span><span class="sxs-lookup"><span data-stu-id="daeb5-116">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="daeb5-117">Abrufen aller Ereignisse im freigegebenen Kalender</span><span class="sxs-lookup"><span data-stu-id="daeb5-117">Get all the events in the shared calendar</span></span>

<span data-ttu-id="daeb5-118">Rufen Sie alle Ereignisse im Standardkalender ab, den Adrian mit John geteilt hat:</span><span class="sxs-lookup"><span data-stu-id="daeb5-118">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="daeb5-119">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine Sammlung der [event](/graph/api/resources/event?view=graph-rest-1.0)-Instanzen in Adrians Standardkalender.</span><span class="sxs-lookup"><span data-stu-id="daeb5-119">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="daeb5-120">Abrufen des freigegebenen Kalenders</span><span class="sxs-lookup"><span data-stu-id="daeb5-120">Get the shared calendar</span></span>

<span data-ttu-id="daeb5-121">Rufen Sie den Standardkalender ab, den Adrian mit John geteilt hat.</span><span class="sxs-lookup"><span data-stu-id="daeb5-121">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="daeb5-122">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine [calendar](/graph/api/resources/calendar?view=graph-rest-1.0)-Instanz, die Adrians Standardordner darstellt.</span><span class="sxs-lookup"><span data-stu-id="daeb5-122">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="daeb5-123">Dieselben GET-Funktionen würden gelten, wenn Adrian an John weiteren Zugriff auf Adrians Standardkalender delegiert hätte oder wenn Adrian sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="daeb5-123">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="daeb5-124">Wenn Adrian weder seinen Standardkalender für John freigegeben noch sein Postfach an John delegiert hat, wird bei der Angabe von Adrians Benutzer-ID oder seines Benutzerprinzipalnamens in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="daeb5-124">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="daeb5-125">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="daeb5-125">Next steps</span></span>

<span data-ttu-id="daeb5-126">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="daeb5-126">Find out more about:</span></span>

- [<span data-ttu-id="daeb5-127">Vorteile der Integration mit dem Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="daeb5-127">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="daeb5-128">Die [Kalender-API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="daeb5-128">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>