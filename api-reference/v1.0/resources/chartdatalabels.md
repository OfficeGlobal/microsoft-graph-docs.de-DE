---
title: ChartDataLabels-Ressourcentyp
description: Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.
author: lumine2008
ms.openlocfilehash: 39c95d0849d398df7d57f676cc392c157e6f43f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339053"
---
# <a name="chartdatalabels-resource-type"></a>ChartDataLabels-Ressourcentyp

Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartDataLabels abrufen](../api/chartdatalabels-get.md) | [WorkbookChartDataLabels](chartdatalabels.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.|
|[Update](../api/chartdatalabels-update.md) | [WorkbookChartDataLabels](chartdatalabels.md) |Dient zum Aktualisieren des ChartDataLabels-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|position|string|DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt. Die möglichen Werte sind: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.|
|Separator|string|Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.|
|showBubbleSize|boolean|Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.|
|showCategoryName|boolean|Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.|
|showLegendKey|boolean|Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.|
|showPercentage|boolean|Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.|
|showSeriesName|boolean|Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.|
|showValue|boolean|Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Format|[WorkbookChartDataLabelFormat](chartdatalabelformat.md)|Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->