---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
ms.openlocfilehash: b6d4ea3acf4995548fce7f2c86b3c95c444b59b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020041"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>deviceEnrollmentPlatformRestriction-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Plattformspezifische Registrierungseinschränkungen
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|platformBlocked|Boolescher Wert|Sperren der Plattform für die Registrierung|
|personalDeviceEnrollmentBlocked|Boolescher Wert|Sperren privat genutzter Geräte für die Registrierung|
|osMinimumVersion|Zeichenfolge|Unterstützte mindestens benötigte iOS-Version|
|osMaximumVersion|Zeichenfolge|Unterstützte maximal verwendbare iOS-Version|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



