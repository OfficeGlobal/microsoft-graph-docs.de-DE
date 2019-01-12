---
title: Ressourcentyp windowsPackageInformation
description: Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac0f9aad1cdba1eaaac12754fd4a4d0ad4a6db32
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926848"
---
# <a name="windowspackageinformation-resource-type"></a>Ressourcentyp windowsPackageInformation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Die Windows-Architektur für die diese app ausgeführt werden kann. Mögliche Werte sind: `none`, `x86`, `x64`, `arm` und `neutral`.|
|displayName|Zeichenfolge|Der Anzeigename.|
|identityName|Zeichenfolge|Identitätsname|
|identityPublisher|Zeichenfolge|Der Identity-Herausgeber.|
|identityResourceIdentifier|Zeichenfolge|Der Identitätsressourcenbezeichner.|
|identityVersion|Zeichenfolge|Die Identität-Version.|
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





