# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="0f8e3-101">Ressourcentyp „meetingTimeSuggestionsResult“</span><span class="sxs-lookup"><span data-stu-id="0f8e3-101">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="0f8e3-102">Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-102">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="0f8e3-103">In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user_findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-103">The following are the possible reasons that [findMeetingTimes](../api/user_findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="0f8e3-104">**Wert für emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="0f8e3-104">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="0f8e3-105">**Gründe**</span><span class="sxs-lookup"><span data-stu-id="0f8e3-105">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="0f8e3-106">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="0f8e3-106">attendeesUnavailable</span></span> | <span data-ttu-id="0f8e3-107">Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die [Besprechungskonfidenz](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion). Dieser ist standardmäßig auf 50 % festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-107">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="0f8e3-108">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="0f8e3-108">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="0f8e3-p101">Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="0f8e3-111">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="0f8e3-111">locationsUnavailable</span></span> | <span data-ttu-id="0f8e3-112">Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-112">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="0f8e3-113">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="0f8e3-113">organizerUnavailable</span></span> | <span data-ttu-id="0f8e3-114">Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, aber der Organisator ist während des angefragten Zeitfensters nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-114">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="0f8e3-115">unbekannt</span><span class="sxs-lookup"><span data-stu-id="0f8e3-115">unknown</span></span> | <span data-ttu-id="0f8e3-116">Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-116">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f8e3-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f8e3-117">JSON representation</span></span>

<span data-ttu-id="0f8e3-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="0f8e3-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f8e3-119">Properties</span></span>
| <span data-ttu-id="0f8e3-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f8e3-120">Property</span></span>     | <span data-ttu-id="0f8e3-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0f8e3-121">Type</span></span>   |<span data-ttu-id="0f8e3-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f8e3-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f8e3-123">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="0f8e3-123">emptySuggestionsReason</span></span>|<span data-ttu-id="0f8e3-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f8e3-124">String</span></span>|<span data-ttu-id="0f8e3-125">Ein Grund dafür, dass keine Besprechungsvorschläge zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-125">A reason for not returning any meeting suggestions. Possible values are: , , , , or .</span></span> <span data-ttu-id="0f8e3-126">Die möglichen Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, oder`unknown`.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-126">The possible values are `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, , , , , , , , or `unknown`.</span></span> <span data-ttu-id="0f8e3-127">Diese Eigenschaft ist eine leere Zeichenfolge, wenn die **meetingTimeSuggestions** -Eigenschaft Besprechungsvorschläge enthält.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-127">A reason for not returning any meeting suggestions. Possible values are: , , , , or . This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="0f8e3-128">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="0f8e3-128">meetingTimeSuggestions</span></span>|<span data-ttu-id="0f8e3-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0f8e3-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) collection</span></span>|<span data-ttu-id="0f8e3-130">Ein Array von Besprechungsvorschlägen.</span><span class="sxs-lookup"><span data-stu-id="0f8e3-130">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->