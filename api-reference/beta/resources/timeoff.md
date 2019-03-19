---
title: timeOff-Ressourcentyp
description: Eine nicht-Arbeitseinheit im Zeitplan.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676989"
---
# <a name="timeoff-resource-type"></a>timeOff-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine nicht-Arbeitseinheit im Zeitplan.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[TimeOff erstellen](../api/schedule-post-timesoff.md) | [timeOff](timeOff.md) | Dient zum Erstellen eines neuen Objekts vom Typ `timeOff`.|
|[AufListen von zeitOffs](../api/schedule-list-timesoff.md) | [timeOff](timeOff.md) -Sammlung | Rufen Sie die Liste `timeOff` der Objekte in diesem Zeitplan ab.|
|[TimeOff abrufen](../api/timeoff-get.md) | [timeOff](timeOff.md) | Rufen Sie `timeOff` eine nach ID ab.|
|[TimeOff ersetzen](../api/timeoff-put.md) | [timeOff](timeOff.md) | Ersetzen Sie `timeOff`a.|
|[TimeOff löschen](../api/timeoff-delete.md) | Keine | Löschen Sie `timeOff` eine aus dem Zeitplan.|

## <a name="properties"></a>Eigenschaften
|Name          |Typ           |Beschreibung                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID des `timeOff`.|
| userId            |`string`      |Die ID des Benutzers, der dem `timeOff`zugewiesen ist. Erforderlich.|
| sharedTimeOff     |[timeOffItem](timeoffitem.md)  |Die freigegebene `timeOff` Version dieses, die sowohl von Mitarbeitern als auch von Managern angezeigt werden kann. Erforderlich.|
| draftTimeOff      |[timeOffItem](timeoffitem.md)        |Die Entwurfsversion dieses `timeOff` , die von Managern angezeigt werden kann. Erforderlich.|
| createdDateTime       |`DateTimeOffset`        |Der Zeitstempel, an dem `timeOff` dieser zuerst erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. |
| lastModifiedDateTime      |`DateTimeOffset`        |Der Zeitstempel, an dem `timeOff` dieser zuletzt aktualisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. |
| lastModifiedBy        |`microsoft.graph.identitySet`        |Die Identität, die zuletzt aktualisiert `timeOff`hat. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
