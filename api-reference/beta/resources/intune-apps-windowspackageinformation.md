---
title: Dem windowspackageinformation-Ressourcentyp
description: Enthält Eigenschaften für die Paketinformationen für eine Windows-Branchen-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba69fe277809b3ce4d6f81a198fc305204984d73
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166451"
---
# <a name="windowspackageinformation-resource-type"></a>Dem windowspackageinformation-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für die Paketinformationen für eine Windows-Branchen-app.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Die Windows-Architektur, für die diese APP ausgeführt werden kann. Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.|
|displayName|String|Der Anzeige Name.|
|identityName|Zeichenfolge|Identitätsname|
|identityPublisher|Zeichenfolge|Der Identitäts Herausgeber.|
|identityResourceIdentifier|Zeichenfolge|Der Identitätsressourcenbezeichner.|
|identityVersion|Zeichenfolge|Die Identitäts Version.|
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




