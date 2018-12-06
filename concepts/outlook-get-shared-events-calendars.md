---
title: Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender
description: In Outlook können Kunden einen Kalender mit anderen Benutzern teilen und sie Ereignisse in diesem Kalender anzeigen oder ändern lassen. Kunden können außerdem eine Stellvertretung für das Handeln in ihrem Auftrag erteilen, um Besprechungsanfragen zu empfangen oder zu beantworten oder um Elemente im Kalender zu erstellen oder zu ändern.
ms.openlocfilehash: e05352e164b127adca1305dded5cbb00840eed52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092229"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="65b91-104">Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender</span><span class="sxs-lookup"><span data-stu-id="65b91-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="65b91-105">In Outlook können Kunden einen Kalender mit anderen Benutzern teilen und sie Ereignisse in diesem Kalender anzeigen oder ändern lassen.</span><span class="sxs-lookup"><span data-stu-id="65b91-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="65b91-106">Kunden können außerdem eine Stellvertretung für das Handeln in ihrem Auftrag erteilen, um Besprechungsanfragen zu empfangen oder zu beantworten oder um Elemente im Kalender zu erstellen oder zu ändern.</span><span class="sxs-lookup"><span data-stu-id="65b91-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="65b91-107">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Ereignissen in Kalendern, die von anderen Benutzern geteilt wurden, sowie das Abrufen der Kalender selbst.</span><span class="sxs-lookup"><span data-stu-id="65b91-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="65b91-108">Die Unterstützung gilt auch für Kalender, die delegiert wurden.</span><span class="sxs-lookup"><span data-stu-id="65b91-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="65b91-109">Beispielsweise hat Adrian für John seinen Standardkalender freigegeben und John Lesezugriff erteilt.</span><span class="sxs-lookup"><span data-stu-id="65b91-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="65b91-110">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Calendars.Read.Shared oder Calendars.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Adrians Standardkalender und auf die Ereignisse in diesem Kalender zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="65b91-110">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="65b91-111">Abrufen eines Ereignisses im freigegebenen Kalender</span><span class="sxs-lookup"><span data-stu-id="65b91-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="65b91-112">Sie können ein bestimmtes Ereignis in Adrians freigegebenem Standardkalender abrufen:</span><span class="sxs-lookup"><span data-stu-id="65b91-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="65b91-113">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und die [event](/graph/api/resources/event?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Adrians Posteingang.</span><span class="sxs-lookup"><span data-stu-id="65b91-113">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="65b91-114">Abrufen aller Ereignisse im freigegebenen Kalender</span><span class="sxs-lookup"><span data-stu-id="65b91-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="65b91-115">Rufen Sie alle Ereignisse im Standardkalender ab, den Adrian mit John geteilt hat:</span><span class="sxs-lookup"><span data-stu-id="65b91-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="65b91-116">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine Sammlung der [event](/graph/api/resources/event?view=graph-rest-1.0)-Instanzen in Adrians Standardkalender.</span><span class="sxs-lookup"><span data-stu-id="65b91-116">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="65b91-117">Abrufen des freigegebenen Kalenders</span><span class="sxs-lookup"><span data-stu-id="65b91-117">Get the shared folder</span></span>

<span data-ttu-id="65b91-118">Rufen Sie den Standardkalender ab, den Adrian mit John geteilt hat.</span><span class="sxs-lookup"><span data-stu-id="65b91-118">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="65b91-119">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine [calendar](/graph/api/resources/calendar?view=graph-rest-1.0)-Instanz, die Adrians Standardordner darstellt.</span><span class="sxs-lookup"><span data-stu-id="65b91-119">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="65b91-120">Dieselben GET-Funktionen würden gelten, wenn Adrian an John weiteren Zugriff auf Adrians Standardkalender delegiert hätte oder wenn Adrian sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="65b91-120">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="65b91-121">Wenn Adrian weder seinen Standardkalender für John freigegeben noch sein Postfach an John delegiert hat, wird bei der Angabe von Adrians Benutzer-ID oder seines Benutzerprinzipalnamens in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65b91-121">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="65b91-122">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="65b91-122">Next steps</span></span>

<span data-ttu-id="65b91-123">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="65b91-123">Find out more about:</span></span>

- [<span data-ttu-id="65b91-124">Vorteile der Integration mit dem Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="65b91-124">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="65b91-125">Die [Kalender-API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="65b91-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>