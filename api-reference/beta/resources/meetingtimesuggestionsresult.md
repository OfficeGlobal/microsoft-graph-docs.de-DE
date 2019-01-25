---
title: Ressourcentyp „meetingTimeSuggestionsResult“
description: Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 9d64fe43ac65e3366975b3981053b6d163d41522
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510820"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="bd195-103">Ressourcentyp „meetingTimeSuggestionsResult“</span><span class="sxs-lookup"><span data-stu-id="bd195-103">meetingTimeSuggestionsResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd195-104">Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="bd195-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="bd195-105">In der folgenden Tabelle finden Sie mögliche Gründe, aus denen findMeetingTimes keine Besprechungsvorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="bd195-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="bd195-106">Wert für „emptySuggestionsReason“</span><span class="sxs-lookup"><span data-stu-id="bd195-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="bd195-107">Gründe</span><span class="sxs-lookup"><span data-stu-id="bd195-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="bd195-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="bd195-108">attendeesUnavailable</span></span> | <span data-ttu-id="bd195-109">Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die [Besprechungskonfidenz](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion). Dieser ist standardmäßig auf 50 % festgelegt.</span><span class="sxs-lookup"><span data-stu-id="bd195-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="bd195-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="bd195-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="bd195-p101">Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.</span><span class="sxs-lookup"><span data-stu-id="bd195-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="bd195-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="bd195-113">locationsUnavailable</span></span> | <span data-ttu-id="bd195-114">Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar.</span><span class="sxs-lookup"><span data-stu-id="bd195-114">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="bd195-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="bd195-115">organizerUnavailable</span></span> | <span data-ttu-id="bd195-116">Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="bd195-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="bd195-117">unknown</span><span class="sxs-lookup"><span data-stu-id="bd195-117">unknown</span></span> | <span data-ttu-id="bd195-118">Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.</span><span class="sxs-lookup"><span data-stu-id="bd195-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd195-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd195-119">JSON representation</span></span>

<span data-ttu-id="bd195-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd195-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bd195-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd195-121">Properties</span></span>
| <span data-ttu-id="bd195-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd195-122">Property</span></span>     | <span data-ttu-id="bd195-123">Typ</span><span class="sxs-lookup"><span data-stu-id="bd195-123">Type</span></span>   |<span data-ttu-id="bd195-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd195-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd195-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="bd195-125">emptySuggestionsReason</span></span>|<span data-ttu-id="bd195-126">String</span><span class="sxs-lookup"><span data-stu-id="bd195-126">String</span></span>|<span data-ttu-id="bd195-p102">Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden. Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` oder `unknown`. Diese Eigenschaft ist eine leere Zeichenfolge, wenn die Eigenschaft **meetingTimeSuggestions** keine Besprechungsvorschläge enthält.</span><span class="sxs-lookup"><span data-stu-id="bd195-p102">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="bd195-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="bd195-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="bd195-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span><span class="sxs-lookup"><span data-stu-id="bd195-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="bd195-132">Ein Array von Besprechungsvorschlägen</span><span class="sxs-lookup"><span data-stu-id="bd195-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestionsresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
