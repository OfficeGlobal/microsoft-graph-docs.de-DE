---
title: WorksheetProtectionOptions-Ressourcentyp
description: Stellt die Optionen für den Arbeitsblattschutz dar.
author: lumine2008
ms.openlocfilehash: 772c8b5eca7e9754a6bbc00e43cac102680974a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348573"
---
# <a name="worksheetprotectionoptions-resource-type"></a>WorksheetProtectionOptions-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Optionen für den Arbeitsblattschutz dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowAutoFilter|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen der Verwendung der automatischen Filterfunktion dar.|
|allowDeleteColumns|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Löschens von Spalten dar.|
|allowDeleteRows|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Löschens von Zeilen dar.|
|allowFormatCells|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Formatierens von Zellen dar.|
|allowFormatColumns|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Formatierens von Spalten dar.|
|allowFormatRows|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Formatierens von Zeilen dar.|
|allowInsertColumns|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Einfügens von Spalten dar.|
|allowInsertHyperlinks|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Einfügens von Hyperlinks dar.|
|allowInsertRows|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Einfügens von Zeilen dar.|
|allowPivotTables|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen der Verwendung der Pivottabellenfunktion dar.|
|allowSort|boolean|Stellt die Arbeitsblatt-Schutzoption zum Zulassen der Verwendung der Sortierfunktion dar.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->