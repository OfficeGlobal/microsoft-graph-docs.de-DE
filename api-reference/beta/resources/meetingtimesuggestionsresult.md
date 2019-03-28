---
title: Ressourcentyp „meetingTimeSuggestionsResult“
description: Eine Sammlung von Besprechungs Vorschlägen, falls vorhanden, und der Grund, wenn dies nicht der Fall ist.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 654e53c5a3a329774e1b78065bb8cbcd41d6721f
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937788"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="90ca1-103">Ressourcentyp „meetingTimeSuggestionsResult“</span><span class="sxs-lookup"><span data-stu-id="90ca1-103">meetingTimeSuggestionsResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ca1-104">Eine Sammlung von Besprechungs Vorschlägen, falls vorhanden, und der Grund, wenn dies nicht der Fall ist.</span><span class="sxs-lookup"><span data-stu-id="90ca1-104">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="90ca1-105">In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="90ca1-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="90ca1-106">**Wert für „emptySuggestionsReason“**</span><span class="sxs-lookup"><span data-stu-id="90ca1-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="90ca1-107">**Gründe**</span><span class="sxs-lookup"><span data-stu-id="90ca1-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="90ca1-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="90ca1-108">attendeesUnavailable</span></span> | <span data-ttu-id="90ca1-109">Die Verfügbarkeit aller Teilnehmer ist bekannt, aber nicht genügend Teilnehmer stehen zur Verfügung, um den Vertrauens Schwellenwert für die [Besprechung](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) zu erreichen, der standardmäßig 50% für einen beliebigen Zeitraum beträgt.</span><span class="sxs-lookup"><span data-stu-id="90ca1-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="90ca1-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="90ca1-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="90ca1-p101">Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.</span><span class="sxs-lookup"><span data-stu-id="90ca1-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="90ca1-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="90ca1-113">locationsUnavailable</span></span> | <span data-ttu-id="90ca1-114">Die **IsRequired** -Eigenschaft des **timeconstraint** -Parameters ist als true angegeben, und es sind jedoch keine Speicherorte an den berechneten Zeitschlitzen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="90ca1-114">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="90ca1-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="90ca1-115">organizerUnavailable</span></span> | <span data-ttu-id="90ca1-116">Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="90ca1-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="90ca1-117">unknown</span><span class="sxs-lookup"><span data-stu-id="90ca1-117">unknown</span></span> | <span data-ttu-id="90ca1-118">Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.</span><span class="sxs-lookup"><span data-stu-id="90ca1-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90ca1-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="90ca1-119">JSON representation</span></span>

<span data-ttu-id="90ca1-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="90ca1-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="90ca1-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="90ca1-121">Properties</span></span>
| <span data-ttu-id="90ca1-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90ca1-122">Property</span></span>     | <span data-ttu-id="90ca1-123">Typ</span><span class="sxs-lookup"><span data-stu-id="90ca1-123">Type</span></span>   |<span data-ttu-id="90ca1-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90ca1-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90ca1-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="90ca1-125">emptySuggestionsReason</span></span>|<span data-ttu-id="90ca1-126">String</span><span class="sxs-lookup"><span data-stu-id="90ca1-126">String</span></span>|<span data-ttu-id="90ca1-127">Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="90ca1-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="90ca1-128">Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="90ca1-128">Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="90ca1-129">Diese Eigenschaft ist eine leere Zeichenfolge, wenn die **meetingTimeSuggestions** -Eigenschaft alle Besprechungsvorschläge enthält.</span><span class="sxs-lookup"><span data-stu-id="90ca1-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="90ca1-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="90ca1-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="90ca1-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span><span class="sxs-lookup"><span data-stu-id="90ca1-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="90ca1-132">Ein Array von Besprechungsvorschlägen</span><span class="sxs-lookup"><span data-stu-id="90ca1-132">An array of meeting suggestions.</span></span>|

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