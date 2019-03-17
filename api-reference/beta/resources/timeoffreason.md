---
title: timeOffReason-Ressourcentyp
description: Ein gültiger Grund, die Zeitdauer im Zeitplan zu übernehmen.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657532"
---
# <a name="timeoffreason-resource-type"></a>timeOffReason-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein gültiger Grund für eine [timeOff](timeoff.md) -Instanz in einem [Zeitplan](schedule.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[TimeOffReason erstellen](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | Erstellen Sie eine `timeOffReason`neue.|
|[TimeOffReason aufListen](../api/schedule-list-timeoffreasons.md) | [timeOffReason](timeoffreason.md) -Sammlung | Abrufen der Liste der `timeOffReasons` in einem Zeitplan.|
|[TimeOffReason abrufen](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | Rufen Sie `timeOffReason` eine nach ID ab.|
|[TimeOffReason ersetzen](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | Ersetzen Sie `timeOffReason`a.|
|[TimeOffReason löschen](../api/timeoffreason-delete.md) | None | Als `timeOffReason` inaktiv markieren.|

## <a name="properties"></a>Eigenschaften
|Name          |Typ           |Beschreibung                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |ID des `timeOffReason`.|
| displayName               | `string`                  | Der Name des `timeOffReason`. Erforderlich. |
| icontype | `enum`   | Unterstützte Symboltypen: None; Auto Kalender ausgeführt Ebene FirstAid Arzt notWorking; Takt juryDuty; weltweit Tasse Telefon Wetter Schirm Piggybank Hund Kuchen trafficCone; PIN sonnigen. Erforderlich. |
| isActive          |`bool`      | Gibt an, `timeOffReason` ob die verwendet werden kann, wenn neue Entitäten erstellt oder vorhandene aktualisiert werden. Erforderlich. |
| createdDateTime       |`DateTimeOffset`        |Der Zeitstempel, an dem `timeOffReason` dieser zuerst erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. |
| lastModifiedDateTime      |`DateTimeOffset`         |Der Zeitstempel, an dem `timeOffReason` dieser zuletzt aktualisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. |
| lastModifiedBy        |`microsoft.graph.identitySet`        |Die Identität, die zuletzt aktualisiert `timeOffReason`hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
