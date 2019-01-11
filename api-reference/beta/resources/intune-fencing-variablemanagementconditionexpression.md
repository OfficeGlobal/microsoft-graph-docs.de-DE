---
title: Ressourcentyp variableManagementConditionExpression
description: Ergibt die Bedingung Verwaltungsstatus als boolescher Ausdruck.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d0805f7c698f90cbcb10bfffdce9c95ce6705b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890153"
---
# <a name="variablemanagementconditionexpression-resource-type"></a>Ressourcentyp variableManagementConditionExpression

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ergibt die Bedingung Verwaltungsstatus als boolescher Ausdruck.

Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionId|String|Die Bedingung Management-Id, die verwendet wird, für den Ausdruck ausgewertet werden soll.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```





