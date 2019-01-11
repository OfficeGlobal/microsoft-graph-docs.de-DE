---
title: Ressourcentyp governanceRuleSetting
description: Stellt die Regeln, denen die rolleneinstellungen bestehen.
localization_priority: Normal
ms.openlocfilehash: 7554c96daec70a95cde5ab0c3faedfba74764cff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894257"
---
# <a name="governancerulesetting-resource-type"></a>Ressourcentyp governanceRuleSetting

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Regeln, denen die rolleneinstellungen bestehen.


## <a name="properties"></a>Eigenschaften
|Eigenschaft      | Typ         |Beschreibung|
|:-------------|:-------------|:----------|
|ruleIdentifier|Zeichenfolge        |Die Id der Regel. Beispielsweise ``ExpirationRule`` und ``MfaRule``.|
|setting       |Zeichenfolge        |Die Einstellungen der Regel. Der Wert ist eine JSON-Zeichenfolge mit einer Liste von Paaren im Format Parameter_Name:Parameter_Value. Beispielsweise gibt `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
