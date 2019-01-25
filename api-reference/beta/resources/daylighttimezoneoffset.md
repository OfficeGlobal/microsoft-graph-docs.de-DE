---
title: daylightTimeZoneOffset-Ressourcentyp
description: Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.
localization_priority: Normal
ms.openlocfilehash: 160163d6f574eb75746fa751e383c06696006e43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507586"
---
# <a name="daylighttimezoneoffset-resource-type"></a>daylightTimeZoneOffset-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.

Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:

- **bias** ist 300
- **daylightBias** ist -100
- **dayOccurrence** ist 4
- **dayOfWeek** ist „Sonntag“
- **month** ist 5
- **time** ist  02:00:00 _ **year** ist 0. Dies bedeutet, dass die Zeit während der Sommerzeit +300-100=200 Minuten vor der UTC-Zeit liegt. Der Übergang von Sommerzeit zu Standardzeit findet jedes Jahr um 2 Uhr am vierten Sonntag im Mai stattfindet.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| daylightBias | Edm.Int32 | Der Zeitversatz der Sommerzeit von der Koordinierten Weltzeit (UTC). Dieser Wert wird in Minuten angegeben.  |
| dayOccurrence | Edm.Int32 | Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt. |
| dayOfWeek | string | Stellt den Wochentag dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt. |
| Monat | Edm.Int32 | Stellt den Monat dar, in dem der Übergang von Standardzeit zu Sommerzeit erfolgt. |
| Uhrzeit | Edm.TimeOfDay | Stellt die Uhrzeit dar, zu der der Übergang von Standardzeit zu Sommerzeit erfolgt. |
| Jahr | Edm.Int32 | Stellt dar, wie häufig der Wechsel von Standardzeit zu Sommerzeit in einem Jahr erfolgt. Der Wert 0 bedeutet z. B. jedes Jahr.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/daylighttimezoneoffset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
