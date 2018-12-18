---
title: Ressourcentyp managementConditionExpressionString
description: Eine Zeichenfolge Management Bedingung ist eine Zeichenfolgendarstellung eines Ausdrucks Bedingung Management.
author: tfitzmac
ms.openlocfilehash: eabcc730e86f74e2afc7c93874d47e787579c899
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361040"
---
# <a name="managementconditionexpressionstring-resource-type"></a>Ressourcentyp managementConditionExpressionString

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Zeichenfolge Management Bedingung ist eine Zeichenfolgendarstellung eines Ausdrucks Bedingung Management.

Erbt vom [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Wert|Zeichenfolge|Die Verwaltung Condition-Anweisung Ausdruck String-Wert.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





