---
title: ChartPointFormat-Ressourcentyp
description: Stellt das Formatierungsobjekt für Diagrammpunkte dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 5923252a9fce47eedc58751def301b6515560ddd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883342"
---
# <a name="chartpointformat-resource-type"></a>ChartPointFormat-Ressourcentyp

Stellt das Formatierungsobjekt für Diagrammpunkte dar.


## <a name="methods"></a>Methoden
Keine

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|Stellt die Füllung eines Diagramms dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
