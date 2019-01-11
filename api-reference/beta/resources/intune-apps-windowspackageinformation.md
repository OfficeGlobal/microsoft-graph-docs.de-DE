---
title: Ressourcentyp windowsPackageInformation
description: Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f7f3cd593670e071ae62bdb287bcebeee01d555
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849532"
---
# <a name="windowspackageinformation-resource-type"></a>Ressourcentyp windowsPackageInformation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Die Windows-Architektur für die diese app ausgeführt werden kann. Mögliche Werte sind: `none`, `x86`, `x64`, `arm` und `neutral`.|
|displayName|String|Der Anzeigename.|
|identityName|String|Identitätsname|
|identityPublisher|String|Der Identity-Herausgeber.|
|identityResourceIdentifier|String|Der Identitätsressourcenbezeichner.|
|identityVersion|String|Die Identität-Version.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Der Wert für die Mindestversion des verwendbaren Betriebssystems.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  }
}
```





