---
title: Ressourcentyp filterOperatorSchema
description: Beschreibt einen Operator, der in einem Filter verwendet werden kann.
localization_priority: Normal
ms.openlocfilehash: 0d26fb58b77369b70ab185fa8ad5214d6b6c1e71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848279"
---
# <a name="filteroperatorschema-resource-type"></a>Ressourcentyp filterOperatorSchema

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Beschreibt einen Operator, der in einem [Filter](synchronization-filter.md)verwendet werden kann.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:--------------------------|:---------------|
|Stelligkeit                       |String          |Stelligkeit des Operators. Mögliche Werte sind: `Binary` und `Unary`. Der Standardwert ist `Binary`.|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |Mögliche Werte sind: `All` und `Any`. Gilt nur für mehrwertige Attribute. `All`bedeutet, dass alle Werte, die die Bedingung erfüllen müssen. `Any`bedeutet, dass mindestens ein Wert hat, um die Bedingung zu erfüllen. Der Standardwert ist `All`.|
|name                        |String                     |Name des Operators. |
|supportedAttributeTypes     |Collection von Objekten des Typs „String“         |Attribut Typen, die vom Operator unterstützt. Mögliche Werte sind: `Boolean`, `Binary`, `Reference`, `Integer` und `String`.|

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
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
