---
title: Ressourcentyp deviceManagementUserRightsSetting
description: Stellt eine Benutzerrechte festlegen.
ms.openlocfilehash: e657c15a76700ef87283220254937ec685c57784
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063359"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a>Ressourcentyp deviceManagementUserRightsSetting

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt eine Benutzerrechte festlegen.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|state|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Einstellung für Benutzerrechterichtlinien, die den aktuellen Status dieses Benutzers darstellt. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|localUsersOrGroups|[DeviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) -Auflistung|Eine Auflistung von lokalen Benutzern oder Gruppen, die auf Gerät festgelegt werden, wenn der Status dieser Einstellung zulässig ist, der darstellt. Diese Sammlung darf maximal 500 Elemente enthalten.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```





