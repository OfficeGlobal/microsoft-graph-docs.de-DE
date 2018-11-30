---
title: Ressourcentyp unaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.
ms.openlocfilehash: 958c180e52a268f849eca1fe0d2a2b75ff81333b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062191"
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





