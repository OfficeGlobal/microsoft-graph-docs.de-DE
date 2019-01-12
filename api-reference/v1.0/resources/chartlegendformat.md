---
title: ChartLegendFormat-Ressourcentyp
description: Kapselt die Formateigenschaften einer Diagrammlegende.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f35f7a3cf152024bd89f03daf8be98ec1d8066b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972068"
---
# <a name="chartlegendformat-resource-type"></a>ChartLegendFormat-Ressourcentyp

Kapselt die Formateigenschaften einer Diagrammlegende.


## <a name="methods"></a>Methoden
Keine

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.|
|Schriftart|[WorkbookChartFont](chartfont.md)|Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. einer Diagrammlegende dar. Schreibgeschützt.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
