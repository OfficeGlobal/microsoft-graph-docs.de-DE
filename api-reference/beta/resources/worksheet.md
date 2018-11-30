---
title: Worksheet-Ressourcentyp
description: Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.
ms.openlocfilehash: 513a1fceb8e0b7e2c7667d5fac2e4a5978ed7c04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059137"
---
# <a name="worksheet-resource-type"></a>Worksheet-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Arbeitsblatt abrufen](../api/worksheet-get.md) | [Worksheet](worksheet.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des worksheet-Objekts.|
|[Diagramm erstellen](../api/worksheet-post-charts.md) |[Chart](chart.md)| Dient zum Erstellen eines neuen Diagramms durch Veröffentlichen in der Diagrammsammlung.|
|[Namen auflisten](../api/worksheet-list-names.md) |[NamedItem](nameditem.md) collection| Dient zum Abrufen der benannten Elementsammlung, die mit dem Arbeitsblatt verknüpft ist.|
|[Diagramme auflisten](../api/worksheet-list-charts.md) |[Diagrammsammlung](chart.md)| Dient zum Abrufen einer Diagrammobjeksammlung.|
|[Tabelle erstellen](../api/worksheet-post-tables.md) |[Table](table.md)| Dient zum Erstellen einer neuen Tabelle durch Veröffentlichen in der Diagrammsammlung.|
|[Tabellen auflisten](../api/worksheet-list-tables.md) |[Tabellensammlung](table.md)| Dient zum Abrufen einer Tabellenobjeksammlung.|
|[Update](../api/worksheet-update.md) | [Worksheet](worksheet.md)   |Dient zum Aktualisieren des Worksheet-Objekts. |
|[Cell](../api/worksheet-cell.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.|
|[Range](../api/worksheet-range.md)|[Range](range.md)|Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.|
|[Usedrange](../api/worksheet-usedrange.md)|[Range](range.md)|Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.|
|[Delete](../api/worksheet-delete.md)|Keine|Löscht das Arbeitsblatt aus der Arbeitsmappe.|
|[List](../api/worksheet-list.md) | [Worksheet](worksheet.md) collection |Dient zum Abrufen der Arbeitsblatt-Objektsammlung. |
|[Add](../api/worksheetcollection-add.md)|[Worksheet](worksheet.md)|Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblätter hinzugefügt. |
|[pivotTables auflisten](../api/workbookworksheet-list-pivottables.md) |[workbookPivotTable](workbookpivottable.md)-Sammlung| Rufen Sie eine workbookPivotTable-Objektsammlung ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn das Arbeitsblatt umbenannt oder verschoben wird. Schreibgeschützt.|
|name|string|Der Anzeigename des Arbeitsblatts.|
|position|int|Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.|
|visibility|string|Die Sichtbarkeit des Arbeitsblatts. Mögliche Werte: `Visible`, `Hidden`, `VeryHidden`.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|charts|[Diagrammsammlung](chart.md)|Gibt die Sammlung von Diagrammen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.|
|names|[NamedItem](nameditem.md) collection|Gibt die Sammlung von Namen zurück, die mit dem Arbeitsblatt verknüpft sind. Schreibgeschützt.|
|pivotTables|[workbookPivotTable](workbookpivottable.md)-Sammlung| Die Sammlung von PivotTables, die Teil des Arbeitsblatts sind. |
|Schutz|[WorksheetProtection](worksheetprotection.md)|Gibt das Arbeitsblattschutz-Objekt für ein Arbeitsblatt zurück. Schreibgeschützt.|
|Tabellen|[Table](table.md) collection|Gibt die Sammlung von Tabellen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
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
