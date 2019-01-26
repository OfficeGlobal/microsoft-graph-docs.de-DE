---
title: Ressourcentyp filterOperatorSchema
description: Beschreibt einen Operator, der in einem Filter verwendet werden kann.
localization_priority: Normal
ms.openlocfilehash: 366e00b5d21efeaf67e3e799c5b1c2412a68e268
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573682"
---
# <a name="filteroperatorschema-resource-type"></a>Ressourcentyp filterOperatorSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt einen Operator, der in einem [Filter](synchronization-filter.md)verwendet werden kann.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:--------------------------|:---------------|
|Stelligkeit                       | microsoft.graph.scopeOperatorType         |Stelligkeit des Operators. Mögliche Werte sind: `Binary` und `Unary`. Der Standardwert ist `Binary`.|
|multivaluedComparisonType   | microsoft.graph.scopeOperatorMultiValuedComparisonType          |Mögliche Werte sind: `All` und `Any`. Gilt nur für mehrwertige Attribute. `All`bedeutet, dass alle Werte, die die Bedingung erfüllen müssen. `Any`bedeutet, dass mindestens ein Wert hat, um die Bedingung zu erfüllen. Der Standardwert ist `All`.|
|supportedAttributeTypes     | AttributeType-Auflistung         |Attribut Typen, die vom Operator unterstützt. Mögliche Werte sind: `Boolean`, `Binary`, `Reference`, `Integer` und `String`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "microsoft.graph.scopeOperatorType",
  "multivaluedComparisonType": "microsoft.graph.scopeOperatorMultiValuedComparisonType",  
  "supportedAttributeTypes": ["attributeType"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
