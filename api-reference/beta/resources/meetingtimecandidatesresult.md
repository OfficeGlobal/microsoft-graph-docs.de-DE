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
# <a name="meetingtimecandidatesresult-resource-type"></a>Ressourcentyp meetingTimeCandidatesResult

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.

In der folgenden Tabelle finden Sie mögliche Gründe, aus denen findMeetingTimes keine Besprechungsvorschläge zurückgibt.

|**EmptySuggestionsHint Wert**|Gründe|
|:-----|:-----|
| attendeesUnavailable | Die Verfügbarkeit aller Teilnehmer ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Schwellenwert für die Besprechungskonfidenz. Dieser ist standardmäßig auf 50 % festgelegt. Dieser Grenzwert basiert auf der Teilnehmer Frei/Gebucht-Status für einer vorgeschlagenen Besprechung Zeitraum an, mit dem eines Teilnehmers kostenlose Status, Anwesenheit, Status unbekannt 50 % und gebucht-Status 0 % Wahrscheinlichkeit 100 % entspricht.|
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
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|emptySuggestionsHint|String|Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden. Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` und `unknown`.|
|meetingTimeSlots|[MeetingTimeCandidate](meetingtimecandidate.md) -Auflistung|Ein Array von Besprechungsvorschlägen|

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
