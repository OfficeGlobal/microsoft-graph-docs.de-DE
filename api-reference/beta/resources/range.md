# <a name="range-resource-type"></a>Range-Ressourcentyp

Ein Bereich stellt einen Satz von einer oder mehrerer zusammenhängender Zellen wie z. B. eine Zelle, eine Zeile oder eine Spalte, ein Block von Zellen usw. dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Range abrufen](../api/range_get.md) | [Range](range.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des range-Objekts.|
|[Update](../api/range_update.md) | [Range](range.md)    |Dient zum Aktualisiren des Range-Objekts. |
|[Boundingrect](../api/range_boundingrect.md)|[Range](range.md)|Ruft das kleinste Bereichsobjekt ab, das die angegebenen Bereiche umfasst. Beispielsweise das GetBoundingRect von "B2:C5" und "D10:E15" lautet "B2:E16".|
|[Cell](../api/range_cell.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.|
|[Column](../api/range_column.md)|[Range](range.md)|Ruft eine Spalte ab, die im Bereich enthalten ist.|
|[Columnsafter](../api/workbookrange_columnsafter.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.|
|[Columnsbefore](../api/workbookrange_columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Spalten links vom gegebenen Bereich ab.|
|[Entirecolumn](../api/range_entirecolumn.md)|[Range](range.md)|Ruft ein Objekt ab, das die gesamte Spalte des Bereichs darstellt.|
|[Entirerow](../api/range_entirerow.md)|[Range](range.md)|Ruft ein Objekt ab, das die gesamte Zeile des Bereichs darstellt.|
|[Intersection](../api/range_intersection.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.|
|[Lastcell](../api/range_lastcell.md)|[Range](range.md)|Ruft die letzte Zelle im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs „B2: D5“ „D5“.|
|[Lastcolumn](../api/range_lastcolumn.md)|[Range](range.md)|Ruft die letzte Spalte im Bereich ab. Beispielsweise lautet die letzte Spalte von „B2:D5“ „D2:D5“.|
|[Lastrow](../api/range_lastrow.md)|[Range](range.md)|Ruft die letzte Zeile im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs "B2: D5" "B5:D5".|
|[Offsetrange](../api/range_offsetrange.md)|[Range](range.md)|Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.|
|[Row](../api/range_row.md)|[Range](range.md)|Ruft eine Zelle ab, die im Bereich enthalten ist.|
|[Rowsabove](../api/workbookrange_rowsabove.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.|
|[Rowsbelow](../api/workbookrange_rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Zeilen unterhalb eines gegebenen Bereichs ab.|
|[Usedrange](../api/range_usedrange.md)|[Range](range.md)|Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.|
|[Clear](../api/range_clear.md)|None|Löscht Bereichswerte, Format, Füllung, Rahmen usw.|
|[Löschen](../api/range_delete.md)|None|Löscht die dem Bereich zugeordneten Zellen.|
|[Insert](../api/range_insert.md)|[Range](range.md)|Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.|
|[Merge](../api/range_merge.md)|None|Führt die Zellen des Bereichs in eine Region im Arbeitsblatt zusammen.|
|[Resizedrange](../api/workbookrange_resizedrange.md)|[workbookRangeView](workbookrangeview.md)|Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.|
|[Unmerge](../api/range_unmerge.md)|None|Hebt den Zellverbund des Bereichs in einzelne Zellen auf.|
|[Visibleview](../api/workbookrange_visibleview.md)|[workbookRangeView](workbookrangeview.md)|Ruft den in einem gefilterten Bereich sichtbaren Bereich ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|address|string|Entspricht dem Bereichsverweis in A1-Schreibweise. Adresswert für den Blattbezug (z. B. Tabelle1!A1:B4). Schreibgeschützt.|
|addressLocal|string|Stellt den Bereichsbezug für den angegebenen Bereich in der Sprache des Benutzers dar. Schreibgeschützt.|
|cellCount|int|Anzahl der Zellen im Bereich. Schreibgeschützt.|
|columnCount|int|Stellt die Gesamtanzahl der Spalten im Bereich dar. Schreibgeschützt.|
|columnHidden|boolean|Stellt dar, ob alle Spalten des aktuellen Bereichs ausgeblendet sind.|
|columnIndex|int|Stellt die Spaltenanzahl der ersten Zelle im Bereich dar. Nullindiziert. Schreibgeschützt.|
|formulas|json|Stellt die Formel in der A1-Schreibweise dar.|
|formulasLocal|json|Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar.  Beispielsweise würde die englische Formel „= SUM(A1, 1.5)“ in Deutsch „= SUMME(A1; 1,5)“ werden.|
|formulasR1C1|json|Stellt die Formel in der R1C1-Schreibweise dar.|
|hidden|boolean|Stellt dar, ob alle Zellen des aktuellen Bereichs ausgeblendet sind. Schreibgeschützt.|
|numberFormat|json|Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar.|
|rowCount|int|Gibt die Anzahl der Zeilen im Bereich zurück. Schreibgeschützt.|
|rowHidden|boolean|Stellt dar, ob alle Zeilen des aktuellen Bereichs ausgeblendet sind.|
|rowIndex|int|Gibt die Spaltenanzahl der ersten Zelle im Bereich zurück. Nullindiziert. Schreibgeschützt.|
|text|json|Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.|
|valueTypes|string|Stellt den Datentyp in jeder Zelle dar. Mögliche Werte: `Unknown`, `Empty`, `String`, `Integer`, `Double`, `Boolean`, `Error`. Schreibgeschützt.|
|values|json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Format|[RangeFormat](rangeformat.md)|Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, den Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt. Schreibgeschützt.|
|sort|[RangeSort](rangesort.md)|Das Arbeitsblatt, das den aktuellen Bereich enthält. Schreibgeschützt.|
|Arbeitsblatt|[Worksheet](worksheet.md)|Das Arbeitsblatt, das den aktuellen Bereich enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.range"
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
