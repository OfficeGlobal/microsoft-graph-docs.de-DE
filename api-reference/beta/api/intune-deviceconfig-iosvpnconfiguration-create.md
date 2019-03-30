---
title: IosVpnConfiguration erstellen
description: Erstellen eines neuen iosVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e220b2a41ce61ae71343b2754993c6b5082f352e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985872"
---
# <a name="create-iosvpnconfiguration"></a>IosVpnConfiguration erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das iosVpnConfiguration-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVpnConfiguration erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|connectionName|String|Dem Benutzer angezeigter Verbindungsname. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|Verbindungstyp. Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt. Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn`,,, `customVpn`, `ciscoIPSec` `citrix`,, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess` `f5Access2018` `citrixSso`,,, `paloAltoGlobalProtectV2`.|
|loginGroupOrDomain|String|Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|String|Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Reich|String|Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|VPN-Server im Netzwerk. Stellen Sie sicher, dass Endbenutzer auf diesen Netzwerkspeicherort zugreifen können. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Bezeichner|String|Vom VPN-Anbieter bereitgestellter Bezeichner, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist. Beispiel: Cisco AnyConnect verwendet einen Bezeichner des Formulars "com. Cisco. AnyConnect. applevpn. Plugin", geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung|Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist. Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist. Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden. Diese Auflistung kann maximal 25 Elemente enthalten. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist. Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist. Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden. Diese Auflistung kann maximal 25 Elemente enthalten. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|enableSplitTunneling|Boolescher Wert|Senden Sie den gesamten Netzwerkdatenverkehr über VPN. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Authentifizierungsmethode für diese VPN-Verbindung. Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|enablePerApp|Boolescher Wert|Wenn Sie dies auf true festlegen, wird eine pro-App-VPN-Nutzlast erstellt, die später apps zugeordnet werden kann, die diese VPN-Anschluss auf dem iOS-Gerät des Endbenutzers auslösen können. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|safariDomains|String collection|Safari-Domänen, wenn diese VPN-pro-app-Einstellung aktiviert ist. Zusätzlich zu den apps, die mit diesem VPN verknüpft sind, können auch hier angegebene Safari-Domänen diese VPN-Verbindung auslösen. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Sammlung|Regeln für on-Demand. Diese Sammlung darf maximal 500 Elemente enthalten. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Sie|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|Proxy Server. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|optInToDeviceIdSharing|Boolescher Wert|Opt-in für die Freigabe der Geräte-ID an Drittanbieter-VPN-Clients für die Verwendung während der Überprüfung der Netzwerkzugriffssteuerung. Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|providerType|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|Anbietertyp für pro-App-VPN. Mögliche Werte sind: `notConfigured`, `appProxy` und `packetTunnel`.|
|User Domain|String|Nur Zscaler. Geben Sie in der Zscaler-App eine statische Domäne ein, in der das Anmeldefeld vorab aufgefüllt werden soll. Wenn dieser Wert leer bleibt, wird stattdessen die Azure Active Directory-Domäne des Benutzers verwendet.|
|strictEnforcement|Boolescher Wert|Nur Zscaler. Blockiert den Netzwerkdatenverkehr, bis sich der Benutzer bei der Zscaler-App anmeldet. "True" bedeutet, dass der Datenverkehr blockiert ist.|
|cloudName|String|Nur Zscaler. Zscaler-Wolke, der der Benutzer zugewiesen ist.|
|excludeList|String collection|Nur Zscaler. Liste der Netzwerkadressen, die nicht über die Zscaler-Cloud gesendet werden.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```




