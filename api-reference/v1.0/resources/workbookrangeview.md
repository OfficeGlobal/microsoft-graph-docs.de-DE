---
title: Ressourcentyp rangeView
description: RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.
ms.openlocfilehash: e7a19464e52f694705f2e22795513110ae7cbd89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016116"
---
# <a name="rangeview-resource-type"></a>Ressourcentyp rangeView
RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Zeilen auflisten](../api/workbookrangeview-list-rows.md) |[workbookRangeView](workbookrangeview.md)-Sammlung| Rufen Sie eine workbookRangeView-Objektsammlung ab.|
|[Itemat](../api/workbookrangeview-itemat.md)|[workbookRangeView](workbookrangeview.md)|Rufen Sie ein im Index basiertes RangeView-Element ab.|
|[Range](../api/workbookrangeview-range.md)|[workbookRange](range.md)|Rufen Sie das Range-Objekt ab, das mit der Bereichsansicht verknüpft ist.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|cellAddresses|Json|Stellt die Zelle Adressen
|columnCount|Int32|Gibt die Anzahl der sichtbaren Spalten zurück. Schreibgeschützt.|
|formulas|Json|Stellt die Formel in der A1-Schreibweise dar. |
|formulasLocal|Json|Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar. Beispielsweise würde die englische Formel "= SUM(A1, 1.5)" in Deutsch "= SUMME(A1; 1,5) " werden.    |
|formulasR1C1|Json|Stellt die Formel in der R1C1-Schreibweise dar.   |
|Index|Int32|Der Index des Bereichs.|
|numberFormat|Json|Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar. Schreibgeschützt. |
|rowCount|Int32|Gibt die Anzahl der sichtbaren Zeilen zurück. Schreibgeschützt.  |
|text|Json|Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.    |
|valueTypes|Json|Stellt den Typ der Daten, die jeder Zelle an. Schreibgeschützt. Die möglichen Werte sind: unbekannt, leer, String, Integer, Double, Boolean, Fehler. |
|values|Json|Stellt die Rohwerte der angegebenen Bereichsansicht dar. Die zurückgegebenen Daten können vom Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zellen, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.   |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Rows|[workbookRangeView](workbookrangeview.md)-Sammlung| Stellt eine Sammlung der mit dem Bereich verknüpften Bereichsansichten dar. Schreibgeschützt.    Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
