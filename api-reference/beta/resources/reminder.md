---
title: reminder-Ressourcentyp
description: Eine Erinnerung für ein Ereignis in einem Benutzerkalender.
localization_priority: Normal
ms.openlocfilehash: 88d9cb4f30f60819a606b3b1f3573d16860d9a00
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521033"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="906cd-103">reminder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="906cd-103">reminder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="906cd-104">Eine Erinnerung für ein [Ereignis](event.md) in einem [Kalender](calendar.md)des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="906cd-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="906cd-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="906cd-105">Properties</span></span>
| <span data-ttu-id="906cd-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="906cd-106">Property</span></span>     | <span data-ttu-id="906cd-107">Typ</span><span class="sxs-lookup"><span data-stu-id="906cd-107">Type</span></span>   |<span data-ttu-id="906cd-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="906cd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="906cd-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="906cd-109">changeKey</span></span>|<span data-ttu-id="906cd-110">String</span><span class="sxs-lookup"><span data-stu-id="906cd-110">String</span></span>|<span data-ttu-id="906cd-p101">Gibt die Version der Erinnerung an. Jedes Mal, wenn die Erinnerung geändert wird, wird auch **changeKey** geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="906cd-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="906cd-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="906cd-114">eventEndTime</span></span>|[<span data-ttu-id="906cd-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="906cd-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="906cd-116">Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="906cd-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="906cd-117">eventId</span><span class="sxs-lookup"><span data-stu-id="906cd-117">eventId</span></span>|<span data-ttu-id="906cd-118">String</span><span class="sxs-lookup"><span data-stu-id="906cd-118">String</span></span>|<span data-ttu-id="906cd-p102">Die eindeutige ID des Ereignisses. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="906cd-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="906cd-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="906cd-121">eventLocation</span></span>|[<span data-ttu-id="906cd-122">Location</span><span class="sxs-lookup"><span data-stu-id="906cd-122">Location</span></span>](location.md)|<span data-ttu-id="906cd-123">Der Speicherort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="906cd-123">The location of the event.</span></span>|
|<span data-ttu-id="906cd-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="906cd-124">eventStartTime</span></span>|[<span data-ttu-id="906cd-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="906cd-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="906cd-126">Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="906cd-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="906cd-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="906cd-127">eventSubject</span></span>|<span data-ttu-id="906cd-128">String</span><span class="sxs-lookup"><span data-stu-id="906cd-128">String</span></span>|<span data-ttu-id="906cd-129">Der Text der Betreffzeile des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="906cd-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="906cd-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="906cd-130">eventWebLink</span></span>|<span data-ttu-id="906cd-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="906cd-131">String</span></span>|<span data-ttu-id="906cd-132">Die URL zum Öfnen des Ereignisses in Outlook im Web.</span><span class="sxs-lookup"><span data-stu-id="906cd-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="906cd-p103">Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook im Web bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="906cd-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="906cd-135">Auf diese URL kann von einem iFrame aus zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="906cd-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="906cd-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="906cd-136">reminderFireTime</span></span>|[<span data-ttu-id="906cd-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="906cd-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="906cd-138">Datum, Uhrzeit und Zeitzone für das Ausführen der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="906cd-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="906cd-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="906cd-139">JSON representation</span></span>

<span data-ttu-id="906cd-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="906cd-140">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/reminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
