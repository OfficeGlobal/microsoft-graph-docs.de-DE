---
title: Table-Ressourcentyp
description: Stellt eine Excel-Tabelle dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2e3e9c93f7459d666fbe7f28a67241c2831b7079
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642646"
---
# <a name="table-resource-type"></a>Table-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Excel-Tabelle dar.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Tabelle abrufen](../api/table-get.md) | [Table](table.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des table-Objekts.|
|[TableColumn erstellen](../api/table-post-columns.md) |[TableColumn](tablecolumn.md)| Dient zum Erstellen einer neuen TableColumn durch Veröffentlichen in der Diagrammsammlung.|
|[Spalten auflisten](../api/table-list-columns.md) |[TableColumn](tablecolumn.md)-Sammlung| Dient zum Abrufen einer TableColumn-Objektsammlung.|
|[TableRow erstellen](../api/table-post-rows.md) |[TableRow](tablerow.md)| Dient zum Erstellen einer neuen TableRow durch Veröffentlichen in der Zeilensammlung.|
|[Zeilen auflisten](../api/table-list-rows.md) |[TableRow](tablerow.md)-Sammlung| Dient zum Abrufen einer TableRow-Objektsammlung.|
|[Update](../api/table-update.md) | [Table](table.md)   |Dient zum Aktualisieren des Table-Objekts. |
|[Databodyrange](../api/table-databodyrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit dem Datenteil der Tabelle verknüpft ist.|
|[Headerrowrange](../api/table-headerrowrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der Kopfzeile der Tabelle verknüpft ist.|
|[Range](../api/table-range.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Tabelle verknüpft ist.|
|[Totalrowrange](../api/table-totalrowrange.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der Ergebniszeile der Tabelle verknüpft ist.|
|[Clearfilters](../api/table-clearfilters.md)|Keine|Löscht alle Filter, die derzeit in der Tabelle verwendet werden.|
|[Converttorange](../api/table-converttorange.md)|[Range](range.md)|Wandelt die Tabelle in einen normalen Bereich von Zellen um. Alle Daten werden beibehalten.|
|[Delete](../api/table-delete.md)|Keine|Löscht die Tabelle.|
|[Reapplyfilters](../api/table-reapplyfilters.md)|Keine|Wendet alle Filter erneut an, die derzeit in der Tabelle vorhanden sind.|
|[List](../api/table-list.md) | [Tabellensammlung](table.md) |Dient zum Abrufen einer Tabellenobjektsammlung. |
|[Add](../api/tablecollection-add.md)|[Table](table.md)|Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn die Tabelle umbenannt wird. Diese Eigenschaft sollte als nicht transparenter Zeichenfolgenwert interpretiert werden und sollte nicht in einen anderen Typ ausgewertet werden. Schreibgeschützt.|
|name|string|Der Name der Tabelle.|
|showHeaders|Boolescher Wert|Gibt an, ob die Kopfzeile sichtbar oder nicht sichtbar ist. Dieser Wert kann festgelegt werden, um die Kopfzeile anzuzeigen, oder sie zu entfernen.|
|showTotals|Boolescher Wert|Gibt an, ob die Ergebniszeile sichtbar ist oder nicht. Dieser Wert kann so festgelegt werden, dass die Ergebniszeile angezeigt oder ausgeblendet wird.|
|style|string|Konstanter Wert, der das Tabellenformat darstellt. Die folgenden Werte sind möglich: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. Es kann ebenfalls eine in der Arbeitsmappe vorhandene benutzerdefinierte Formatierung angegeben werden.|
|highlightFirstColumn|Boolean|Gibt an, ob die erste Spalte spezielle Formatierung enthält.   |
|highlightLastColumn|Boolean|Gibt an, ob die letzte Spalte spezielle Formatierung enthält. |
|showBandedColumns|Boolean|Gibt an, ob die Spalten gebänderte Formatierung aufweisen, wobei ungerade Spalten anders hervorgehoben werden als gerade, um die Tabelle leichter lesbar zu machen.   |
|showBandedRows|Boolean|Gibt an, ob die Zeilen gebänderte Formatierung aufweisen, wobei ungerade Zeilen anders hervorgehoben werden als gerade, um die Tabelle leichter lesbar zu machen.    |
|showFilterButton|Boolean|Gibt an, ob die Filterschaltflächen am oberen Rand jedes Spaltenheaders sichtbar sind. Diese Einstellung ist nur zulässig, wenn die Tabelle eine Kopfzeile enthält.   |
|legacyId|String|In älteren Excel-Clients verwendete Legacy-ID. Der Wert des Bezeichners bleibt unverändert, auch wenn die Tabelle umbenannt wird. Diese Eigenschaft sollte als nicht transparenter Zeichenfolgenwert interpretiert werden und sollte nicht in einen anderen Typ ausgewertet werden. Schreibgeschützt.   |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|columns|[TableColumn](tablecolumn.md)-Sammlung|Stellt eine Auflistung aller Spalten in der Tabelle dar. Schreibgeschützt.|
|Rows|[TableRow](tablerow.md)-Sammlung|Stellt eine Auflistung aller Zeilen in der Tabelle dar. Schreibgeschützt.|
|sort|[TableSort](tablesort.md)|Stellt die Sortierung für die Tabelle dar. Schreibgeschützt.|
|Arbeitsblatt|[Worksheet](worksheet.md)|Das Arbeitsblatt, das die aktuelle Tabelle enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
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
  "style": "String",
  "legacyId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/table.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
