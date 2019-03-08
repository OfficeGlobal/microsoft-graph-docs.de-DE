---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 66fbc59fa9fe4880c023086c9bd334e04650bc73
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481713"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn-Ressourcentyp

Die **calculatedColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Daten der Spalten basierend auf anderen Spalten der Webseite berechnet werden.

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
| **format**     | Zeichenfolge  | Für `dateTime`-Ausgabetypen das Format des Werts. Muss `dateOnly` oder `dateTime` sein.
| **formula**    | Zeichenfolge  | Die Formel, die verwendet wird, um den Wert für diese Spalte zu berechnen.
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
