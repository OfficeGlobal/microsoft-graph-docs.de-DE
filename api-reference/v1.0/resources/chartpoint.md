# <a name="chartpoint-resource-type"></a>ChartPoint-Ressourcentyp

Stellt einen Punkt einer Datenreihe in einem Diagramm dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartPoint abrufen](../api/chartpoint_get.md) | [WorkbookChartPoint](chartpoint.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.|
|[Liste](../api/chartpoint_list.md) | [WorkbookChartPoint](chartpoint.md)-Sammlung |Dient zum Abrufen der chartPoint-Objektsammlung. |
|[ItemAt](../api/chartpointscollection_itemat.md)|[WorkbookChartPoint](chartpoint.md)|Abrufen eines Punkts anhand seiner Position in der Datenreihe.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Wert|Json|Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.|
|id|Zeichenfolge|Eindeutiger Bezeichner|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Format|[WorkbookChartPointFormat](chartpointformat.md)|Kapselt die Formateigenschaften eines Diagrammpunkts ein. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->