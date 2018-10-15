# <a name="chart-resource-type"></a>Chart-Ressourcentyp

Steht für ein Diagrammobjekt in einer Arbeitsmappe.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Chart abrufen](../api/chart_get.md) | [WorkbookChart](chart.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des Chart-Objekts.|
|[ChartSeries erstellen](../api/chart_post_series.md) |[WorkbookChartSeries](chartseries.md)| Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.|
|[Reihe auflisten](../api/chart_list_series.md) |[WorkbookChartSeries](chartseries.md)-Sammlung| Dient zum Abrufen einer ChartSeries-Objektsammlung.|
|[Aktualisieren](../api/chart_update.md) | [WorkbookChart](chart.md)   |Dient zum Aktualisieren des Chart-Objekts. |
|[Abbild](../api/chart_image.md)|Abbildung der base64-codierten Zeichenfolge|Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.|
|[Löschen](../api/chart_delete.md)|Keine|Löscht das Diagrammobjekt.|
|[Setdata](../api/chart_setdata.md)|Keine|Setzt die Quelldaten für das Diagramm zurück.|
|[Setposition](../api/chart_setposition.md)|Keine|Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.|
|[Liste](../api/chart_list.md) | [WorkbookChart](chart.md) -Sammlung |Dient zum Abrufen der Diagrammobjeksammlung. |
|[Itemat](../api/chartcollection_itemat.md)|[WorkbookChart](chart.md)|Ruft ein Diagramm anhand seiner Position in der Sammlung ab.|
|[Hinzufügen](../api/chartcollection_add.md)|[WorkbookChart](chart.md)|Erstellt ein neues Diagramm.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Höhe|double|Die Höhe des Diagrammobjekts (in Punkten).|
|ID|Zeichenfolge|Ruft ein Diagramm anhand seiner Position in der Sammlung ab. Schreibgeschützt.|
|links|double|Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).|
|Name|Zeichenfolge|Gibt den Namen eines Diagrammobjekts an.|
|oben|double|Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).|
|Breite|double|Die Breite des Diagrammobjekts (in Punkten).|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Achsen|[WorkbookChartAxes](chartaxes.md)|Die Achsen des Diagramms. Schreibgeschützt.|
|dataLabels|[WorkbookChartDataLabels](chartdatalabels.md)|Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.|
|Format|[WorkbookChartAreaFormat](chartareaformat.md)|Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.|
|legend|[WorkbookChartLegend](chartlegend.md)|Die Legende für das Diagramm. Schreibgeschützt.|
|series|[WorkbookChartSeries](chartseries.md)-Sammlung|Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.|
|title|[WorkbookChartTitle](charttitle.md)|Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.|
|Arbeitsblatt|[WorkbookWorksheet](worksheet.md)|Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->