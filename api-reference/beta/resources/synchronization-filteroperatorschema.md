---
title: Ressourcentyp filterOperatorSchema
description: Beschreibt einen Operator, der in einem Filter verwendet werden kann.
ms.openlocfilehash: 1a4e21aea2b65073a00c9797065f6788a66e2334
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059369"
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