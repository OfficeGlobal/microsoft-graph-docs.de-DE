---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: b0efefbbd6a47a547bc724274fd9bc26b2628442
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510757"
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **ChoiceColumn** einer [ColumnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer Auswahlliste ausgewählt werden können.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **choiceColumn**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname      | Typ               | Beschreibung
|:-------------------|:-------------------|:----------------------------------------------
| **allowTextEntry** | boolean            | Ist der Wert true, sind benutzerdefinierte Werte, die sich nicht in der konfigurierten Auswahl befinden, zugelassen.
| **choices**        | Collection(string) | Die Liste der Werte, die für diese Spalte zur Verfügung stehen.
| **displayAs**      | string             | Wie werden die Auswahlmöglichkeiten in der UX dargestellt? Muss `checkBoxes`, `dropDownMenu` oder `radioButtons` sein.


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/choicecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
