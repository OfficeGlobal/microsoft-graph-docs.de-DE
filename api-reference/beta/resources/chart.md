# <a name="chart-resource-type"></a>Chart-Ressourcentyp

Steht für ein Diagrammobjekt in einer Arbeitsmappe.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Chart abrufen](../api/chart_get.md) | [Chart](chart.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chart-Objekts.|
|[ChartSeries erstellen](../api/chart_post_series.md) |[ChartSeries](chartseries.md)| Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.|
|[Reihe auflisten](../api/chart_list_series.md) |[ChartSeries-Sammlung](chartseries.md)| Dient zum Abrufen einer ChartSeries-Objektsammlung.|
|[Update](../api/chart_update.md) | [Chart](chart.md)    |Dient zum Aktualisieren des Chart-Objekts. |
|[Image](../api/chart_image.md)|Abbildung der base64-codierten Zeichenfolge|Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.|
|[Löschen](../api/chart_delete.md)|Keine|Löscht das Diagrammobjekt.|
|[Setdata](../api/chart_setdata.md)|Keine|Setzt die Quelldaten für das Diagramm zurück.|
|[Setposition](../api/chart_setposition.md)|Keine|Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.|
|[List](../api/chart_list.md) | [Diagrammsammlung](chart.md) |Dient zum Abrufen der Diagrammobjeksammlung. |
|[Itemat](../api/chartcollection_itemat.md)|[Chart](chart.md)|Ruft ein Diagramm anhand seiner Position in der Sammlung ab.|
|[Add](../api/chartcollection_add.md)|[Chart](chart.md)|Erstellt ein neues Diagramm.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|height|double|Die Höhe des Diagrammobjekts (in Punkten).|
|id|string|Ruft ein Diagramm anhand seiner Position in der Sammlung ab. Schreibgeschützt.|
|left|double|Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).|
|name|string|Gibt den Namen eines Diagrammobjekts an.|
|top|double|Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).|
|width|double|Die Breite des Diagrammobjekts (in Punkten).|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Achsen|[ChartAxes](chartaxes.md)|Die Achsen des Diagramms. Schreibgeschützt.|
|dataLabels|[ChartDataLabels](chartdatalabels.md)|Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.|
|Format|[ChartAreaFormat](chartareaformat.md)|Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.|
|Legende|[ChartLegend](chartlegend.md)|Die Legende für das Diagramm. Schreibgeschützt.|
|Datenreihe|[ChartSeries-Sammlung](chartseries.md)|Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.|
|title|[ChartTitle](charttitle.md)|Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.|
|Arbeitsblatt|[Worksheet](worksheet.md)|Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
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