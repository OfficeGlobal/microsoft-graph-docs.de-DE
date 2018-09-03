# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="28b92-101">Ressourcentyp „meetingTimeSuggestion“</span><span class="sxs-lookup"><span data-stu-id="28b92-101">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="28b92-102">Ein Besprechungsvorschlag mit Informationen wie dem Besprechungstermin, der Teilnahmewahrscheinlichkeit, der individuellen Verfügbarkeit und den verfügbaren Besprechungsorten</span><span class="sxs-lookup"><span data-stu-id="28b92-102">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28b92-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28b92-103">JSON representation</span></span>

<span data-ttu-id="28b92-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="28b92-104">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="28b92-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28b92-105">Properties</span></span>
| <span data-ttu-id="28b92-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28b92-106">Property</span></span>     | <span data-ttu-id="28b92-107">Typ</span><span class="sxs-lookup"><span data-stu-id="28b92-107">Type</span></span>   |<span data-ttu-id="28b92-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28b92-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28b92-109">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="28b92-109">attendeeAvailability</span></span>|<span data-ttu-id="28b92-110">[attendeeAvailability](attendeeavailability.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="28b92-110">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="28b92-111">Ein Array, das den Verfügbarkeitsstatus jedes Teilnehmers für diesen Besprechungsvorschlag anzeigt.</span><span class="sxs-lookup"><span data-stu-id="28b92-111">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="28b92-112">confidence</span><span class="sxs-lookup"><span data-stu-id="28b92-112">confidence</span></span>|<span data-ttu-id="28b92-113">Doppelt</span><span class="sxs-lookup"><span data-stu-id="28b92-113">Double</span></span>|<span data-ttu-id="28b92-114">Ein Prozentwert, der angibt, wie hoch die Wahrscheinlichkeit ist, dass alle Teilnehmer teilnehmen können</span><span class="sxs-lookup"><span data-stu-id="28b92-114">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="28b92-115">Orte</span><span class="sxs-lookup"><span data-stu-id="28b92-115">locations</span></span>|<span data-ttu-id="28b92-116">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="28b92-116">[location](location.md) collection</span></span>|<span data-ttu-id="28b92-117">Ein Array, das den Namen und den geografischen Ort jedes Besprechungsorts für den betreffenden Besprechungsvorschlag angibt</span><span class="sxs-lookup"><span data-stu-id="28b92-117">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="28b92-118">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="28b92-118">meetingTimeSlot</span></span>|[<span data-ttu-id="28b92-119">timeSlot</span><span class="sxs-lookup"><span data-stu-id="28b92-119">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="28b92-120">Ein für die Besprechung vorgeschlagenes Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="28b92-120">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="28b92-121">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="28b92-121">organizerAvailability</span></span>|<span data-ttu-id="28b92-122">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="28b92-122">FreeBusyStatus</span></span>| <span data-ttu-id="28b92-123">Die Verfügbarkeit des Besprechungsorganisators für diesen Besprechungsvorschlag.</span><span class="sxs-lookup"><span data-stu-id="28b92-123">Availability of the meeting organizer for this meeting suggestion. Possible values are: , , , , , .</span></span> <span data-ttu-id="28b92-124">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="28b92-124">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="28b92-125">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="28b92-125">suggestionReason</span></span>|<span data-ttu-id="28b92-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28b92-126">String</span></span>|<span data-ttu-id="28b92-127">Grund, aus dem der betreffende Besprechungstermin vorgeschlagen wurde</span><span class="sxs-lookup"><span data-stu-id="28b92-127">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->