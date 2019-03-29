---
title: MacOSEnterpriseWiFiConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines macOSEnterpriseWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0e9da43c989e45946aab06f4499cba4c346160c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982056"
---
# <a name="update-macosenterprisewificonfiguration"></a>MacOSEnterpriseWiFiConfiguration aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekts.

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)erforderlich sind.

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
|networkName|String|Netzwerk Name geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|SSID|String|Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectAutomatically|Boolescher Wert|Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet. Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolescher Wert|Verbinden, wenn das Netzwerk seinen Namen (SSID) nicht sendet. Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet. Von [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)geerbt. Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|Proxy Settings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Proxytyp für diese WLAN-Verbindung, die von [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)geerbt wurde. Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|String|Die IP-Adresse oder der DNS-Hostname des Proxyservers, wenn die manuelle Konfiguration ausgewählt ist. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyManualPort|Int32|Der Proxy Server, wenn die manuelle Konfiguration ausgewählt ist. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|URL des automatischen Konfigurationsskripts des Proxyservers, wenn die automatische Konfiguration ausgewählt ist. Diese URL ist in der Regel der Speicherort der PAC (Proxy Auto Configuration)-Datei. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|PresharedKey wurde|String|Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|EAP (Extensible Authentication Protocol). Gibt den Typ des EAP-Protokolls an, das auf dem WLAN-Endpunkt (Router) festgelegt ist. Mögliche Werte sind: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap` und `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|EAP-FAST-Konfigurations Option, wenn EAP-FAST der ausgewählte EAP-Typ ist. Mögliche Werte sind: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision` und `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|String collection|Namen von vertrauenswürdigen Servern, wenn der EAP-Typ für EAP-TLS/TTLS/FAST oder PEAP konfiguriert ist. Dies ist der allgemeine Name, der in den von Ihrer vertrauenswürdigen Zertifizierungsstelle ausgegebenen Zertifikaten verwendet wird. Wenn Sie diese Informationen angeben, können Sie die dynamische Vertrauensstellung umgehen, die auf Endbenutzergeräten angezeigt wird, wenn Sie eine Verbindung mit diesem WLAN-Netzwerk herstellen.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|AuthentifizierungsMethode, wenn der EAP-Typ auf PEAP oder EAP-TTLS konfiguriert ist. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Nicht-EAP-Methode für die Authentifizierung (innere Identität) bei EAP-TTLS und AuthenticationMethod ist username und Password. Mögliche Werte sind: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap` und `microsoftChapVersionTwo`.|
|Outeridentityprivacytemporaryvalue wurden|String|Aktivieren Sie Identitätsdatenschutz (äußere Identität), wenn der EAP-Typ für EAP-TTLS, EAP-FAST oder PEAP konfiguriert ist. Diese Eigenschaft maskiert Benutzernamen mit dem von Ihnen eingegebenen Text. Wenn Sie beispielsweise "Anonymous" verwenden, wird jeder Benutzer, der sich mit dem richtigen Benutzernamen für diese WLAN-Verbindung authentifiziert, als "Anonym" angezeigt.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1085

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1257

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




