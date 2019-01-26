---
title: Range-Ressourcentyp
description: Ein Bereich stellt einen Satz von einer oder mehrerer zusammenhängender Zellen wie z. B. eine Zelle, eine Zeile oder eine Spalte, ein Block von Zellen usw. dar.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 08bbecd51528012a23f02ebc83cb401e21126df1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575062"
---
# <a name="range-resource-type"></a>Range-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Bereich stellt einen Satz von einer oder mehrerer zusammenhängender Zellen wie z. B. eine Zelle, eine Zeile oder eine Spalte, ein Block von Zellen usw. dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Range abrufen](../api/range-get.md) | [range](range.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des range-Objekts.|
|[Aktualisieren](../api/range-update.md) | [range](range.md)   |Dient zum Aktualisiren des Range-Objekts. |
|[Boundingrect](../api/range-boundingrect.md)|[range](range.md)|Ruft das kleinste Bereichsobjekt ab, das die angegebenen Bereiche umfasst. Beispielsweise das GetBoundingRect von "B2:C5" und "D10:E15" lautet "B2:E16".|
|[Cell](../api/range-cell.md)|[range](range.md)|Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.|
|[Column](../api/range-column.md)|[range](range.md)|Ruft eine Spalte ab, die im Bereich enthalten ist.|
|[Columnsafter](../api/workbookrange-columnsafter.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.|
|[Columnsbefore](../api/workbookrange-columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Spalten links vom gegebenen Bereich ab.|
|[Entirecolumn](../api/range-entirecolumn.md)|[range](range.md)|Ruft ein Objekt ab, das die gesamte Spalte des Bereichs darstellt.|
|[Entirerow](../api/range-entirerow.md)|[range](range.md)|Ruft ein Objekt ab, das die gesamte Zeile des Bereichs darstellt.|
|[Intersection](../api/range-intersection.md)|[range](range.md)|Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.|
|[Lastcell](../api/range-lastcell.md)|[Range](range.md)|Ruft die letzte Zelle im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs „B2:D5“ „D5“.|
|[Lastcolumn](../api/range-lastcolumn.md)|[range](range.md)|Ruft die letzte Spalte im Bereich ab. Beispielsweise lautet die letzte Spalte von „B2:D5“ „D2:D5“.|
|[Lastrow](../api/range-lastrow.md)|[Range](range.md)|Ruft die letzte Zeile im Bereich ab. Beispielsweise lautet die letzte Zeile des Bereichs "B2:D5" "B5:D5".|
|[Offsetrange](../api/range-offsetrange.md)|[range](range.md)|Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.|
|[Row](../api/range-row.md)|[Range](range.md)|Ruft eine Zeile ab, die im Bereich enthalten ist.|
|[Rowsabove](../api/workbookrange-rowsabove.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.|
|[Rowsbelow](../api/workbookrange-rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|Ruft eine bestimmte Anzahl von Zeilen unterhalb eines gegebenen Bereichs ab.|
|[Usedrange](../api/range-usedrange.md)|[range](range.md)|Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.|
|[Clear](../api/range-clear.md)|Keine|Löscht Bereichswerte, Format, Füllung, Rahmen usw.|
|[Löschen](../api/range-delete.md)|Keine|Löscht die dem Bereich zugeordneten Zellen.|
|[Einfügen](../api/range-insert.md)|[range](range.md)|Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.|
|[Merge](../api/range-merge.md)|Keine|Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.|
|[Resizedrange](../api/workbookrange-resizedrange.md)|[workbookRangeView](workbookrangeview.md)|Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.|
|[Unmerge](../api/range-unmerge.md)|Keine|Hebt den Zellverbund des Bereichs in einzelne Zellen auf.|
|[Visibleview](../api/workbookrange-visibleview.md)|[workbookRangeView](workbookrangeview.md)|Ruft den in einem gefilterten Bereich sichtbaren Bereich ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|address|string|Entspricht dem Bereichsverweis in A1-Schreibweise. Adresswert für den Blattbezug (z. B. Tabelle1!A1:B4). Schreibgeschützt.|
|addressLocal|string|Stellt den Bereichsbezug für den angegebenen Bereich in der Sprache des Benutzers dar. Schreibgeschützt.|
|cellCount|int|Anzahl der Zellen im Bereich. Schreibgeschützt.|
|columnCount|int|Stellt die Gesamtanzahl der Spalten im Bereich dar. Schreibgeschützt.|
|columnHidden|Boolescher Wert|Stellt dar, ob alle Spalten des aktuellen Bereichs ausgeblendet sind.|
|columnIndex|int|Stellt die Spaltenanzahl der ersten Zelle im Bereich dar. Nullindiziert. Schreibgeschützt.|
|formulas|Json|Stellt die Formel in der A1-Schreibweise dar.|
|formulasLocal|Json|Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar.  Beispielsweise würde die englische Formel „= SUM(A1, 1.5)“ in Deutsch „= SUMME(A1; 1,5)“ werden.|
|formulasR1C1|Json|Stellt die Formel in der R1C1-Schreibweise dar.|
|hidden|Boolescher Wert|Stellt dar, ob alle Zellen des aktuellen Bereichs ausgeblendet sind. Schreibgeschützt.|
|numberFormat|Json|Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar.|
|rowCount|int|Gibt die Anzahl der Zeilen im Bereich zurück. Schreibgeschützt.|
|rowHidden|Boolescher Wert|Stellt dar, ob alle Zeilen des aktuellen Bereichs ausgeblendet sind.|
|rowIndex|int|Gibt die Spaltenanzahl der ersten Zelle im Bereich zurück. Nullindiziert. Schreibgeschützt.|
|text|Json|Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.|
|valueTypes|string|Stellt den Datentyp in jeder Zelle dar. Mögliche Werte: `Unknown`, `Empty`, `String`, `Integer`, `Double`, `Boolean`, `Error`. Schreibgeschützt.|
|values|Json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[rangeFormat](rangeformat.md)|Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, den Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt. Schreibgeschützt.|
|sort|[workbookRangeSort](rangesort.md)|Das Arbeitsblatt, das den aktuellen Bereich enthält. Schreibgeschützt.|
|Arbeitsblatt|[workbookWorksheet](worksheet.md)|Das Arbeitsblatt, das den aktuellen Bereich enthält. Schreibgeschützt.|

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
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "hidden": true,
  "numberFormat": "Json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "Json",
  "valueTypes": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
