---
title: Ressourcentyp mobileAppIntentAndStateDetail
description: Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.
ms.openlocfilehash: d793f23346991c681ecfd4e0d55272153496ae36
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057960"
---
# <a name="mobileappintentandstatedetail-resource-type"></a>Ressourcentyp mobileAppIntentAndStateDetail

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|applicationId|Zeichenfolge|MobieApp-Bezeichner.|
|displayName|String|Der vom Administrator bereitgestellte oder importierte Titel der App.|
|mobileAppIntent|[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)|Mobile App beabsichtigt. Mögliche Werte sind: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment` und `exclude`.|
|displayVersion|String|Menschen lesbare Version der Anwendung|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|Der Installationsstatus der app. Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.|
|supportedDeviceTypes|[MobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) -Auflistung|Die unterstützten Plattformen für die app.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```




