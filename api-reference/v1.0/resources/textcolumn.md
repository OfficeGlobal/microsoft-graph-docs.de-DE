---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: d064253cfad141d5879afb52451ca28fa2aeca67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860879"
---
# <a name="textcolumn-resource-type"></a>TableColumn-Ressourcentyp

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

| Eigenschaftenname                   | Typ    | Beschreibung
|:--------------------------------|:--------|:---------------------------------
| **allowMultipleLines**          | Boolean | Gibt an, ob mehrere Textzeilen zugelassen sind.
| **appendChangesToExistingText** | Boolean | Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.
| **linesForEditing**             | int32   | Die Größe des Textfeldes.
| **maxLength**                   | int32   | Die maximal Anzahl Zeichen für den Wert.
| **textType**                    | string  | Der Texttyp des gespeicherten Textes. Muss `plain` oder `richText` sein.

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
