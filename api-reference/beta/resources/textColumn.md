---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 5ff280b6c969d9832e2f81f77dc32237f9905aad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061636"
---
# <a name="textcolumn-resource-type"></a>TableColumn-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
