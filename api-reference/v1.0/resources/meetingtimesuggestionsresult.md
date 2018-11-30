---
title: Ressourcentyp „meetingTimeSuggestionsResult“
description: Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.
ms.openlocfilehash: 5504971618e6b8f6fdb82b203142e84c23c595f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017034"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>Ressourcentyp „meetingTimeSuggestionsResult“

Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.

In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.

|**Wert für „emptySuggestionsReason“**|**Gründe**|
|:-----|:-----|
| attendeesUnavailable | Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die [Besprechungskonfidenz](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion). Dieser ist standardmäßig auf 50 % festgelegt.|
| attendeesUnavailableOrUnknown | Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.|
| locationsUnavailable | Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar. |
| organizerUnavailable | Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar. |
| unknown | Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

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
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|emptySuggestionsReason|String|Einen Grund für die Besprechungsvorschläge nicht zurückgeben. Die möglichen Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, oder `unknown`. Diese Eigenschaft ist eine leere Zeichenfolge, wenn die **MeetingTimeSuggestions** -Eigenschaft Besprechungsvorschläge enthält.|
|meetingTimeSuggestions|[meetingTimeSuggestion](meetingtimesuggestion.md) collection|Ein Array von Besprechungsvorschlägen|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->