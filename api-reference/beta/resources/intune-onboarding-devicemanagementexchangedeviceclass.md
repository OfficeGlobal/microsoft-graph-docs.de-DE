---
title: Ressourcentyp deviceManagementExchangeDeviceClass
description: Geräteklasse in Exchange.
author: tfitzmac
ms.openlocfilehash: 01e0877388391deaebbda18e48247f4e3585a63a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316779"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>Ressourcentyp deviceManagementExchangeDeviceClass

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Geräteklasse in Exchange.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|String|Name der Geräteklasse die von dieser Regel betroffen sind.|
|type|[deviceManagementExchangeAccessRuleType](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|Typ des Geräts, die durch diese Regel beeinflusst wird, z. B. Modell, Familie. Mögliche Werte: `family`, `model`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```





