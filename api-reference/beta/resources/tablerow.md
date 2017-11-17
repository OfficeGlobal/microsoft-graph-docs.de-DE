# <a name="tablerow-resource-type"></a>TableRow-Ressourcentyp

Stellt eine Zeile in einer Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[TableRow abrufen](../api/tablerow_get.md) | [TableRow](tablerow.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableRow-Objekts.|
|[Update](../api/tablerow_update.md) | [TableRow](tablerow.md)    |Dient zum Aktualisieren des TableRow-Objekts. |
|[Range](../api/tablerow_range.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Zeile verknüpft ist.|
|[Delete](../api/tablerow_delete.md)|Keine|Löscht die Zeile aus der Tabelle.|
|[List](../api/tablerow_list.md) | [TableRow](tablerow.md)-Sammlung: |Dient zum Abrufen einer tableRow-Objektsammlung. |
|[Itemat](../api/tablerowcollection_itemat.md)|[TableRow](tablerow.md)|Ruft eine Zeile anhand ihrer Position in der Auflistung ab.|
|[Add](../api/tablerowcollection_add.md)|[TableRow](tablerow.md)|Fügt der Tabelle eine neue Zeile hinzu.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Index|int|Gibt die Indexnummer der Zeile in der Zeilenauflistung der Tabelle zurück. Nullindiziert. Schreibgeschützt.|
|values|json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->