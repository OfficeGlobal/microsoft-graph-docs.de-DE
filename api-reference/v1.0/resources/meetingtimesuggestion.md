---
title: Ressourcentyp „meetingTimeSuggestion“
description: 'Ein besprechungsvorschlag, das Informationen wie Besprechungszeit, Anwesenheit Wahrscheinlichkeit, einzelne enthält '
localization_priority: Normal
ms.openlocfilehash: d1cca365c66c114063fbf859e241a5d9a81303e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845997"
---
# <a name="meetingtimesuggestion-resource-type"></a>Ressourcentyp „meetingTimeSuggestion“

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
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attendeeAvailability|[attendeeAvailability](attendeeavailability.md) collection|Ein Array, das den Verfügbarkeitsstatus jedes Teilnehmers für den betreffenden Besprechungsvorschlag anzeigt|
|confidence|Double|Ein Prozentwert, der angibt, wie hoch die Wahrscheinlichkeit ist, dass alle Teilnehmer teilnehmen können|
|locations|[location](location.md)-Sammlung|Ein Array, das den Namen und den geografischen Ort jedes Besprechungsorts für den betreffenden Besprechungsvorschlag angibt|
|meetingTimeSlot|[timeSlot](timeslot.md)|Ein für die Besprechung vorgeschlagenes Zeitfenster|
|organizerAvailability|freeBusyStatus| Verfügbarkeit der Organisator der Besprechung für diese besprechungsvorschlag. Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|suggestionReason|String|Grund, aus dem der betreffende Besprechungstermin vorgeschlagen wurde|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
