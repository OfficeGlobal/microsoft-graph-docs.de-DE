# <a name="worksheet-resource-type"></a>Worksheet-Ressourcentyp

Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Arbeitsblatt abrufen](../api/worksheet_get.md) | [WorkbookWorksheet](worksheet.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des worksheet-Objekts.|
|[Diagramm erstellen](../api/worksheet_post_charts.md) |[WorkbookChart](chart.md)| Dient zum Erstellen eines neuen Diagramms durch Veröffentlichen in der Diagrammsammlung.|
|[Namen auflisten](../api/worksheet_list_names.md) |[WorkbookNamedItem](nameditem.md)-Sammlung| Dient zum Abrufen der benannten Elementsammlung, die mit dem Arbeitsblatt verknüpft ist.|
|[Diagramme auflisten](../api/worksheet_list_charts.md) |[WorkbookChart](chart.md)-Sammlung| Dient zum Abrufen einer Diagrammobjeksammlung.|
|[Tabelle erstellen](../api/worksheet_post_tables.md) |[WorkbookTable](table.md)| Dient zum Erstellen einer neuen Tabelle durch Veröffentlichen in der Diagrammsammlung.|
|[Tabellen auflisten](../api/worksheet_list_tables.md) |[WorkbookTable](table.md)-Sammlung| Dient zum Abrufen einer Tabellenobjeksammlung.|
|[Aktualisieren](../api/worksheet_update.md) | [WorkbookWorksheet](worksheet.md)   |Dient zum Aktualisieren des Worksheet-Objekts. |
|[Zelle](../api/worksheet_cell.md)|[Spanne](range.md)|Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.|
|[Spanne](../api/worksheet_range.md)|[Spanne](range.md)|Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.|
|[Usedrange](../api/worksheet_usedrange.md)|[Spanne](range.md)|Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.|
|[Löschen](../api/worksheet_delete.md)|Keine|Löscht das Arbeitsblatt aus der Arbeitsmappe.|
|[Liste](../api/worksheet_list.md) | [WorkbookWorksheet](worksheet.md)-Sammlung |Dient zum Abrufen der Arbeitsblatt-Objektsammlung. |
|[Hinzufügen](../api/worksheetcollection_add.md)|[WorkbookWorksheet](worksheet.md)|Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblätter hinzugefügt. |
|[pivotTables auflisten](../api/workbookworksheet_list_pivottables.md) |[workbookPivotTable](workbookpivottable.md)-Sammlung| Rufen Sie eine workbookPivotTable-Objektsammlung ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge|Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn das Arbeitsblatt umbenannt oder verschoben wird. Schreibgeschützt.|
|name|Zeichenfolge|Der Anzeigename des Arbeitsblatts.|
|position|int|Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.|
|visibility|Zeichenfolge|Die Sichtbarkeit des Arbeitsblatts. Die möglichen Werte sind: `Visible`, `Hidden`, `VeryHidden`.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|charts|[WorkbookChart](chart.md)-Sammlung|Gibt die Sammlung von Diagrammen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.|
|names|[WorkbookNamedItem](nameditem.md)-Sammlung|Gibt die Sammlung von Namen zurück, die mit dem Arbeitsblatt verknüpft sind. Schreibgeschützt.|
|pivotTables|[workbookPivotTable](workbookpivottable.md)-Sammlung| Die Sammlung von PivotTables, die Teil des Arbeitsblatts sind. |
|protection|[WorkbookWorksheetProtection](worksheetprotection.md)|Gibt das Arbeitsblattschutz-Objekt für ein Arbeitsblatt zurück. Schreibgeschützt.|
|Tabellen|[WorkbookTable](table.md)-Sammlung|Gibt die Sammlung von Tabellen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
