---
title: Ressourcentyp appleVpnConfiguration
description: Apple VPN-Konfigurationsprofil.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 85a70322a601fd09c9b944fcfd1d07885fa8f1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853256"
---
# <a name="applevpnconfiguration-resource-type"></a>Ressourcentyp appleVpnConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Apple VPN-Konfigurationsprofil.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste appleVpnConfigurations](../api/intune-deviceconfig-applevpnconfiguration-list.md)|[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) -Objekte.|
|[Abrufen von appleVpnConfiguration](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|connectionName|String|Name der Verbindung für den Benutzer angezeigt.|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|Verbindungstyp. Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.|
|loginGroupOrDomain|String|Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.|
|role|String|Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.|
|Bereich|String|Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.|
|Server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|VPN-Server im Netzwerk. Stellen Sie sicher, dass Endbenutzer dieser Speicherort im Netzwerk zugreifen können.|
|Bezeichner|String|Bezeichner von VPN-Anbieter bereitgestellt, wenn Verbindungstyp auf benutzerdefinierte VPN festgelegt ist. Beispiel: Cisco AnyConnect verwendet eine Kennung des dem Formular com.cisco.anyconnect.applevpn.plugin|
|customData|[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung|Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist. Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren. Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare. Diese Sammlung kann maximal 25 Elemente enthalten.|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist. Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren. Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare. Diese Sammlung kann maximal 25 Elemente enthalten.|
|enableSplitTunneling|Boolean|Senden Sie alle Netzwerkdatenverkehr über VPN.|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Authentifizierungsmethode für diese VPN-Verbindung. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|enablePerApp|Boolean|Dies auf True festlegen, erstellt pro App VPN-Nutzlast, später Apps zugeordnet sein kann, die diese VPN-Verbindung auf iOS-Gerät des Endbenutzers auslösen kann.|
|safariDomains|Collection von Objekten des Typs „String“|Safari Domänen, wenn diese VPN pro App-Einstellung aktiviert ist. Zusätzlich zu den apps dieses VPN zugeordnet angegeben Safari Domänen Hier wird auch können Sie diese VPN-Verbindung zu lösen.|
|onDemandRules|[VpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Auflistung|Bei Bedarf Regeln. Diese Collection darf maximal 500 Elemente enthalten.|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|Proxy-Server.|
|optInToDeviceIdSharing|Boolean|Opt-In, das das Gerät Id Drittanbieter-VPN-Clients für die Verwendung während der Network Access Control Validierung Freigabe.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
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





