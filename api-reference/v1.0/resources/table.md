# <a name="table-resource-type"></a>Table-Ressourcentyp

Stellt eine Excel-Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Tabelle abrufen](../api/table_get.md) | [WorkbookTable](table.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des table-Objekts.|
|[TableColumn erstellen](../api/table_post_columns.md) |[WorkbookTableColumn](tablecolumn.md)| Dient zum Erstellen einer neuen TableColumn durch Veröffentlichen in der Diagrammsammlung.|
|[Spalten auflisten](../api/table_list_columns.md) |[WorkbookTableColumn](tablecolumn.md) -Sammlung| Dient zum Abrufen einer TableColumn-Objektsammlung.|
|[TableRow erstellen](../api/table_post_rows.md) |[WorkbookTableRow](tablerow.md)| Dient zum Erstellen einer neuen TableRow durch Veröffentlichen in der Zeilensammlung.|
|[Zeilen auflisten](../api/table_list_rows.md) |[WorkbookTableRow](tablerow.md) -Sammlung| Dient zum Abrufen einer TableRow-Objektsammlung.|
|[Aktualisieren](../api/table_update.md) | [WorkbookTable](table.md)   |Dient zum Aktualisieren des Table-Objekts. |
|[Databodyrange](../api/table_databodyrange.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit dem Datenteil der Tabelle verknüpft ist.|
|[Headerrowrange](../api/table_headerrowrange.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit der Kopfzeile der Tabelle verknüpft ist.|
|[Bereich](../api/table_range.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Tabelle verknüpft ist.|
|[Totalrowrange](../api/table_totalrowrange.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das mit der Ergebniszeile der Tabelle verknüpft ist.|
|[Clearfilters](../api/table_clearfilters.md)|Keine|Löscht alle Filter, die derzeit in der Tabelle verwendet werden.|
|[Converttorange](../api/table_converttorange.md)|[Bereich](range.md)|Wandelt die Tabelle in einen normalen Bereich von Zellen um. Alle Daten werden beibehalten.|
|[Löschen](../api/table_delete.md)|Keine|Löscht die Tabelle.|
|[Reapplyfilters](../api/table_reapplyfilters.md)|Keine|Wendet alle Filter erneut an, die derzeit in der Tabelle vorhanden sind.|
|[Liste](../api/table_list.md) | [WorkbookTable](table.md) -Sammlung |Dient zum Abrufen einer Tabellenobjektsammlung. |
|[Hinzufügen](../api/tablecollection_add.md)|[WorkbookTable](table.md)|Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|ID|Zeichenfolge|Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn die Tabelle umbenannt wird. Diese Eigenschaft sollte als nicht transparenter Zeichenfolgenwert interpretiert werden und sollte nicht in einen anderen Typ ausgewertet werden. Schreibgeschützt.|
|Name|Zeichenfolge|Der Name der Tabelle.|
|showHeaders|boolesch|Gibt an, ob die Kopfzeile sichtbar oder nicht sichtbar ist. Dieser Wert kann festgelegt werden, um die Kopfzeile anzuzeigen, oder sie zu entfernen.|
|showTotals|boolesch|Gibt an, ob die Ergebniszeile sichtbar ist oder nicht. Dieser Wert kann so festgelegt werden, dass die Ergebniszeile angezeigt oder ausgeblendet wird.|
|Stil|Zeichenfolge|Konstanter Wert, der das Tabellenformat darstellt. Die möglichen Werte sind: TableStyleLight1 bis TableStyleLight21 TableStyleMedium1 bis TableStyleMedium28 TableStyleStyleDark1 bis TableStyleStyleDark11. Eine benutzerdefinierte Formatvorlage, die in der Arbeitsmappe vorhanden ist, kann auch angegeben werden.|
|highlightFirstColumn|boolesch|Gibt an, ob die erste Spalte spezielle Formatierung enthält.   |
|highlightLastColumn|boolesch|Gibt an, ob die letzte Spalte spezielle Formatierung enthält. |
|showBandedColumns|boolesch|Gibt an, ob die Spalten gebänderte Formatierung aufweisen, wobei ungerade Spalten anders hervorgehoben werden als gerade, um die Tabelle leichter lesbar zu machen.   |
|showBandedRows|boolesch|Gibt an, ob die Zeilen gebänderte Formatierung aufweisen, wobei ungerade Zeilen anders hervorgehoben werden als gerade, um die Tabelle leichter lesbar zu machen.    |
|showFilterButton|boolesch|Gibt an, ob die Filterschaltflächen am oberen Rand jedes Spaltenheaders sichtbar sind. Diese Einstellung ist nur zulässig, wenn die Tabelle eine Kopfzeile enthält.   |
|legacyId|Zeichenfolge|In älteren Excel-Clients verwendete Legacy-ID. Der Wert des Bezeichners bleibt unverändert, auch wenn die Tabelle umbenannt wird. Diese Eigenschaft sollte als nicht transparenter Zeichenfolgenwert interpretiert werden und sollte nicht in einen anderen Typ ausgewertet werden. Schreibgeschützt.   |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Spalten|[WorkbookTableColumn](tablecolumn.md) -Sammlung|Stellt eine Auflistung aller Spalten in der Tabelle dar. Schreibgeschützt.|
|Rows|[WorkbookTableRow](tablerow.md) -Sammlung|Stellt eine Auflistung aller Zeilen in der Tabelle dar. Schreibgeschützt.|
|sortieren|[WorkbookTableSort](tablesort.md)|Stellt die Sortierung für die Tabelle dar. Schreibgeschützt.|
|Arbeitsblatt|[WorkbookWorksheet](worksheet.md)|Das Arbeitsblatt, das die aktuelle Tabelle enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTable"
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
  "style": "String",
  "legacyId": "String"
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
