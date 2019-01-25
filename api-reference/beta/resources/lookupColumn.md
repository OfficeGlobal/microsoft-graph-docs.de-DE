---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 2efb199fafbf7c60af0e13720ea1b9efd93dc05c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517519"
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **lookupColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer anderen Quelle der Website nachgeschlagen werden.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **lookupColumn**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname             | Typ    | Beschreibung
|:--------------------------|:--------|:---------------------------------------
| **allowMultipleValues**   | boolean | Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.
| **allowUnlimitedLength**  | boolean | Gibt an, ob die Werte in der Spalte die standardmäßige Grenze von 255 Zeichen überschreiten dürfen.
| **columnName**            | string  | Der Name der Nachschlagequellen-Spalte.
| **listId**                | string  | Der eindeutige Bezeichner der Nachschlagequellen-Liste.
| **primaryLookupColumnId** | string  | Wenn angegeben, erfolgt in dieser Spalte ein *zweites Nachschlagen*. In der Liste wird ein weiteres Feld zu dem beim *ersten Nachschlagen* ermittelten Element hinzugefügt. Verwenden Sie das Listenelement des *ersten * Nachschlagens als Quelle für die hier genannte Spalte.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/lookupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
