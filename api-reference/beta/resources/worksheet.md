---
title: Worksheet-Ressourcentyp
description: Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6a3a5fbb222c9228b55b2dac2a38b699ed15f213
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574376"
---
# <a name="worksheet-resource-type"></a>Worksheet-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Arbeitsblatt abrufen](../api/worksheet-get.md) | [WorkbookWorksheet](worksheet.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des worksheet-Objekts.|
|[Diagramm erstellen](../api/worksheet-post-charts.md) |[WorkbookChart](chart.md)| Dient zum Erstellen eines neuen Diagramms durch Veröffentlichen in der Diagrammsammlung.|
|[Namen auflisten](../api/worksheet-list-names.md) |[WorkbookNamedItem](workbooknameditem.md) -Auflistung| Dient zum Abrufen der benannten Elementsammlung, die mit dem Arbeitsblatt verknüpft ist.|
|[Diagramme auflisten](../api/worksheet-list-charts.md) |[WorkbookChart](chart.md) -Auflistung| Dient zum Abrufen einer Diagrammobjeksammlung.|
|[Tabelle erstellen](../api/worksheet-post-tables.md) |[WorkbookTable](table.md)| Dient zum Erstellen einer neuen Tabelle durch Veröffentlichen in der Diagrammsammlung.|
|[Tabellen auflisten](../api/worksheet-list-tables.md) |[WorkbookTable](table.md) -Auflistung| Dient zum Abrufen einer Tabellenobjeksammlung.|
|[Aktualisieren](../api/worksheet-update.md) | [WorkbookWorksheet](worksheet.md)   |Dient zum Aktualisieren des Worksheet-Objekts. |
|[Cell](../api/worksheet-cell.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.|
|[Range](../api/worksheet-range.md)|[Range](range.md)|Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.|
|[Usedrange](../api/worksheet-usedrange.md)|[Range](range.md)|Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.|
|[Löschen](../api/worksheet-delete.md)|Keine|Löscht das Arbeitsblatt aus der Arbeitsmappe.|
|[List](../api/worksheet-list.md) | [WorkbookWorksheet](worksheet.md) -Auflistung |Dient zum Abrufen der Arbeitsblatt-Objektsammlung. |
|[Add](../api/worksheetcollection-add.md)|[WorkbookWorksheet](worksheet.md)|Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblätter hinzugefügt. |
|[pivotTables auflisten](../api/workbookworksheet-list-pivottables.md) |[workbookPivotTable](workbookpivottable.md)-Sammlung| Rufen Sie eine workbookPivotTable-Objektsammlung ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn das Arbeitsblatt umbenannt oder verschoben wird. Schreibgeschützt.|
|name|string|Der Anzeigename des Arbeitsblatts.|
|position|int|Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.|
|visibility|string|Die Sichtbarkeit des Arbeitsblatts ein. Die möglichen Werte sind: `Visible`, `Hidden`, `VeryHidden`.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|charts|[WorkbookChart](chart.md) -Auflistung|Gibt die Sammlung von Diagrammen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.|
|names|[WorkbookNamedItem](workbooknameditem.md) -Auflistung|Gibt die Sammlung von Namen zurück, die mit dem Arbeitsblatt verknüpft sind. Schreibgeschützt.|
|pivotTables|[workbookPivotTable](workbookpivottable.md)-Sammlung| Die Sammlung von PivotTables, die Teil des Arbeitsblatts sind. |
|Schutz|[WorkbookWorksheetProtection](worksheetprotection.md)|Gibt das Arbeitsblattschutz-Objekt für ein Arbeitsblatt zurück. Schreibgeschützt.|
|Tabellen|[WorkbookTable](table.md) -Auflistung|Gibt die Sammlung von Tabellen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
