---
title: reminder-Ressourcentyp
description: Eine Erinnerung für ein Ereignis in einem Benutzerkalender.
ms.openlocfilehash: 131de8772c6b4fa400ab0f48197430611030c255
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019501"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="3c209-103">reminder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c209-103">reminder resource type</span></span>

<span data-ttu-id="3c209-104">Eine Erinnerung für ein [Ereignis](event.md) in einem [Kalender](calendar.md)des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="3c209-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3c209-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c209-105">Properties</span></span>
| <span data-ttu-id="3c209-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c209-106">Property</span></span>     | <span data-ttu-id="3c209-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3c209-107">Type</span></span>   |<span data-ttu-id="3c209-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c209-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c209-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="3c209-109">changeKey</span></span>|<span data-ttu-id="3c209-110">String</span><span class="sxs-lookup"><span data-stu-id="3c209-110">String</span></span>|<span data-ttu-id="3c209-p101">Gibt die Version der Erinnerung an. Jedes Mal, wenn die Erinnerung geändert wird, wird auch **changeKey** geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="3c209-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="3c209-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="3c209-114">eventEndTime</span></span>|[<span data-ttu-id="3c209-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3c209-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3c209-116">Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="3c209-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="3c209-117">eventId</span><span class="sxs-lookup"><span data-stu-id="3c209-117">eventId</span></span>|<span data-ttu-id="3c209-118">String</span><span class="sxs-lookup"><span data-stu-id="3c209-118">String</span></span>|<span data-ttu-id="3c209-p102">Die eindeutige ID des Ereignisses. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3c209-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="3c209-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="3c209-121">eventLocation</span></span>|[<span data-ttu-id="3c209-122">Location</span><span class="sxs-lookup"><span data-stu-id="3c209-122">Location</span></span>](location.md)|<span data-ttu-id="3c209-123">Der Speicherort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="3c209-123">The location of the event.</span></span>|
|<span data-ttu-id="3c209-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="3c209-124">eventStartTime</span></span>|[<span data-ttu-id="3c209-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3c209-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3c209-126">Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="3c209-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="3c209-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="3c209-127">eventSubject</span></span>|<span data-ttu-id="3c209-128">String</span><span class="sxs-lookup"><span data-stu-id="3c209-128">String</span></span>|<span data-ttu-id="3c209-129">Der Text der Betreffzeile des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="3c209-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="3c209-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="3c209-130">eventWebLink</span></span>|<span data-ttu-id="3c209-131">String</span><span class="sxs-lookup"><span data-stu-id="3c209-131">String</span></span>|<span data-ttu-id="3c209-132">Die URL zum Öfnen des Ereignisses in Outlook im Web.</span><span class="sxs-lookup"><span data-stu-id="3c209-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="3c209-p103">Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook im Web bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="3c209-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="3c209-135">Auf diese URL kann von einem iFrame aus zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="3c209-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="3c209-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="3c209-136">reminderFireTime</span></span>|[<span data-ttu-id="3c209-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3c209-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3c209-138">Datum, Uhrzeit und Zeitzone für das Ausführen der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="3c209-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c209-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c209-139">JSON representation</span></span>

<span data-ttu-id="3c209-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c209-140">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->