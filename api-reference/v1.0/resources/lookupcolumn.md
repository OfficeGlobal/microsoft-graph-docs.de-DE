---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 41e643019d842a365c333efa3c3a6861c51a7fc7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892100"
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn-Ressourcentyp

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
