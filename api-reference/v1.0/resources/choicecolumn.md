---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: c266550e8918603c3ee6104818c0aa721f1281d9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn-Ressourcentyp

Die **ChoiceColumn** einer [ColumnDefinition](columnDefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer Auswahlliste ausgewählt werden können.

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
  "tocPath": "Resources/ChoiceColumn"
} -->
