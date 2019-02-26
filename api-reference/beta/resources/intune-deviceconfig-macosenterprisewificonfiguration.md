---
title: macOSEnterpriseWiFiConfiguration-Ressourcentyp
description: MacOS Wi-Fi WPA-Enterprise/WPA2-Enterprise-Konfigurationsprofil.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79204850256c5c8241526862c5fa7b735af633e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143323"
---
# <a name="macosenterprisewificonfiguration-resource-type"></a>macOSEnterpriseWiFiConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

MacOS Wi-Fi WPA-Enterprise/WPA2-Enterprise-Konfigurationsprofil.


Erbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MacOSEnterpriseWiFiConfigurations aufListen](../api/intune-deviceconfig-macosenterprisewificonfiguration-list.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekte.|
|[MacOSEnterpriseWiFiConfiguration abrufen](../api/intune-deviceconfig-macosenterprisewificonfiguration-get.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Lesen von Eigenschaften und Beziehungen des [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekts.|
|[MacOSEnterpriseWiFiConfiguration erstellen](../api/intune-deviceconfig-macosenterprisewificonfiguration-create.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Erstellen eines neuen [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekts.|
|[MacOSEnterpriseWiFiConfiguration löschen](../api/intune-deviceconfig-macosenterprisewificonfiguration-delete.md)|Keine|Löscht eine [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).|
|[MacOSEnterpriseWiFiConfiguration aktualisieren](../api/intune-deviceconfig-macosenterprisewificonfiguration-update.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Aktualisieren der Eigenschaften eines [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|networkName|Zeichenfolge|Netzwerk Name geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|SSID|Zeichenfolge|Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectAutomatically|Boolean|Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet. Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Verbinden, wenn das Netzwerk seinen Namen (SSID) nicht sendet. Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet. Von [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)geerbt. Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|Proxy Settings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Proxytyp für diese WLAN-Verbindung, die von [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)geerbt wurde. Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|Zeichenfolge|Die IP-Adresse oder der DNS-Hostname des Proxyservers, wenn die manuelle Konfiguration ausgewählt ist. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyManualPort|Int32|Der Proxy Server, wenn die manuelle Konfiguration ausgewählt ist. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|Zeichenfolge|URL des automatischen Konfigurationsskripts des Proxyservers, wenn die automatische Konfiguration ausgewählt ist. Diese URL ist in der Regel der Speicherort der PAC (Proxy Auto Configuration)-Datei. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|PresharedKey wurde|Zeichenfolge|Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|EAP (Extensible Authentication Protocol). Gibt den Typ des EAP-Protokolls an, das auf dem WLAN-Endpunkt (Router) festgelegt ist. Mögliche Werte sind: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap` und `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|EAP-FAST-Konfigurations Option, wenn EAP-FAST der ausgewählte EAP-Typ ist. Mögliche Werte: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|String collection|Namen von vertrauenswürdigen Servern, wenn der EAP-Typ für EAP-TLS/TTLS/FAST oder PEAP konfiguriert ist. Dies ist der allgemeine Name, der in den von Ihrer vertrauenswürdigen Zertifizierungsstelle ausgegebenen Zertifikaten verwendet wird. Wenn Sie diese Informationen angeben, können Sie die dynamische Vertrauensstellung umgehen, die auf Endbenutzergeräten angezeigt wird, wenn Sie eine Verbindung mit diesem WLAN-Netzwerk herstellen.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|AuthentifizierungsMethode, wenn der EAP-Typ auf PEAP oder EAP-TTLS konfiguriert ist. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Nicht-EAP-Methode für die Authentifizierung (innere Identität) bei EAP-TTLS und AuthenticationMethod ist username und Password. Mögliche Werte: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|Outeridentityprivacytemporaryvalue wurden|Zeichenfolge|Aktivieren Sie Identitätsdatenschutz (äußere Identität), wenn der EAP-Typ für EAP-TTLS, EAP-FAST oder PEAP konfiguriert ist. Diese Eigenschaft maskiert Benutzernamen mit dem von Ihnen eingegebenen Text. Wenn Sie beispielsweise "Anonymous" verwenden, wird jeder Benutzer, der sich mit dem richtigen Benutzernamen für diese WLAN-Verbindung authentifiziert, als "Anonym" angezeigt.|

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
|rootCertificateForServerValidation|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Vertrauenswürdiges Stammzertifikat für die Server Überprüfung, wenn EAP-Typ für EAP-TLS/TTLS/FAST oder PEAP konfiguriert ist.|
|identityCertificateForClientAuthentication|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Identitätszertifikat für die Clientauthentifizierung, wenn EAP-Typ für EAP-TLS, EAP-TTLS (mit Zertifikatauthentifizierung) oder PEAP (mit Zertifikatauthentifizierung) konfiguriert ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```




