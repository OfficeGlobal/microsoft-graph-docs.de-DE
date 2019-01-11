---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 5433b5b5a76d313f8f34e460400906479e6d3d7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876055"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
  "tocPath": "Resources/CalculatedColumn"
} -->
