---
title: ChartDataLabelFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 586b201b0bcc70765fb68aa7736664f493f5539b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876923"
---
# <a name="chartdatalabelformat-resource-type"></a>ChartDataLabelFormat-Ressourcentyp

Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.


## <a name="methods"></a>Methoden
Keine

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|Stellt die Füllung der aktuellen Diagrammdatenbeschriftung dar. Schreibgeschützt.|
|Schriftart|[WorkbookChartFont](chartfont.md)|Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für eine Diagrammdatenbeschriftung dar. Schreibgeschützt.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
