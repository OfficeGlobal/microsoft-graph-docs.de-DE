---
title: Der applevpnconfiguration-Ressourcentyp
description: Apple VPN-Konfigurationsprofil.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9f526e256a5ec8ecd4e364b4e017508a999ea17
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163301"
---
# <a name="applevpnconfiguration-resource-type"></a>Der applevpnconfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Apple VPN-Konfigurationsprofil.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AppleVpnConfigurations aufListen](../api/intune-deviceconfig-applevpnconfiguration-list.md)|[der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) -Objekte.|
|[Der applevpnconfiguration abrufen](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[Der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) -Objekts.|

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
|connectionName|Zeichenfolge|Dem Benutzer angezeigter Verbindungsname.|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|Verbindungstyp. Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn`,,, `customVpn`, `ciscoIPSec` `citrix`,, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess` `f5Access2018` `citrixSso`,,, `paloAltoGlobalProtectV2`.|
|loginGroupOrDomain|Zeichenfolge|Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist.|
|role|Zeichenfolge|Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.|
|Bereich|Zeichenfolge|Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.|
|Server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|VPN-Server im Netzwerk. Stellen Sie sicher, dass Endbenutzer auf diesen Netzwerkspeicherort zugreifen können.|
|Bezeichner|Zeichenfolge|Vom VPN-Anbieter bereitgestellter Bezeichner, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist. Beispiel: Cisco AnyConnect verwendet einen Bezeichner des Formulars "com. Cisco. AnyConnect. applevpn. Plugin".|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung|Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist. Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist. Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden. Diese Auflistung kann maximal 25 Elemente enthalten.|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist. Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist. Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden. Diese Auflistung kann maximal 25 Elemente enthalten.|
|enableSplitTunneling|Boolescher Wert|Senden Sie den gesamten Netzwerkdatenverkehr über VPN.|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Authentifizierungsmethode für diese VPN-Verbindung. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|enablePerApp|Boolescher Wert|Wenn Sie dies auf true festlegen, wird eine pro-App-VPN-Nutzlast erstellt, die später apps zugeordnet werden kann, die diese VPN-Anschluss auf dem iOS-Gerät des Endbenutzers auslösen können.|
|safariDomains|String collection|Safari-Domänen, wenn diese VPN-pro-app-Einstellung aktiviert ist. Zusätzlich zu den apps, die mit diesem VPN verknüpft sind, können auch hier angegebene Safari-Domänen diese VPN-Verbindung auslösen.|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Sammlung|Regeln für on-Demand. Diese Collection darf maximal 500 Elemente enthalten.|
|Sie|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|Proxy Server.|
|optInToDeviceIdSharing|Boolescher Wert|Opt-in für die Freigabe der Geräte-ID an Drittanbieter-VPN-Clients für die Verwendung während der Überprüfung der Netzwerkzugriffssteuerung.|

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
  "@odata.type": "microsoft.graph.appleVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnConfiguration",
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
  "connectionName": "String",
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```




