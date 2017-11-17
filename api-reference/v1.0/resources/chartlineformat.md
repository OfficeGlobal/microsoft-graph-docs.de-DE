# <a name="chartlineformat-resource-type"></a>ChartLineFormat-Ressourcentyp

Kapselt die Formatierungsoptionen für Linienelemente.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartLineFormat abrufen](../api/chartlineformat_get.md) | [ChartLineFormat](chartlineformat.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.|
|[Update](../api/chartlineformat_update.md) | [ChartLineFormat](chartlineformat.md)    |Dient zum Aktualisieren des ChartLineFormat-Objekts. |
|[Clear](../api/chartlineformat_clear.md)|Keine|Löschen der Linienformatierung eines Diagrammelements.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|color|string|HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->