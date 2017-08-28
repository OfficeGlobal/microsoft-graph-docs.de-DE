# <a name="table-resource-type"></a>Table-Ressourcentyp

Stellt eine Excel-Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Tabelle abrufen](../api/table_get.md) | [Table](table.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des table-Objekts.|
|[TableColumn erstellen](../api/table_post_columns.md) |[TableColumn](tablecolumn.md)| Dient zum Erstellen einer neuen TableColumn durch Veröffentlichen in der Diagrammsammlung.|
|[Spalten auflisten](../api/table_list_columns.md) |[TableColumn](tablecolumn.md)-Sammlung| Dient zum Abrufen einer TableColumn-Objektsammlung.|
|[TableRow erstellen](../api/table_post_rows.md) |[TableRow](tablerow.md)| Dient zum Erstellen einer neuen TableRow durch Veröffentlichen in der Zeilensammlung.|
|[Zeilen auflisten](../api/table_list_rows.md) |[TableRow](tablerow.md)-Sammlung| Dient zum Abrufen einer TableRow-Objektsammlung.|
|[Update](../api/table_update.md) | [Table](table.md)   |Dient zum Aktualisieren des Table-Objekts. |
|[Databodyrange](../api/table_databodyrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit dem Datenteil der Tabelle verknüpft ist.|
|[Headerrowrange](../api/table_headerrowrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der Kopfzeile der Tabelle verknüpft ist.|
|[Range](../api/table_range.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Tabelle verknüpft ist.|
|[Totalrowrange](../api/table_totalrowrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der Ergebniszeile der Tabelle verknüpft ist.|
|[Clearfilters](../api/table_clearfilters.md)|Keine|Löscht alle Filter, die derzeit in der Tabelle verwendet werden.|
|[Converttorange](../api/table_converttorange.md)|[Range](range.md)|Wandelt die Tabelle in einen normalen Bereich von Zellen um. Alle Daten werden beibehalten.|
|[Delete](../api/table_delete.md)|Keine|Löscht die Tabelle.|
|[Reapplyfilters](../api/table_reapplyfilters.md)|Keine|Wendet alle Filter erneut an, die derzeit in der Tabelle vorhanden sind.|
|[List](../api/table_list.md) | [Tabellensammlung](table.md) |Dient zum Abrufen einer Tabellenobjektsammlung. |
|[Add](../api/tablecollection_add.md)|[Table](table.md)|Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|int|Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn die Tabelle umbenannt wird. Schreibgeschützt.|
|name|string|Der Name der Tabelle.|
|showHeaders|boolean|Gibt an, ob die Kopfzeile sichtbar oder nicht sichtbar ist. Dieser Wert kann festgelegt werden, um die Kopfzeile anzuzeigen, oder sie zu entfernen.|
|showTotals|boolean|Gibt an, ob die Ergebniszeile sichtbar ist oder nicht. Dieser Wert kann so festgelegt werden, dass die Ergebniszeile angezeigt oder ausgeblendet wird.|
|style|string|Konstanter Wert, der das Tabellenformat darstellt. Die folgenden Werte sind möglich: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. Es kann ebenfalls eine in der Arbeitsmappe vorhandene benutzerdefinierte Formatierung angegeben werden.|
|highlightFirstColumn|Boolean|Gibt an, ob die erste Spalte spezielle Formatierung enthält.   |
|highlightLastColumn|Boolean|Gibt an, ob die letzte Spalte spezielle Formatierung enthält. |
|showBandedColumns|Boolean|Gibt an, ob die Spalten gebänderte Formatierung aufweisen, wobei ungerade Spalten anders hervorgehoben werden als gerade, um die Tabelle leichter lesbar zu machen.   |
|showBandedRows|Boolean|Gibt an, ob die Zeilen gebänderte Formatierung aufweisen, wobei ungerade Zeilen anders hervorgehoben werden als gerade, um die Tabelle leichter lesbar zu machen.    |
|showFilterButton|Boolean|Gibt an, ob die Filterschaltflächen am oberen Rand jedes Spaltenheaders sichtbar sind. Diese Einstellung ist nur zulässig, wenn die Tabelle eine Kopfzeile enthält.   |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|columns|[TableColumn](tablecolumn.md)-Sammlung|Stellt eine Auflistung aller Spalten in der Tabelle dar. Schreibgeschützt.|
|rows|[TableRow](tablerow.md)-Sammlung|Stellt eine Auflistung aller Zeilen in der Tabelle dar. Schreibgeschützt.|
|sort|[TableSort](tablesort.md)|Stellt die Sortierung für die Tabelle dar. Schreibgeschützt.|
|Arbeitsblatt|[Worksheet](worksheet.md)|Das Arbeitsblatt, das die aktuelle Tabelle enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.table"
}-->

```json
{
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "id": "String (identifier)",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
