---
title: WorksheetProtectionOptions-Ressourcentyp
description: Stellt die Optionen für den Arbeitsblattschutz dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e32e41eb46cc5af98f6d9aeffcf470e22fbad349
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514789"
---
# <a name="worksheetprotectionoptions-resource-type"></a>WorksheetProtectionOptions-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Optionen für den Arbeitsblattschutz dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowAutoFilter|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen der Verwendung der automatischen Filterfunktion dar.|
|allowDeleteColumns|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Löschens von Spalten dar.|
|allowDeleteRows|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Löschens von Zeilen dar.|
|allowFormatCells|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Formatierens von Zellen dar.|
|allowFormatColumns|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Formatierens von Spalten dar.|
|allowFormatRows|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Formatierens von Zeilen dar.|
|allowInsertColumns|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Einfügens von Spalten dar.|
|allowInsertHyperlinks|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Einfügens von Hyperlinks dar.|
|allowInsertRows|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen des Einfügens von Zeilen dar.|
|allowPivotTables|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen der Verwendung der Pivottabellenfunktion dar.|
|allowSort|Boolescher Wert|Stellt die Arbeitsblatt-Schutzoption zum Zulassen der Verwendung der Sortierfunktion dar.|

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
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotectionoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
