# <a name="tablerow-resource-type"></a>TableRow-Ressourcentyp

Stellt eine Zeile in einer Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[TableRow abrufen](../api/tablerow_get.md) | [WorkbookTableRow](tablerow.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableRow-Objekts.|
|[Aktualisieren](../api/tablerow_update.md) | [WorkbookTableRow](tablerow.md)  |Dient zum Aktualisieren des TableRow-Objekts. |
|[Bereich](../api/tablerow_range.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Zeile verknüpft ist.|
|[Löschen](../api/tablerow_delete.md)|Keine|Löscht die Zeile aus der Tabelle.|
|[Liste](../api/tablerow_list.md) | [WorkbookTableRow](tablerow.md)-Sammlung |Dient zum Abrufen einer tableRow-Objektsammlung. |
|[Itemat](../api/tablerowcollection_itemat.md)|[WorkbookTableRow](tablerow.md)|Ruft eine Zeile anhand ihrer Position in der Auflistung ab.|
|[Hinzufügen](../api/tablerowcollection_add.md)|[WorkbookTableRow](tablerow.md)|Fügt der Tabelle eine neue Zeile hinzu.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Index|int|Gibt die Indexnummer der Zeile in der Zeilenauflistung der Tabelle zurück. Nullindiziert. Schreibgeschützt.|
|values|Json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
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