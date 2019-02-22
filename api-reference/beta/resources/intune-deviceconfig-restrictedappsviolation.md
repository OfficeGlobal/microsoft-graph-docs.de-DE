---
title: restrictedAppsViolation-Ressourcentyp
description: Verletzung des Konfigurationsprofils für eingeschränkte apps pro Gerät und Benutzer
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8764d3d84ba0706f3769ef019def43cb080660d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139914"
---
# <a name="restrictedappsviolation-resource-type"></a>restrictedAppsViolation-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verletzung des Konfigurationsprofils für eingeschränkte apps pro Gerät und Benutzer

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[RestrictedAppsViolations aufListen](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekte.|
|[RestrictedAppsViolation abrufen](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Lesen von Eigenschaften und Beziehungen des [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.|
|[RestrictedAppsViolation erstellen](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Erstellen eines neuen [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.|
|[RestrictedAppsViolation löschen](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Keine|Löscht eine [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[RestrictedAppsViolation aktualisieren](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Aktualisieren der Eigenschaften eines [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für das Objekt. Zusammengesetzt aus "Account-ID", "Device", "Policies" und "userId"|
|userId|String|Benutzer eindeutiger Bezeichner, muss GUID sein|
|userName|Zeichenfolge|Benutzername|
|managedDeviceId|Zeichenfolge|Eindeutiger Bezeichner für verwaltetes Gerät, muss GUID sein|
|deviceName|Zeichenfolge|Gerätename|
|deviceConfigurationId|Zeichenfolge|Device Configuration Profile Unique Identifier, must be GUID|
|deviceConfigurationName|Zeichenfolge|Name des Geräte Konfigurationsprofils|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Plattformtyp. Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Eingeschränkter apps-Status. Mögliche Werte sind: `prohibitedApps` und `notApprovedApps`.|
|restrictedApps|[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) -Sammlung|Liste der verletzten eingeschränkten apps|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```




