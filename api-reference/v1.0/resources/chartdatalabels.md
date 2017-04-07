# <a name="chartdatalabels-resource-type"></a>ChartDataLabels-Ressourcentyp

Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartDataLabels abrufen](../api/chartdatalabels_get.md) | [ChartDataLabels](chartdatalabels.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.|
|[Update](../api/chartdatalabels_update.md) | [ChartDataLabels](chartdatalabels.md)    |Dient zum Aktualisieren des ChartDataLabels-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Position|string|DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt. Mögliche Werte: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.|
|Separator|string|Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.|
|showBubbleSize|boolean|Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.|
|showCategoryName|boolean|Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.|
|showLegendKey|boolean|Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.|
|showPercentage|boolean|Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.|
|showSeriesName|boolean|Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.|
|showValue|boolean|Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Format|[ChartDataLabelFormat](chartdatalabelformat.md)|Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
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