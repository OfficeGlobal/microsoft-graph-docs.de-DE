---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 524f25b6b5097197daeb8b130b10ff7513010965
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525003"
---
# <a name="textcolumn-resource-type"></a>TableColumn-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **textColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname                   | Typ   | Beschreibung
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | string | Gibt an, ob mehrere Textzeilen zugelassen sind.
| **appendChangesToExistingText** | string | Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.
| **linesForEditing**             | int    | Die Größe des Textfeldes.
| **maxLength**                   | int    | Die maximal Anzahl Zeichen für den Wert.
| **textType**                    | string | Der Texttyp des gespeicherten Textes. Muss `plain` oder `richText` sein.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/textColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
