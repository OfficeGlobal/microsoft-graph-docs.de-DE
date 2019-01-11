---
title: Ressourcentyp binaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 509e03e7d492289fc9615f7f8ad47bf13d5bead4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857050"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>Ressourcentyp binaryManagementConditionExpression

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.

Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|operator|[binaryManagementConditionExpressionOperatorType](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|Die Auswertung der binären Operation verwendete Operator. Mögliche Werte sind: `or` und `and`.|
|firstOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|Dem ersten Operanden der binären Operation.|
|secondOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|Der zweite Operand des binären Vorgangs.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





