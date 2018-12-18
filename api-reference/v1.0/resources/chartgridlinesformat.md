---
title: ChartGridlinesFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammgitternetzlinien.
author: lumine2008
ms.openlocfilehash: 61e75f644e70174bad04d5ae37b15cd07bc4d4bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328959"
---
# <a name="chartgridlinesformat-resource-type"></a>ChartGridlinesFormat-Ressourcentyp

Kapselt die Formateigenschaften für die Diagrammgitternetzlinien.


## <a name="methods"></a>Methoden
Keine

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|line|[WorkbookChartLineFormat](chartlineformat.md)|Stellt die Formatierung der Diagrammlinien dar. Schreibgeschützt.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->