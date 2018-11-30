---
title: Ressourcentyp meetingTimeCandidate
description: 'Ein besprechungsvorschlag, das Informationen wie Besprechungszeit, Anwesenheit Wahrscheinlichkeit, einzelne enthält '
ms.openlocfilehash: 56aae66cf4c532108d2db2f8f4cfc71487f09150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059852"
---
# <a name="meetingtimecandidate-resource-type"></a><span data-ttu-id="1c902-103">Ressourcentyp meetingTimeCandidate</span><span class="sxs-lookup"><span data-stu-id="1c902-103">meetingTimeCandidate resource type</span></span>

> <span data-ttu-id="1c902-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c902-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c902-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c902-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c902-106">Ein Besprechungsvorschlag mit Informationen wie dem Besprechungstermin, der Teilnahmewahrscheinlichkeit, der individuellen Verfügbarkeit und den verfügbaren Besprechungsorten</span><span class="sxs-lookup"><span data-stu-id="1c902-106">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c902-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1c902-107">JSON representation</span></span>

<span data-ttu-id="1c902-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1c902-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidate"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionHint": "String"
}

```
## <a name="properties"></a><span data-ttu-id="1c902-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1c902-109">Properties</span></span>
| <span data-ttu-id="1c902-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c902-110">Property</span></span>     | <span data-ttu-id="1c902-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1c902-111">Type</span></span>   |<span data-ttu-id="1c902-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c902-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c902-113">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="1c902-113">attendeeAvailability</span></span>|<span data-ttu-id="1c902-114">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="1c902-114">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="1c902-115">Ein Array, das den Verfügbarkeitsstatus jedes Teilnehmers für den betreffenden Besprechungsvorschlag anzeigt</span><span class="sxs-lookup"><span data-stu-id="1c902-115">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="1c902-116">confidence</span><span class="sxs-lookup"><span data-stu-id="1c902-116">confidence</span></span>|<span data-ttu-id="1c902-117">Double</span><span class="sxs-lookup"><span data-stu-id="1c902-117">Double</span></span>|<span data-ttu-id="1c902-118">Ein Prozentwert, der angibt, wie hoch die Wahrscheinlichkeit ist, dass alle Teilnehmer teilnehmen können</span><span class="sxs-lookup"><span data-stu-id="1c902-118">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="1c902-119">locations</span><span class="sxs-lookup"><span data-stu-id="1c902-119">locations</span></span>|<span data-ttu-id="1c902-120">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1c902-120">[location](location.md) collection</span></span>|<span data-ttu-id="1c902-121">Ein Array, das den Namen und den geografischen Ort jedes Besprechungsorts für den betreffenden Besprechungsvorschlag angibt</span><span class="sxs-lookup"><span data-stu-id="1c902-121">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="1c902-122">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="1c902-122">meetingTimeSlot</span></span>|[<span data-ttu-id="1c902-123">timeSlot</span><span class="sxs-lookup"><span data-stu-id="1c902-123">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="1c902-124">Ein für die Besprechung vorgeschlagenes Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="1c902-124">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="1c902-125">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="1c902-125">organizerAvailability</span></span>|<span data-ttu-id="1c902-126">String</span><span class="sxs-lookup"><span data-stu-id="1c902-126">String</span></span>| <span data-ttu-id="1c902-p102">Die Verfügbarkeit des Besprechungsorganisators für diesen Besprechungsvorschlag. Mögliche Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1c902-p102">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="1c902-129">suggestionHint</span><span class="sxs-lookup"><span data-stu-id="1c902-129">suggestionHint</span></span>|<span data-ttu-id="1c902-130">String</span><span class="sxs-lookup"><span data-stu-id="1c902-130">String</span></span>|<span data-ttu-id="1c902-131">Grund, aus dem der betreffende Besprechungstermin vorgeschlagen wurde</span><span class="sxs-lookup"><span data-stu-id="1c902-131">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->