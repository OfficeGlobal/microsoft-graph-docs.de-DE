---
title: WindowsWifiEnterpriseEAPConfiguration erstellen
description: Erstellen eines neuen windowsWifiEnterpriseEAPConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8df4ef22727b6bb56ccf759408f60ba22f0dc6dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146725"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a>WindowsWifiEnterpriseEAPConfiguration erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

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
Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsWifiEnterpriseEAPConfiguration-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsWifiEnterpriseEAPConfiguration erforderlich sind.

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
|PresharedKey wurde|Zeichenfolge|Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Geben Sie den WiFi-Sicherheitstyp an. Von [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)geerbt. Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Geben Sie den Grenzwert für die gemessene Verbindung für die WLAN-Verbindung an. Von [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)geerbt. Mögliche Werte sind: `unrestricted`, `fixed` und `variable`.|
|SSID|Zeichenfolge|Geben Sie die SSID der WiFi-Verbindung an. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkName|Zeichenfolge|Geben Sie den Namen der Netzwerkkonfiguration an. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectAutomatically|Boolescher Wert|Geben Sie an, ob die WiFi-Verbindung automatisch eine Verbindung herstellen soll, wenn in Reichweite. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectToPreferredNetwork|Boolescher Wert|Geben Sie an, ob die WLAN-Verbindung mit den bevorzugten Netzwerken verbunden werden soll, wenn Sie bereits mit diesem verknüpft ist.  Erfordert, dass ConnectAutomatically auf true festgelegt ist. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolescher Wert|Geben Sie an, ob die WLAN-Verbindung automatisch eine Verbindung herstellen soll, selbst wenn die SSID nicht übertragen wird. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Geben Sie die Proxyeinstellung für die von [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)geerbte WLAN-Konfiguration an. Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|Zeichenfolge|Geben Sie die IP-Adresse für den Proxy Server an. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyManualPort|Int32|Geben Sie den Anschluß für den Proxy Server an. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|Zeichenfolge|Geben Sie die URL für das Proxy Server-Konfigurationsskript an. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|forceFIPSCompliance|Boolescher Wert|Geben Sie an, ob die FIPS-Konformität erzwungen werden soll. Geerbt von [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkSingleSignOn|[networkSingleSignOnType](../resources/intune-deviceconfig-networksinglesignontype.md)|Geben Sie den Typ des SSO-Netzwerks an. Mögliche Werte sind: `disabled`, `prelogon` und `postlogon`.|
|maximumAuthenticationTimeoutInSeconds|Int32|Angeben des maximalen Authentifizierungstimeouts (in Sekunden).  Gültiger Range: 1-120|
|promptForAdditionalAuthenticationCredentials|Boolescher Wert|Geben Sie an, ob die WLAN-Verbindung weitere Authentifizierungsanmeldeinformationen anfordern soll.|
|enablePairwiseMasterKeyCaching|Boolescher Wert|Geben Sie an, ob die WLAN-Verbindung eine paarweise Zwischenspeicherung aktivieren soll.|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|Geben Sie die maximale Anzahl von paarweise-Hauptschlüssel Cache Zeit (in Minuten) an.  Gültiger Range: 5-1440|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|Geben Sie die maximale Anzahl von paarweise-Hauptschlüsseln im Cache an.  Gültiger Range: 1-255|
|enablePreAuthentication|Boolescher Wert|Geben Sie an, ob die Vorauthentifizierung aktiviert werden soll.|
|maximumPreAuthenticationAttempts|Int32|Geben Sie maximale vorauthentifizierungs Versuche an.  Gültiger Range: 1-16|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|EAP (Extensible Authentication Protocol). Gibt den Typ des EAP-Protokolls an, das auf dem WLAN-Endpunkt (Router) festgelegt ist. Mögliche Werte sind: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap` und `eapFast`.|
|trustedServerCertificateNames|String collection|Geben Sie vertrauenswürdige Serverzertifikat Namen an.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Geben Sie die Authentifizierungsmethode an. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Angeben des inneren Authentifizierungsprotokolls für EAP-TTLS. Mögliche Werte: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|Outeridentityprivacytemporaryvalue wurden|Zeichenfolge|Geben Sie die Zeichenfolge an, die Benutzernamen für Datenschutz bei Verwendung von EAP-TTLS oder PEAP ersetzen soll.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




