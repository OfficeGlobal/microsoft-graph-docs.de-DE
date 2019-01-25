---
title: Ressourcentyp attributeMappingParameterSchema
description: Beschreibt einen einzelnen Parameter in einer AttributeMappingFunctionSchema verwendet.
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529950"
---
# <a name="attributemappingparameterschema-resource-type"></a>Ressourcentyp attributeMappingParameterSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt einen einzelnen Parameter in einer [AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)verwendet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Boolescher Wert                   |Der angegebene Parameter kann mehrere Male bereitgestellt werden (beispielsweise Eingabe mehrere Zeichenfolgen der `Concatenate(string,string,...)` Funktion). |
|name                        |Zeichenfolge                    |Parametername |
|erforderlich                    |Boolescher Wert                   |`true`Wenn der Parameter erforderlich ist. andernfalls `false`. |
|type                        |Zeichenfolge                    |Mögliche Werte: `Boolean`, `Binary`, `Reference`, `Integer`, `String`. Der Standardwert lautet `String`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingparameterschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
