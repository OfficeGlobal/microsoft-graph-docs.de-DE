---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 1e10997bd70f97fa91177aee48a6ffcecff40ab5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480838"
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
| **allowMultipleLines**          | Boolesch | Gibt an, ob mehrere Textzeilen zugelassen sind.
| **appendChangesToExistingText** | Boolesch | Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.
| **linesForEditing**             | Int32   | Die Größe des Textfeldes.
| **maxLength**                   | Int32   | Die maximal Anzahl Zeichen für den Wert.
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
