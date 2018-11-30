---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 6841f453cdfd423ead3edeea5895242a28b998f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016635"
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn-Ressourcentyp

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


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
