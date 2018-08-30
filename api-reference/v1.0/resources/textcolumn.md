---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: b5c41091b9193aabc36ee04e9dcc310bfc110af1
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264287"
---
# <a name="textcolumn-resource-type"></a>TableColumn-Ressourcentyp

Die **textColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.

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

| Eigenschaftenname                   | Typ    | Beschreibung
|:--------------------------------|:--------|:---------------------------------
| **allowMultipleLines**          | Boolescher Wert | Gibt an, ob mehrere Textzeilen zugelassen sind.
| **appendChangesToExistingText** | Boolescher Wert | Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.
| **linesForEditing**             | Int32   | Die Größe des Textfeldes.
| **maxLength**                   | Int32   | Die maximal Anzahl Zeichen für den Wert.
| **textType**                    | Zeichenfolge  | Der Texttyp des gespeicherten Textes. Muss `plain` oder `richText` sein. `richText`

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->
