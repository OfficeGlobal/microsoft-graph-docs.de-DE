---
title: ChartAxisFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92258887c9646890ee63d14aebcd32ada7a8aaa6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952111"
---
# <a name="chartaxisformat-resource-type"></a>ChartAxisFormat-Ressourcentyp

Kapselt die Formateigenschaften für die Diagrammachse.


## <a name="methods"></a>Methoden
Keine
## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Schriftart|[WorkbookChartFont](chartfont.md)|Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammachsenelement dar. Schreibgeschützt.|
|line|[WorkbookChartLineFormat](chartlineformat.md)|Stellt die Formatierung der Diagrammlinien dar. Schreibgeschützt.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
