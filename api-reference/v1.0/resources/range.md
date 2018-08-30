# <a name="range-resource-type"></a>Range-Ressourcentyp

Ein Bereich stellt einen Satz von einer oder mehrerer zusammenhängender Zellen wie z. B. eine Zelle, eine Zeile oder eine Spalte, ein Block von Zellen usw. dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Bereich abrufen](../api/range_get.md) | [Bereich](range.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des Range-Objekts.|
|[Aktualisieren](../api/range_update.md) | [Bereich](range.md)   |Dient zum Aktualisieren des Range-Objekts. |
|[Boundingrect](../api/range_boundingrect.md)|[Bereich](range.md)|Ruft das kleinste Range-Objekt, das die angegebenen Bereichen umfasst. Beispielsweise ist der GetBoundingRect von "B2:C5" und "D10:E15": "B2:E16".|
|[Zelle](../api/range_cell.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.|
|[Spalte](../api/range_column.md)|[Bereich](range.md)|Ruft eine Spalte ab, die im Bereich enthalten ist.|
|[Columnsafter](../api/workbookrange_columnsafter.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.|
|[Columnsbefore](../api/workbookrange_columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Spalten links vom gegebenen Bereich ab.|
|[Entirecolumn](../api/range_entirecolumn.md)|[Bereich](range.md)|Ruft ein Objekt ab, das die gesamte Spalte des Bereichs darstellt.|
|[Entirerow](../api/range_entirerow.md)|[Bereich](range.md)|Ruft ein Objekt ab, das die gesamte Zeile des Bereichs darstellt.|
|[Intersection](../api/range_intersection.md)|[Bereich](range.md)|Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.|
|[Lastcell](../api/range_lastcell.md)|[Bereich](range.md)|Ruft die letzte Zelle im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs „B2:D5“ „D5“.|
|[Lastcolumn](../api/range_lastcolumn.md)|[Bereich](range.md)|Ruft die letzte Spalte im Bereich ab. Beispielsweise lautet die letzte Spalte von „B2:D5“ „D2:D5“.|
|[Lastrow](../api/range_lastrow.md)|[Bereich](range.md)|Ruft die letzte Zeile im Bereich ab. Beispielsweise lautet die letzte Zeile des Bereichs "B2:D5" "B5:D5".|
|[Offsetrange](../api/range_offsetrange.md)|[Bereich](range.md)|Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.|
|[Zeile](../api/range_row.md)|[Bereich](range.md)|Ruft eine Zeile ab, die im Bereich enthalten ist.|
|[Rowsabove](../api/workbookrange_rowsabove.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.|
|[Rowsbelow](../api/workbookrange_rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Zeilen unterhalb eines gegebenen Bereichs ab.|
|[Usedrange](../api/range_usedrange.md)|[Bereich](range.md)|Gibt den verwendeten Bereich des angegebenen Range-Objekts zurück.|
|[Löschen](../api/range_clear.md)|Keine|Löscht Bereichswerte, Format, Füllung, Rahmen usw.|
|[Löschen](../api/range_delete.md)|Keine|Löscht die dem Bereich zugeordneten Zellen.|
|[Einfügen](../api/range_insert.md)|[Bereich](range.md)|Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.|
|[Zusammenführen](../api/range_merge.md)|Keine|Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.|
|[Resizedrange](../api/workbookrange_resizedrange.md)|[workbookRangeView](workbookrangeview.md)|Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.|
|[Zusammenführung aufheben](../api/range_unmerge.md)|Keine|Hebt den Zellverbund des Bereichs in einzelne Zellen auf.|
|[Visibleview](../api/workbookrange_visibleview.md)|[workbookRangeView](workbookrangeview.md)|Ruft den in einem gefilterten Bereich sichtbaren Bereich ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|address|Zeichenfolge|Entspricht dem Bereichsverweis in A1-Schreibweise. Adresswert für den Blattbezug (z. B. Tabelle1!A1:B4). Schreibgeschützt.|
|addressLocal|Zeichenfolge|Stellt den Bereichsbezug für den angegebenen Bereich in der Sprache des Benutzers dar. Schreibgeschützt.|
|cellCount|int|Anzahl der Zellen im Bereich. Schreibgeschützt.|
|columnCount|int|Stellt die Gesamtanzahl der Spalten im Bereich dar. Schreibgeschützt.|
|columnHidden|boolesch|Stellt dar, ob alle Spalten des aktuellen Bereichs ausgeblendet sind.|
|columnIndex|int|Stellt die Spaltenanzahl der ersten Zelle im Bereich dar. Nullindiziert. Schreibgeschützt.|
|Formeln|Json|Stellt die Formel in der A1-Schreibweise dar.|
|formulasLocal|Json|Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar.  Beispielsweise würde die englische Formel „= SUM(A1, 1.5)“ in Deutsch „= SUMME(A1; 1,5)“ werden.|
|formulasR1C1|Json|Stellt die Formel in der R1C1-Schreibweise dar.|
|ausgeblendet|boolesch|Stellt dar, ob alle Zellen des aktuellen Bereichs ausgeblendet sind. Schreibgeschützt.|
|numberFormat|Json|Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar.|
|rowCount|int|Gibt die Anzahl der Zeilen im Bereich zurück. Schreibgeschützt.|
|rowHidden|boolesch|Stellt dar, ob alle Zeilen des aktuellen Bereichs ausgeblendet sind.|
|rowIndex|int|Gibt die Spaltenanzahl der ersten Zelle im Bereich zurück. Nullindiziert. Schreibgeschützt.|
|Text|Json|Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.|
|valueTypes|Json|Stellt den Typ der Daten, die jeder Zelle an. Mögliche Werte: `Unknown`, `Empty`, `String`, `Integer`, `Double`, `Boolean`, `Error`. Schreibgeschützt.|
|Werte|Json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Format|[WorkbookRangeFormat](rangeformat.md)|Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, den Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt. Schreibgeschützt.|
|sortieren|[WorkbookRangeSort](rangesort.md)|Das Arbeitsblatt, das den aktuellen Bereich enthält. Schreibgeschützt.|
|Arbeitsblatt|[WorkbookWorksheet](worksheet.md)|Das Arbeitsblatt, das den aktuellen Bereich enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRange"
}-->

```json
{
  "address": "string",
  "addressLocal": "string",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": "json",
  "formulasLocal": "json",
  "formulasR1C1": "json",
  "hidden": true,
  "numberFormat": "json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "json",
  "valueTypes": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
