---
title: ChartAxisFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
ms.openlocfilehash: e503b4e62ef7907943f10a395f12eb5d86c1928f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359458"
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