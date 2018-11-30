---
title: Ressourcentyp „meetingTimeSuggestionsResult“
description: Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.
ms.openlocfilehash: 2c6cb28ea0ec899e693300b321c652fb814582f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064776"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="66e3f-103">Ressourcentyp „meetingTimeSuggestionsResult“</span><span class="sxs-lookup"><span data-stu-id="66e3f-103">meetingTimeSuggestionsResult resource type</span></span>

> <span data-ttu-id="66e3f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66e3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66e3f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66e3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66e3f-106">Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="66e3f-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="66e3f-107">In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="66e3f-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="66e3f-108">**Wert für „emptySuggestionsReason“**</span><span class="sxs-lookup"><span data-stu-id="66e3f-108">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="66e3f-109">**Gründe**</span><span class="sxs-lookup"><span data-stu-id="66e3f-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="66e3f-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="66e3f-110">attendeesUnavailable</span></span> | <span data-ttu-id="66e3f-111">Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die [Besprechungskonfidenz](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion). Dieser ist standardmäßig auf 50 % festgelegt.</span><span class="sxs-lookup"><span data-stu-id="66e3f-111">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="66e3f-112">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="66e3f-112">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="66e3f-p102">Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.</span><span class="sxs-lookup"><span data-stu-id="66e3f-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="66e3f-115">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="66e3f-115">locationsUnavailable</span></span> | <span data-ttu-id="66e3f-116">Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar.</span><span class="sxs-lookup"><span data-stu-id="66e3f-116">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="66e3f-117">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="66e3f-117">organizerUnavailable</span></span> | <span data-ttu-id="66e3f-118">Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="66e3f-118">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="66e3f-119">unknown</span><span class="sxs-lookup"><span data-stu-id="66e3f-119">unknown</span></span> | <span data-ttu-id="66e3f-120">Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.</span><span class="sxs-lookup"><span data-stu-id="66e3f-120">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66e3f-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66e3f-121">JSON representation</span></span>

<span data-ttu-id="66e3f-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66e3f-122">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="66e3f-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66e3f-123">Properties</span></span>
| <span data-ttu-id="66e3f-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66e3f-124">Property</span></span>     | <span data-ttu-id="66e3f-125">Typ</span><span class="sxs-lookup"><span data-stu-id="66e3f-125">Type</span></span>   |<span data-ttu-id="66e3f-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66e3f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66e3f-127">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="66e3f-127">emptySuggestionsReason</span></span>|<span data-ttu-id="66e3f-128">String</span><span class="sxs-lookup"><span data-stu-id="66e3f-128">String</span></span>|<span data-ttu-id="66e3f-p103">Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden. Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` oder `unknown`. Diese Eigenschaft ist eine leere Zeichenfolge, wenn die Eigenschaft **meetingTimeSuggestions** keine Besprechungsvorschläge enthält.</span><span class="sxs-lookup"><span data-stu-id="66e3f-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="66e3f-132">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="66e3f-132">meetingTimeSuggestions</span></span>|<span data-ttu-id="66e3f-133">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span><span class="sxs-lookup"><span data-stu-id="66e3f-133">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="66e3f-134">Ein Array von Besprechungsvorschlägen</span><span class="sxs-lookup"><span data-stu-id="66e3f-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->