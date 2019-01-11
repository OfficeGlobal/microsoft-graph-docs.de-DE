---
title: reminder-Ressourcentyp
description: Eine Erinnerung für ein Ereignis in einem Benutzerkalender.
localization_priority: Normal
ms.openlocfilehash: a78c7f82ea0a7db9da45a60de98bb3b1311aaeeb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819964"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="5a980-103">reminder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5a980-103">reminder resource type</span></span>

> <span data-ttu-id="5a980-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5a980-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a980-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a980-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a980-106">Eine Erinnerung für ein [Ereignis](event.md) in einem [Kalender](calendar.md)des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="5a980-106">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a980-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5a980-107">Properties</span></span>
| <span data-ttu-id="5a980-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a980-108">Property</span></span>     | <span data-ttu-id="5a980-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5a980-109">Type</span></span>   |<span data-ttu-id="5a980-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a980-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a980-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="5a980-111">changeKey</span></span>|<span data-ttu-id="5a980-112">String</span><span class="sxs-lookup"><span data-stu-id="5a980-112">String</span></span>|<span data-ttu-id="5a980-p102">Gibt die Version der Erinnerung an. Jedes Mal, wenn die Erinnerung geändert wird, wird auch **changeKey** geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="5a980-p102">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="5a980-116">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="5a980-116">eventEndTime</span></span>|[<span data-ttu-id="5a980-117">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5a980-117">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5a980-118">Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="5a980-118">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="5a980-119">eventId</span><span class="sxs-lookup"><span data-stu-id="5a980-119">eventId</span></span>|<span data-ttu-id="5a980-120">String</span><span class="sxs-lookup"><span data-stu-id="5a980-120">String</span></span>|<span data-ttu-id="5a980-p103">Die eindeutige ID des Ereignisses. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5a980-p103">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="5a980-123">eventLocation</span><span class="sxs-lookup"><span data-stu-id="5a980-123">eventLocation</span></span>|[<span data-ttu-id="5a980-124">Location</span><span class="sxs-lookup"><span data-stu-id="5a980-124">Location</span></span>](location.md)|<span data-ttu-id="5a980-125">Der Speicherort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="5a980-125">The location of the event.</span></span>|
|<span data-ttu-id="5a980-126">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="5a980-126">eventStartTime</span></span>|[<span data-ttu-id="5a980-127">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5a980-127">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5a980-128">Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="5a980-128">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="5a980-129">eventSubject</span><span class="sxs-lookup"><span data-stu-id="5a980-129">eventSubject</span></span>|<span data-ttu-id="5a980-130">String</span><span class="sxs-lookup"><span data-stu-id="5a980-130">String</span></span>|<span data-ttu-id="5a980-131">Der Text der Betreffzeile des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="5a980-131">The text of the event's subject line.</span></span>|
|<span data-ttu-id="5a980-132">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="5a980-132">eventWebLink</span></span>|<span data-ttu-id="5a980-133">String</span><span class="sxs-lookup"><span data-stu-id="5a980-133">String</span></span>|<span data-ttu-id="5a980-134">Die URL zum Öfnen des Ereignisses in Outlook im Web.</span><span class="sxs-lookup"><span data-stu-id="5a980-134">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="5a980-p104">Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook im Web bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="5a980-p104">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="5a980-137">Auf diese URL kann von einem iFrame aus zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="5a980-137">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="5a980-138">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="5a980-138">reminderFireTime</span></span>|[<span data-ttu-id="5a980-139">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5a980-139">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5a980-140">Datum, Uhrzeit und Zeitzone für das Ausführen der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="5a980-140">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a980-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5a980-141">JSON representation</span></span>

<span data-ttu-id="5a980-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5a980-142">Here is a JSON representation of the resource</span></span>

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
