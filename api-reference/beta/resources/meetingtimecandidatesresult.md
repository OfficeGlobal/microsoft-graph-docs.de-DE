---
title: Ressourcentyp meetingTimeCandidatesResult
description: Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.
localization_priority: Normal
ms.openlocfilehash: 5b261295de43dcb0bfb94f85c833559430365002
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810654"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="d451f-103">Ressourcentyp meetingTimeCandidatesResult</span><span class="sxs-lookup"><span data-stu-id="d451f-103">meetingTimeCandidatesResult resource type</span></span>

> <span data-ttu-id="d451f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d451f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d451f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d451f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d451f-106">Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d451f-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="d451f-107">In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="d451f-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="d451f-108">**EmptySuggestionsHint Wert**</span><span class="sxs-lookup"><span data-stu-id="d451f-108">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="d451f-109">**Gründe**</span><span class="sxs-lookup"><span data-stu-id="d451f-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="d451f-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="d451f-110">attendeesUnavailable</span></span> | <span data-ttu-id="d451f-111">Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die Besprechungskonfidenz. Dieser ist standardmäßig auf 50 % festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d451f-111">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="d451f-112">Dieser Grenzwert basiert auf der Teilnehmer Frei/Gebucht-Status für einer vorgeschlagenen Besprechung Zeitraum an, mit dem eines Teilnehmers kostenlose Status, Anwesenheit, Status unbekannt 50 % und gebucht-Status 0 % Wahrscheinlichkeit 100 % entspricht.</span><span class="sxs-lookup"><span data-stu-id="d451f-112">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="d451f-113">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="d451f-113">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="d451f-p103">Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.</span><span class="sxs-lookup"><span data-stu-id="d451f-p103">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="d451f-116">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="d451f-116">locationsUnavailable</span></span> | <span data-ttu-id="d451f-117">Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d451f-117">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="d451f-118">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="d451f-118">organizerUnavailable</span></span> | <span data-ttu-id="d451f-119">Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d451f-119">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="d451f-120">unknown</span><span class="sxs-lookup"><span data-stu-id="d451f-120">unknown</span></span> | <span data-ttu-id="d451f-121">Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.</span><span class="sxs-lookup"><span data-stu-id="d451f-121">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d451f-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d451f-122">JSON representation</span></span>

<span data-ttu-id="d451f-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d451f-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a><span data-ttu-id="d451f-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d451f-124">Properties</span></span>
| <span data-ttu-id="d451f-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d451f-125">Property</span></span>     | <span data-ttu-id="d451f-126">Typ</span><span class="sxs-lookup"><span data-stu-id="d451f-126">Type</span></span>   |<span data-ttu-id="d451f-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d451f-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d451f-128">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="d451f-128">emptySuggestionsHint</span></span>|<span data-ttu-id="d451f-129">String</span><span class="sxs-lookup"><span data-stu-id="d451f-129">String</span></span>|<span data-ttu-id="d451f-p104">Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden. Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d451f-p104">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="d451f-132">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="d451f-132">meetingTimeSlots</span></span>|<span data-ttu-id="d451f-133">[MeetingTimeCandidate](meetingtimecandidate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d451f-133">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="d451f-134">Ein Array von Besprechungsvorschlägen</span><span class="sxs-lookup"><span data-stu-id="d451f-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
