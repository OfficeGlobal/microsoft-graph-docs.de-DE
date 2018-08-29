---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: 7e26b3683c2c84d1c413f3214da39e0a3d016f40
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267843"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn-Ressourcentyp

Die **calculatedColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass die Daten der Spalten basierend auf anderen Spalten der Webseite berechnet werden.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **calculatedColumn**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname  | Typ    | Beschreibung
|:---------------|:--------|:--------------------------------------------------
| **format**     | string  | Für `dateTime`-Ausgabetypen das Format des Werts. Muss `dateOnly` oder `dateTime` sein.
| **formula**    | string  | Die Formel, die verwendet wird, um den Wert für diese Spalte zu berechnen.
| **outputType** | string  | Der Ausgabetyp, der verwendet wird, um Werte in dieser Spalte zu formatieren. Muss `boolean`, `currency`, `dateTime`, `number` oder `text` sein.

In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.
Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->
