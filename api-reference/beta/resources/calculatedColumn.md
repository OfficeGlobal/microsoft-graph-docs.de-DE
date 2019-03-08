---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 74f0e6430d47e0015fa849bb0d4ddf81690a9355
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481909"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/calculatedColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
