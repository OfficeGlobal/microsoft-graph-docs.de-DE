---
title: Ressourcentyp „meetingTimeSuggestion“
description: 'Ein Besprechungs Vorschlag, der Informationen wie Besprechungszeit, Anwesenheits Wahrscheinlichkeit, einzelne '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 379bb4ac4be8e2d8d1bec494cf4d573550d46b55
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057029"
---
# <a name="meetingtimesuggestion-resource-type"></a>Ressourcentyp „meetingTimeSuggestion“

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Besprechungsvorschlag mit Informationen wie dem Besprechungstermin, der Teilnahmewahrscheinlichkeit, der individuellen Verfügbarkeit und den verfügbaren Besprechungsorten

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.locationDataModel"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.meetingTimeSlotDataModel"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attendeeAvailability|[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md) -Sammlung|Ein Array, das den Verfügbarkeitsstatus jedes Teilnehmers für den betreffenden Besprechungsvorschlag anzeigt|
|confidence|Double|Ein Prozentwert, der angibt, wie hoch die Wahrscheinlichkeit ist, dass alle Teilnehmer teilnehmen können|
|locations|[locationDataModel](locationdatamodel.md) -Sammlung|Ein Array, das den Namen und den geografischen Ort jedes Besprechungsorts für den betreffenden Besprechungsvorschlag angibt|
|meetingTimeSlot|[meetingTimeSlotDataModel](meetingtimeslotdatamodel.md)|Ein für die Besprechung vorgeschlagenes Zeitfenster|
|organizerAvailability|availabilityStatus| Die Verfügbarkeit des Besprechungsorganisators für diesen Besprechungsvorschlag. Mögliche Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`und `unknown`.|
|suggestionReason|String|Grund, aus dem der betreffende Besprechungstermin vorgeschlagen wurde|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
