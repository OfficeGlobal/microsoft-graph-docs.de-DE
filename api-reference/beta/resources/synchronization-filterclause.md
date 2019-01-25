---
title: FilterClause Ressourcentyp
description: Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523869"
---
# <a name="filterclause-resource-type"></a>FilterClause Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|operatorName|String|Name des Operators auf den Quell- und Ziel-Operanden angewendet werden soll. Einer der unterstützten Operatoren muss sein. Unterstützte Operatoren können ermittelt werden.|
|sourceOperandName|String|Name der Datenquelle Operand (Operand getesteten). Der Name der Operand muss einem den Attributnamen im Quellobjekt übereinstimmen.|
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
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
