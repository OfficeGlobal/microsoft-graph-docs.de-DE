---
title: Ressourcentyp stringKeyAttributeMappingSourceValuePair
description: Stellt ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist AttributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: ff914c23a238356a821d2902bf18900cf9957548
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516217"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>Ressourcentyp stringKeyAttributeMappingSourceValuePair

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist [AttributeMappingSource](synchronization-attributemappingsource.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Key|String|Der Name des Parameters.|
|Wert|[attributeMappingSource](synchronization-attributemappingsource.md)|Der Wert des Parameters.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyattributemappingsourcevaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
