---
title: Ressourcentyp unaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 06a379a53d6d85956a54bede444714e082196ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949423"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>Ressourcentyp unaryManagementConditionExpression

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.

Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|operator|[unaryManagementConditionExpressionOperatorType](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|Die Auswertung des Vorgangs unärer Operator verwendete Operator. Mögliche Werte sind: `not`.|
|Operand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|Der Operand des Vorgangs unärer Operator.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





