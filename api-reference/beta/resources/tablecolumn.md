# <a name="tablecolumn-resource-type"></a>TableColumn-Ressourcentyp

Stellt eine Spalte in einer Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[TableColumn abrufen](../api/tablecolumn_get.md) | [TableColumn](tablecolumn.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableColumn-Objekts.|
|[Update](../api/tablecolumn_update.md) | [TableColumn](tablecolumn.md)    |Dient zum Aktualisieren des TableColumn-Objekts. |
|[Databodyrange](../api/tablecolumn_databodyrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit dem Datenteil der Spalte verknüpft ist.|
|[Headerrowrange](../api/tablecolumn_headerrowrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der Überschriftenzeile der Spalte verknüpft ist.|
|[Range](../api/tablecolumn_range.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Spalte verknüpft ist.|
|[Totalrowrange](../api/tablecolumn_totalrowrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der Ergebniszeile der Spalte verknüpft ist.|
|[Delete](../api/tablecolumn_delete.md)|Keine|Löscht die Spalte aus der Tabelle.|
|[List](../api/tablecolumn_list.md) | [TableColumn](tablecolumn.md)-Sammlung |Dient zum Abrufen der tableColumn-Objektsammlung. |
|[Itemat](../api/tablecolumncollection_itemat.md)|[TableColumn](tablecolumn.md)|Ruft eine Spalte anhand ihrer Position in der Auflistung ab.|
|[Add](../api/tablecolumncollection_add.md)|[TableColumn](tablecolumn.md)|Fügt der Tabelle eine neue Spalte hinzu.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|int|Gibt einen eindeutigen Schlüssel an, der die Spalte in der Tabelle angibt. Schreibgeschützt.|
|Index|int|Gibt die Indexnummer der Spalte in der Spaltenauflistung der Tabelle zurück. Nullindiziert. Schreibgeschützt.|
|name|string|Gibt den Namen der Tabellenspalte zurück. Schreibgeschützt.|
|values|json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Filter|[Filter](filter.md)|Ruft den auf die Salte angewendeten Filter ab. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->