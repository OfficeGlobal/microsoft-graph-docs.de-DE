---
title: Ressourcentyp stringKeyObjectValuePair
description: Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist ein beliebiges JSON-Objekt, darstellt. Dies ist ein open OData-Typ, die eine Eigenschaft mit dem Namen haben erwartet `value` also ein gültiges JSON-Objekt.
localization_priority: Normal
ms.openlocfilehash: 819a2e004ee712f1250652ce0b3811940545e643
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572171"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>Ressourcentyp stringKeyObjectValuePair

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist ein beliebiges JSON-Objekt, darstellt. Dies ist ein open OData-Typ, die eine Eigenschaft mit dem Namen haben erwartet `value` also ein gültiges JSON-Objekt.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Key|String|Key.|
|Wert|Json|Beliebige JSON-Objekt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value":"Json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
