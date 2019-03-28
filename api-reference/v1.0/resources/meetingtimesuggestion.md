---
title: Ressourcentyp „meetingTimeSuggestion“
description: 'Ein Besprechungs Vorschlag, der Informationen wie Besprechungszeit, Anwesenheits Wahrscheinlichkeit, einzelne '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4c5a4cb4d094e7fd7fe9b0e56227a556c6e5b5d1
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936262"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="1843a-103">Ressourcentyp „meetingTimeSuggestion“</span><span class="sxs-lookup"><span data-stu-id="1843a-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="1843a-104">Ein Besprechungsvorschlag mit Informationen wie dem Besprechungstermin, der Teilnahmewahrscheinlichkeit, der individuellen Verfügbarkeit und den verfügbaren Besprechungsorten</span><span class="sxs-lookup"><span data-stu-id="1843a-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1843a-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1843a-105">JSON representation</span></span>

<span data-ttu-id="1843a-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1843a-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="1843a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1843a-107">Properties</span></span>
| <span data-ttu-id="1843a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1843a-108">Property</span></span>     | <span data-ttu-id="1843a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1843a-109">Type</span></span>   |<span data-ttu-id="1843a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1843a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1843a-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="1843a-111">attendeeAvailability</span></span>|<span data-ttu-id="1843a-112">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="1843a-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="1843a-113">Ein Array, das den Verfügbarkeitsstatus jedes Teilnehmers für den betreffenden Besprechungsvorschlag anzeigt</span><span class="sxs-lookup"><span data-stu-id="1843a-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="1843a-114">confidence</span><span class="sxs-lookup"><span data-stu-id="1843a-114">confidence</span></span>|<span data-ttu-id="1843a-115">Double</span><span class="sxs-lookup"><span data-stu-id="1843a-115">Double</span></span>|<span data-ttu-id="1843a-116">Ein Prozentwert, der angibt, wie hoch die Wahrscheinlichkeit ist, dass alle Teilnehmer teilnehmen können</span><span class="sxs-lookup"><span data-stu-id="1843a-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="1843a-117">locations</span><span class="sxs-lookup"><span data-stu-id="1843a-117">locations</span></span>|<span data-ttu-id="1843a-118">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="1843a-118">[location](location.md) collection</span></span>|<span data-ttu-id="1843a-119">Ein Array, das den Namen und den geografischen Ort jedes Besprechungsorts für den betreffenden Besprechungsvorschlag angibt</span><span class="sxs-lookup"><span data-stu-id="1843a-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="1843a-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="1843a-120">meetingTimeSlot</span></span>|[<span data-ttu-id="1843a-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="1843a-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="1843a-122">Ein für die Besprechung vorgeschlagenes Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="1843a-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="1843a-123">um</span><span class="sxs-lookup"><span data-stu-id="1843a-123">order</span></span>|<span data-ttu-id="1843a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="1843a-124">Int32</span></span>|<span data-ttu-id="1843a-125">Die Reihenfolge der Besprechungszeit Vorschläge nach dem berechneten Konfidenz Wert von hoch nach niedrig, dann nach der Chronologie, wenn es Vorschläge mit derselben Zuverlässigkeit gibt.</span><span class="sxs-lookup"><span data-stu-id="1843a-125">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="1843a-126">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="1843a-126">organizerAvailability</span></span>|<span data-ttu-id="1843a-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="1843a-127">freeBusyStatus</span></span>| <span data-ttu-id="1843a-128">Die Verfügbarkeit des Besprechungsorganisators für diesen Besprechungsvorschlag.</span><span class="sxs-lookup"><span data-stu-id="1843a-128">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="1843a-129">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1843a-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="1843a-130">Eigenschaft suggestionreason vermerkt</span><span class="sxs-lookup"><span data-stu-id="1843a-130">suggestionReason</span></span>|<span data-ttu-id="1843a-131">String</span><span class="sxs-lookup"><span data-stu-id="1843a-131">String</span></span>|<span data-ttu-id="1843a-132">Grund, aus dem der betreffende Besprechungstermin vorgeschlagen wurde</span><span class="sxs-lookup"><span data-stu-id="1843a-132">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
