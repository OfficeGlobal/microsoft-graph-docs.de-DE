# <a name="chartpoint-resource-type"></a>ChartPoint-Ressourcentyp

Stellt einen Punkt einer Datenreihe in einem Diagramm dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartPoint abrufen](../api/chartpoint_get.md) | [ChartPoint](chartpoint.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.|
|[List](../api/chartpoint_list.md) | [ChartPoint-Sammlung](chartpoint.md) |Dient zum Abrufen der ChartPoint-Objektsammlung. |
|[Itemat](../api/chartpointscollection_itemat.md)|[ChartPoint](chartpoint.md)|Abrufen eines Punkts anhand seiner Position in der Datenreihe.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|value|object|Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Format|[ChartPointFormat](chartpointformat.md)|Kapselt die Formateigenschaften eines Diagrammpunkts. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
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