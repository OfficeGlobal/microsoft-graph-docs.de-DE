---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: ad94cadaa26d0fab72236d4037ceffd09a52c561
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514278"
---
# <a name="defaultcolumnvalue-resource-type"></a>DefaultColumnValue-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der **DefaultColumnValue** einer [ColumnDefinition](columndefinition.md)-Ressource gibt den Standardwert für diese Spalte an.
Der Standardwert kann entweder direkt oder als Formel angegeben werden.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **defaultColumnValue**-Ressource.
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung
|:--------------|:-------|:----------------------------------------------------
| **formula**   | string | Die Formel, die verwendet wird, um den Standardwert für diese Spalte zu berechnen.
| **value**     | string | Der direkte Wert, der als Standardwert für diese Spalte verwendet wird.

Es kann jeweils nur **formula** oder **value** angegeben werden.

In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.
Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": [
    "Error: /api-reference/beta/resources/defaultColumnValue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
