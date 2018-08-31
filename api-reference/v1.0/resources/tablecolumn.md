# <a name="tablecolumn-resource-type"></a>TableColumn-Ressourcentyp

Stellt eine Spalte in einer Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[TableColumn abrufen](../api/tablecolumn_get.md) | [WorkbookTableColumn](tablecolumn.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableColumn-Objekts.|
|[Aktualisieren](../api/tablecolumn_update.md) | [WorkbookTableColumn](tablecolumn.md) |TableColumn-Objekt aktualisieren. |
|[Databodyrange](../api/tablecolumn_databodyrange.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit dem Datenteil der Spalte verknüpft ist.|
|[Headerrowrange](../api/tablecolumn_headerrowrange.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit der Überschriftenzeile der Spalte verknüpft ist.|
|[Bereich](../api/tablecolumn_range.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Spalte verknüpft ist.|
|[Totalrowrange](../api/tablecolumn_totalrowrange.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit der Ergebniszeile der Spalte verknüpft ist.|
|[Löschen](../api/tablecolumn_delete.md)|Keine|Löscht die Spalte aus der Tabelle.|
|[Liste](../api/tablecolumn_list.md) | [WorkbookTableColumn](tablecolumn.md) -Sammlung |TableColumn-Objekt-Sammlung abrufen. |
|[Itemat](../api/tablecolumncollection_itemat.md)|[WorkbookTableColumn](tablecolumn.md)|Ruft eine Spalte anhand ihrer Position in der Auflistung ab.|
|[Hinzufügen](../api/tablecolumncollection_add.md)|[WorkbookTableColumn](tablecolumn.md)|Fügt der Tabelle eine neue Spalte hinzu.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge|Gibt einen eindeutigen Schlüssel an, der die Spalte in der Tabelle angibt. Diese Eigenschaft sollte als nicht transparenter Zeichenfolgenwert interpretiert werden und sollte nicht in einen anderen Typ ausgewertet werden. Schreibgeschützt.|
|Index|int|Gibt die Indexnummer der Spalte in der Spaltenauflistung der Tabelle zurück. Nullindiziert. Schreibgeschützt.|
|Name|Zeichenfolge|Gibt den Namen der Tabellenspalte zurück. Schreibgeschützt.|
|Werte|Json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Filter|[WorkbookFilter](filter.md)|Ruft den auf die Spalte angewendeten Filter ab. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
