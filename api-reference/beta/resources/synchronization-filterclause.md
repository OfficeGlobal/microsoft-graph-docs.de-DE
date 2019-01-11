---
title: FilterClause Ressourcentyp
description: Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).
localization_priority: Normal
ms.openlocfilehash: 89807a6086f661388c8d5b1d5f82bfe973c3af39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833859"
---
# <a name="filterclause-resource-type"></a>FilterClause Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|operatorName|Zeichenfolge|Name des Operators auf den Quell- und Ziel-Operanden angewendet werden soll. Einer der unterstützten Operatoren muss sein. Unterstützte Operatoren können ermittelt werden.|
|sourceOperandName|Zeichenfolge|Name der Datenquelle Operand (Operand getesteten). Der Name der Operand muss einem den Attributnamen im Quellobjekt übereinstimmen.|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|Werte, denen mit der Quelloperanden getestet wird.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
