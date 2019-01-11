---
title: Ressourcentyp „meetingTimeSuggestionsResult“
description: Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.
localization_priority: Normal
ms.openlocfilehash: 85a0c3ade54204cb78957e81325869197f403c5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823695"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="10e51-103">Ressourcentyp „meetingTimeSuggestionsResult“</span><span class="sxs-lookup"><span data-stu-id="10e51-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="10e51-104">Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="10e51-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="10e51-105">In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="10e51-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="10e51-106">**Wert für „emptySuggestionsReason“**</span><span class="sxs-lookup"><span data-stu-id="10e51-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="10e51-107">**Gründe**</span><span class="sxs-lookup"><span data-stu-id="10e51-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="10e51-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="10e51-108">attendeesUnavailable</span></span> | <span data-ttu-id="10e51-109">Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die [Besprechungskonfidenz](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion). Dieser ist standardmäßig auf 50 % festgelegt.</span><span class="sxs-lookup"><span data-stu-id="10e51-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="10e51-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="10e51-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="10e51-p101">Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.</span><span class="sxs-lookup"><span data-stu-id="10e51-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="10e51-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="10e51-113">locationsUnavailable</span></span> | <span data-ttu-id="10e51-114">Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar.</span><span class="sxs-lookup"><span data-stu-id="10e51-114">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="10e51-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="10e51-115">organizerUnavailable</span></span> | <span data-ttu-id="10e51-116">Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="10e51-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="10e51-117">unknown</span><span class="sxs-lookup"><span data-stu-id="10e51-117">unknown</span></span> | <span data-ttu-id="10e51-118">Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.</span><span class="sxs-lookup"><span data-stu-id="10e51-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10e51-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10e51-119">JSON representation</span></span>

<span data-ttu-id="10e51-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10e51-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="10e51-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10e51-121">Properties</span></span>
| <span data-ttu-id="10e51-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10e51-122">Property</span></span>     | <span data-ttu-id="10e51-123">Typ</span><span class="sxs-lookup"><span data-stu-id="10e51-123">Type</span></span>   |<span data-ttu-id="10e51-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10e51-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10e51-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="10e51-125">emptySuggestionsReason</span></span>|<span data-ttu-id="10e51-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10e51-126">String</span></span>|<span data-ttu-id="10e51-127">Einen Grund für die Besprechungsvorschläge nicht zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="10e51-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="10e51-128">Die möglichen Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, oder `unknown`.</span><span class="sxs-lookup"><span data-stu-id="10e51-128">The possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="10e51-129">Diese Eigenschaft ist eine leere Zeichenfolge, wenn die **MeetingTimeSuggestions** -Eigenschaft Besprechungsvorschläge enthält.</span><span class="sxs-lookup"><span data-stu-id="10e51-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="10e51-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="10e51-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="10e51-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span><span class="sxs-lookup"><span data-stu-id="10e51-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="10e51-132">Ein Array von Besprechungsvorschlägen</span><span class="sxs-lookup"><span data-stu-id="10e51-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
