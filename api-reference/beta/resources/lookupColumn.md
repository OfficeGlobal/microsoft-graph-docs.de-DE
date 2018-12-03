---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 92eb43dad2ceca173fba79ad7d40f51f488a992c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058207"
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
