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
# <a name="meetingtimesuggestionsresult-resource-type"></a>Ressourcentyp „meetingTimeSuggestionsResult“

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Sammlung von Besprechungs Vorschlägen, falls vorhanden, und der Grund, wenn dies nicht der Fall ist.

In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.

|**Wert für „emptySuggestionsReason“**|**Gründe**|
|:-----|:-----|
| attendeesUnavailable | Die Verfügbarkeit aller Teilnehmer ist bekannt, aber nicht genügend Teilnehmer stehen zur Verfügung, um den Vertrauens Schwellenwert für die [Besprechung](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) zu erreichen, der standardmäßig 50% für einen beliebigen Zeitraum beträgt.|
| attendeesUnavailableOrUnknown | Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.|
| locationsUnavailable | Die **IsRequired** -Eigenschaft des **timeconstraint** -Parameters ist als true angegeben, und es sind jedoch keine Speicherorte an den berechneten Zeitschlitzen verfügbar. |
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
|emptySuggestionsReason|String|Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden. Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` und `unknown`. Diese Eigenschaft ist eine leere Zeichenfolge, wenn die **meetingTimeSuggestions** -Eigenschaft alle Besprechungsvorschläge enthält.|
|meetingTimeSuggestions|[meetingTimeSuggestion](meetingtimesuggestion.md) collection|Ein Array von Besprechungsvorschlägen|

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