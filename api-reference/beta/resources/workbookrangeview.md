---
title: Ressourcentyp rangeView
description: RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ace424d12e38e4bb907923ea542ebd7330130d06
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643979"
---
# <a name="rangeview-resource-type"></a>Ressourcentyp rangeView

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|columnCount|Int32|Gibt die Anzahl der sichtbaren Spalten zurück. Schreibgeschützt.|
|formulas|Json|Stellt die Formel in der A1-Schreibweise dar. |
|formulasLocal|Json|Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar. Beispielsweise würde die englische Formel "= SUM(A1, 1.5)" in Deutsch "= SUMME(A1; 1,5) " werden.    |
|formulasR1C1|Json|Stellt die Formel in der R1C1-Schreibweise dar.   |
|Index|Int32|Der Index des Bereichs.|
|numberFormat|Json|Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar. Schreibgeschützt. |
|rowCount|Int32|Gibt die Anzahl der sichtbaren Zeilen zurück. Schreibgeschützt.  |
|text|Json|Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.    |
|valueTypes|Json|Stellt den Datentyp in jeder Zelle dar. Schreibgeschützt. Die folgenden Werte sind möglich: Unbekannt, leer, Zeichenfolge, Ganzzahl, Doppelwort, Boolesch, Fehler. |
|values|Json|Stellt die Rohwerte der angegebenen Bereichsansicht dar. Die zurückgegebenen Daten können vom Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zellen, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.   |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Rows|[workbookRangeView](workbookrangeview.md)-Sammlung| Stellt eine Sammlung der mit dem Bereich verknüpften Bereichsansichten dar. Schreibgeschützt.    Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
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
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookrangeview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
