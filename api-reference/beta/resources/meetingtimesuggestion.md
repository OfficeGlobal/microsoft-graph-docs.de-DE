---
title: Ressourcentyp „meetingTimeSuggestion“
description: 'Ein Besprechungs Vorschlag, der Informationen wie Besprechungszeit, Anwesenheits Wahrscheinlichkeit, einzelne '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 379bb4ac4be8e2d8d1bec494cf4d573550d46b55
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057029"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="d5bdb-103">Ressourcentyp „meetingTimeSuggestion“</span><span class="sxs-lookup"><span data-stu-id="d5bdb-103">meetingTimeSuggestion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5bdb-104">Ein Besprechungsvorschlag mit Informationen wie dem Besprechungstermin, der Teilnahmewahrscheinlichkeit, der individuellen Verfügbarkeit und den verfügbaren Besprechungsorten</span><span class="sxs-lookup"><span data-stu-id="d5bdb-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5bdb-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5bdb-105">JSON representation</span></span>

<span data-ttu-id="d5bdb-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5bdb-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.locationDataModel"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.meetingTimeSlotDataModel"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="d5bdb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5bdb-107">Properties</span></span>
| <span data-ttu-id="d5bdb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5bdb-108">Property</span></span>     | <span data-ttu-id="d5bdb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d5bdb-109">Type</span></span>   |<span data-ttu-id="d5bdb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5bdb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5bdb-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="d5bdb-111">attendeeAvailability</span></span>|<span data-ttu-id="d5bdb-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d5bdb-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md) collection</span></span>|<span data-ttu-id="d5bdb-113">Ein Array, das den Verfügbarkeitsstatus jedes Teilnehmers für den betreffenden Besprechungsvorschlag anzeigt</span><span class="sxs-lookup"><span data-stu-id="d5bdb-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="d5bdb-114">confidence</span><span class="sxs-lookup"><span data-stu-id="d5bdb-114">confidence</span></span>|<span data-ttu-id="d5bdb-115">Double</span><span class="sxs-lookup"><span data-stu-id="d5bdb-115">Double</span></span>|<span data-ttu-id="d5bdb-116">Ein Prozentwert, der angibt, wie hoch die Wahrscheinlichkeit ist, dass alle Teilnehmer teilnehmen können</span><span class="sxs-lookup"><span data-stu-id="d5bdb-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="d5bdb-117">locations</span><span class="sxs-lookup"><span data-stu-id="d5bdb-117">locations</span></span>|<span data-ttu-id="d5bdb-118">[locationDataModel](locationdatamodel.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d5bdb-118">[locationDataModel](locationdatamodel.md) collection</span></span>|<span data-ttu-id="d5bdb-119">Ein Array, das den Namen und den geografischen Ort jedes Besprechungsorts für den betreffenden Besprechungsvorschlag angibt</span><span class="sxs-lookup"><span data-stu-id="d5bdb-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="d5bdb-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="d5bdb-120">meetingTimeSlot</span></span>|[<span data-ttu-id="d5bdb-121">meetingTimeSlotDataModel</span><span class="sxs-lookup"><span data-stu-id="d5bdb-121">meetingTimeSlotDataModel</span></span>](meetingtimeslotdatamodel.md)|<span data-ttu-id="d5bdb-122">Ein für die Besprechung vorgeschlagenes Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="d5bdb-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="d5bdb-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="d5bdb-123">organizerAvailability</span></span>|<span data-ttu-id="d5bdb-124">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="d5bdb-124">availabilityStatus</span></span>| <span data-ttu-id="d5bdb-p101">Die Verfügbarkeit des Besprechungsorganisators für diesen Besprechungsvorschlag. Mögliche Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d5bdb-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="d5bdb-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="d5bdb-127">suggestionReason</span></span>|<span data-ttu-id="d5bdb-128">String</span><span class="sxs-lookup"><span data-stu-id="d5bdb-128">String</span></span>|<span data-ttu-id="d5bdb-129">Grund, aus dem der betreffende Besprechungstermin vorgeschlagen wurde</span><span class="sxs-lookup"><span data-stu-id="d5bdb-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
