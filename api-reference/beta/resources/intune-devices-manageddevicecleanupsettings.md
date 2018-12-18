---
title: Ressourcentyp managedDeviceCleanupSettings
description: Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.
author: tfitzmac
ms.openlocfilehash: 84650c4d2d182fe0da30ced56786a2c0216a6358
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304088"
---
# <a name="manageddevicecleanupsettings-resource-type"></a>Ressourcentyp managedDeviceCleanupSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceInactivityBeforeRetirementInDays|String|Anzahl der Tage, wenn das Gerät nicht Intune kontaktiert hat.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```





