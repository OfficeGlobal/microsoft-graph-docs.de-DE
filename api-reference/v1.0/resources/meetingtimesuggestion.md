---
title: Ressourcentyp „meetingTimeSuggestion“
description: 'Ein besprechungsvorschlag, das Informationen wie Besprechungszeit, Anwesenheit Wahrscheinlichkeit, einzelne enthält '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 8472526709e563900ac5193b0065111f3ed620fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978809"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="3bdde-103">Ressourcentyp „meetingTimeSuggestion“</span><span class="sxs-lookup"><span data-stu-id="3bdde-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="3bdde-104">Ein Besprechungsvorschlag mit Informationen wie dem Besprechungstermin, der Teilnahmewahrscheinlichkeit, der individuellen Verfügbarkeit und den verfügbaren Besprechungsorten</span><span class="sxs-lookup"><span data-stu-id="3bdde-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bdde-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3bdde-105">JSON representation</span></span>

<span data-ttu-id="3bdde-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3bdde-106">Here is a JSON representation of the resource</span></span>

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
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="3bdde-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3bdde-107">Properties</span></span>
| <span data-ttu-id="3bdde-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3bdde-108">Property</span></span>     | <span data-ttu-id="3bdde-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3bdde-109">Type</span></span>   |<span data-ttu-id="3bdde-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bdde-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bdde-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="3bdde-111">attendeeAvailability</span></span>|<span data-ttu-id="3bdde-112">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="3bdde-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="3bdde-113">Ein Array, das den Verfügbarkeitsstatus jedes Teilnehmers für den betreffenden Besprechungsvorschlag anzeigt</span><span class="sxs-lookup"><span data-stu-id="3bdde-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="3bdde-114">confidence</span><span class="sxs-lookup"><span data-stu-id="3bdde-114">confidence</span></span>|<span data-ttu-id="3bdde-115">Double</span><span class="sxs-lookup"><span data-stu-id="3bdde-115">Double</span></span>|<span data-ttu-id="3bdde-116">Ein Prozentwert, der angibt, wie hoch die Wahrscheinlichkeit ist, dass alle Teilnehmer teilnehmen können</span><span class="sxs-lookup"><span data-stu-id="3bdde-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="3bdde-117">locations</span><span class="sxs-lookup"><span data-stu-id="3bdde-117">locations</span></span>|<span data-ttu-id="3bdde-118">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3bdde-118">[location](location.md) collection</span></span>|<span data-ttu-id="3bdde-119">Ein Array, das den Namen und den geografischen Ort jedes Besprechungsorts für den betreffenden Besprechungsvorschlag angibt</span><span class="sxs-lookup"><span data-stu-id="3bdde-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="3bdde-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="3bdde-120">meetingTimeSlot</span></span>|[<span data-ttu-id="3bdde-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="3bdde-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="3bdde-122">Ein für die Besprechung vorgeschlagenes Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="3bdde-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="3bdde-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="3bdde-123">organizerAvailability</span></span>|<span data-ttu-id="3bdde-124">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="3bdde-124">freeBusyStatus</span></span>| <span data-ttu-id="3bdde-125">Verfügbarkeit der Organisator der Besprechung für diese besprechungsvorschlag.</span><span class="sxs-lookup"><span data-stu-id="3bdde-125">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="3bdde-126">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3bdde-126">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="3bdde-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="3bdde-127">suggestionReason</span></span>|<span data-ttu-id="3bdde-128">String</span><span class="sxs-lookup"><span data-stu-id="3bdde-128">String</span></span>|<span data-ttu-id="3bdde-129">Grund, aus dem der betreffende Besprechungstermin vorgeschlagen wurde</span><span class="sxs-lookup"><span data-stu-id="3bdde-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
