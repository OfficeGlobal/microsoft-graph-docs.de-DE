# <a name="chartseries-resource-type"></a>ChartSeries-Ressourcentyp

Stellt eine Datenreihe in einem Diagramm dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartSeries abrufen](../api/chartseries_get.md) | [WorkbookChartSeries](chartseries.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartSeries-Objekts.|
|[ChartPoints erstellen](../api/chartseries_post_points.md) |[ChartPoints](chartpoint.md)| Dient zum Erstellen eines neuen ChartPoints durch Veröffentlichen in der Punktesammlung.|
|[Punkte auflisten](../api/chartseries_list_points.md) |[ChartPoints](chartpoint.md)-Sammlung| Dient zum Abrufen einer ChartPoints-Objektsammlung.|
|[Aktualisieren](../api/chartseries_update.md) | [WorkbookChartSeries](chartseries.md) |Dient zum Aktualisieren des ChartSeries-Objekts. |
|[Liste](../api/chartseries_list.md) | [WorkbookChartSeries](chartseries.md)-Auflistung |Dient zum Abrufen der chartSeries-Objektsammlung. |
|[Itemat](../api/chartseriescollection_itemat.md)|[WorkbookChartSeries](chartseries.md)|Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Name|string|Gibt den Namen einer Datenreihe in einem Diagramm an.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[WorkbookChartSeriesFormat](chartseriesformat.md)|Stellt die Formatierung für eine Diagrammdatenreihe dar, einschließlich Füllung und Linienformatierung. Schreibgeschützt.|
|points|[WorkbookChartPoint](chartpoint.md)-Auflistung|Stellt eine Sammlung aller Punkte in der Datenreihe dar. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->