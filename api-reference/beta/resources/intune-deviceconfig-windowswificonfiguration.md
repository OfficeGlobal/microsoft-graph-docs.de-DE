---
title: windowsWifiConfiguration-Ressourcentyp
description: Gerätekonfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4ec447d0e77803f939b9aafb413f05d3e90987e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153788"
---
# <a name="windowswificonfiguration-resource-type"></a>windowsWifiConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Gerätekonfiguration.


Erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsWifiConfigurations aufListen](../api/intune-deviceconfig-windowswificonfiguration-list.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekte.|
|[WindowsWifiConfiguration abrufen](../api/intune-deviceconfig-windowswificonfiguration-get.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts.|
|[WindowsWifiConfiguration erstellen](../api/intune-deviceconfig-windowswificonfiguration-create.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|Erstellen eines neuen [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts.|
|[WindowsWifiConfiguration löschen](../api/intune-deviceconfig-windowswificonfiguration-delete.md)|Keine|Löscht eine [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).|
|[WindowsWifiConfiguration aktualisieren](../api/intune-deviceconfig-windowswificonfiguration-update.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|Aktualisieren der Eigenschaften eines [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|PresharedKey wurde|Zeichenfolge|Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk.|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Geben Sie den WiFi-Sicherheitstyp an. Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Geben Sie den Grenzwert für die gemessene Verbindung für die WLAN-Verbindung an. Mögliche Werte sind: `unrestricted`, `fixed` und `variable`.|
|SSID|Zeichenfolge|Geben Sie die SSID der WiFi-Verbindung an.|
|networkName|Zeichenfolge|Geben Sie den Namen der Netzwerkkonfiguration an.|
|connectAutomatically|Boolescher Wert|Geben Sie an, ob die WiFi-Verbindung automatisch eine Verbindung herstellen soll, wenn in Reichweite.|
|connectToPreferredNetwork|Boolescher Wert|Geben Sie an, ob die WLAN-Verbindung mit den bevorzugten Netzwerken verbunden werden soll, wenn Sie bereits mit diesem verknüpft ist.  Erfordert, dass ConnectAutomatically auf true festgelegt ist.|
|connectWhenNetworkNameIsHidden|Boolescher Wert|Geben Sie an, ob die WLAN-Verbindung automatisch eine Verbindung herstellen soll, selbst wenn die SSID nicht übertragen wird.|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Geben Sie die Proxyeinstellung für die WLAN-Konfiguration an. Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|Zeichenfolge|Geben Sie die IP-Adresse für den Proxy Server an.|
|proxyManualPort|Int32|Geben Sie den Anschluß für den Proxy Server an.|
|proxyAutomaticConfigurationUrl|Zeichenfolge|Geben Sie die URL für das Proxy Server-Konfigurationsskript an.|
|forceFIPSCompliance|Boolescher Wert|Geben Sie an, ob die FIPS-Konformität erzwungen werden soll.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true
}
```




