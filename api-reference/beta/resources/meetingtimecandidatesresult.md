---
title: Ressourcentyp meetingTimeCandidatesResult
description: Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: e60c0092ca5724e4019a4c3f75f1239a0e7e9c0b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507516"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="09d3f-103">Ressourcentyp meetingTimeCandidatesResult</span><span class="sxs-lookup"><span data-stu-id="09d3f-103">meetingTimeCandidatesResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d3f-104">Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="09d3f-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="09d3f-105">In der folgenden Tabelle finden Sie mögliche Gründe, aus denen findMeetingTimes keine Besprechungsvorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="09d3f-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="09d3f-106">**EmptySuggestionsHint Wert**</span><span class="sxs-lookup"><span data-stu-id="09d3f-106">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="09d3f-107">Gründe</span><span class="sxs-lookup"><span data-stu-id="09d3f-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="09d3f-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="09d3f-108">attendeesUnavailable</span></span> | <span data-ttu-id="09d3f-109">Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die Besprechungskonfidenz. Dieser ist standardmäßig auf 50 % festgelegt.</span><span class="sxs-lookup"><span data-stu-id="09d3f-109">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="09d3f-110">Dieser Grenzwert basiert auf der Teilnehmer Frei/Gebucht-Status für einer vorgeschlagenen Besprechung Zeitraum an, mit dem eines Teilnehmers kostenlose Status, Anwesenheit, Status unbekannt 50 % und gebucht-Status 0 % Wahrscheinlichkeit 100 % entspricht.</span><span class="sxs-lookup"><span data-stu-id="09d3f-110">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="09d3f-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="09d3f-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="09d3f-p102">Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.</span><span class="sxs-lookup"><span data-stu-id="09d3f-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="09d3f-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="09d3f-114">locationsUnavailable</span></span> | <span data-ttu-id="09d3f-115">Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar.</span><span class="sxs-lookup"><span data-stu-id="09d3f-115">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="09d3f-116">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="09d3f-116">organizerUnavailable</span></span> | <span data-ttu-id="09d3f-117">Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="09d3f-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="09d3f-118">unknown</span><span class="sxs-lookup"><span data-stu-id="09d3f-118">unknown</span></span> | <span data-ttu-id="09d3f-119">Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.</span><span class="sxs-lookup"><span data-stu-id="09d3f-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09d3f-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="09d3f-120">JSON representation</span></span>

<span data-ttu-id="09d3f-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="09d3f-121">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="09d3f-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="09d3f-122">Properties</span></span>
| <span data-ttu-id="09d3f-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09d3f-123">Property</span></span>     | <span data-ttu-id="09d3f-124">Typ</span><span class="sxs-lookup"><span data-stu-id="09d3f-124">Type</span></span>   |<span data-ttu-id="09d3f-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09d3f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09d3f-126">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="09d3f-126">emptySuggestionsHint</span></span>|<span data-ttu-id="09d3f-127">String</span><span class="sxs-lookup"><span data-stu-id="09d3f-127">String</span></span>|<span data-ttu-id="09d3f-p103">Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden. Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="09d3f-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="09d3f-130">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="09d3f-130">meetingTimeSlots</span></span>|<span data-ttu-id="09d3f-131">[MeetingTimeCandidate](meetingtimecandidate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="09d3f-131">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="09d3f-132">Ein Array von Besprechungsvorschlägen</span><span class="sxs-lookup"><span data-stu-id="09d3f-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimecandidatesresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
