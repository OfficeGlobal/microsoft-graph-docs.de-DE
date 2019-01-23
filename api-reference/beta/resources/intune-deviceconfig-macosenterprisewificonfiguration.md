---
title: Ressourcentyp macOSEnterpriseWiFiConfiguration
description: Mac OS Wi-Fi WPA-Enterprise/WPA2-Enterprise Konfigurationsprofil.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ec5bc6a3540241355a4574e85684e0cdf26f8ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425890"
---
# <a name="macosenterprisewificonfiguration-resource-type"></a>Ressourcentyp macOSEnterpriseWiFiConfiguration

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mac OS Wi-Fi WPA-Enterprise/WPA2-Enterprise Konfigurationsprofil.


Erbt vom [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste macOSEnterpriseWiFiConfigurations](../api/intune-deviceconfig-macosenterprisewificonfiguration-list.md)|[MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekte.|
|[Abrufen von macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-get.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekts.|
|[Erstellen von macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-create.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Erstellen eines neuen [MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekts.|
|[MacOSEnterpriseWiFiConfiguration löschen](../api/intune-deviceconfig-macosenterprisewificonfiguration-delete.md)|Keine|Löscht eine [MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).|
|[MacOSEnterpriseWiFiConfiguration aktualisieren](../api/intune-deviceconfig-macosenterprisewificonfiguration-update.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Aktualisieren Sie die Eigenschaften eines [MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Zeichenfolgenauflistung|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Netzwerkname|Zeichenfolge|Netzwerk Namen von [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) geerbt.|
|SSID|Zeichenfolge|Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectAutomatically|Boolean|Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet. Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Verbinden Sie, wenn das Netzwerk seinen Namen (SSID) nicht übertragen wird. Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird. Geerbt von [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md). Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Proxytyp für diese Wi-Fi-Verbindung Inherited aus [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md). Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|Zeichenfolge|IP-Adresse oder den DNS-Hostnamen des Proxyservers bei der manueller Konfiguration ausgewählt ist. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyManualPort|Int32|Die Portnummer des Proxyservers bei der manueller Konfiguration ausgewählt ist. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|Zeichenfolge|URL des eigentlichen Skripts Proxy Server automatische Konfiguration automatische Konfiguration aktiviert ist. Diese URL hat normalerweise den Speicherort der Datei PAC (Proxy Automatische Konfiguration). Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|preSharedKey|Zeichenfolge|Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk. Geerbt von [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Extensible Authentication-Protokoll (EAP). Gibt den Typ des EAP-Protokolls festlegen für den die Wi-Fi-Endpunkt (Router). Mögliche Werte sind: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap` und `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|EAP-FAST Konfigurationsoption wenn EAP-FAST den ausgewählten EAP-Typ ist. Mögliche Werte: sind `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision` und `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|Zeichenfolgenauflistung|Vertrauenswürdige Zertifikat Servernamen an, wenn EAP-Typ EAP-TLS/TTLS/FAST oder PEAP konfiguriert ist. Dies ist der allgemeine Name in Zertifikate der vertrauenswürdigen Zertifizierungsstelle (CA) verwendet. Wenn Sie diese Informationen bereitstellen, können Sie die dynamische vertrauensdialogfeld umgehen, die auf Geräten für Endbenutzer angezeigt wird, wenn sie mit diesem Wi-Fi-Netzwerk zu verbinden.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Authentifizierungsmethode beim EAP-Typ PEAP oder EAP-TTLS konfiguriert ist. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Nicht-EAP-Methode für die Authentifizierung (innere) beim Identität EAP-Typ EAP-TTLS ist und AuthenticationMethod-ist Benutzername und Kennwort. Mögliche Werte: sind `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap` und `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Zeichenfolge|Aktivieren Sie EAP-TTLS, EAP-FAST oder PEAP Identität Privacy (externe Identität) Wenn EAP-Typ konfiguriert ist. Diese Eigenschaft maskiert Benutzernamen mit dem Text, die, den Sie eingeben. Wenn Sie "anonymen" verwenden, wird jeder Benutzer, die mit dieser Wi-Fi-Verbindung mit der echten Benutzernamen authentifiziert "Anonym" angezeigt.|

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
|rootCertificateForServerValidation|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Vertrauenswürdige Stammzertifikat für die gültigkeitsprüfung des Servers an, wenn EAP-Typ EAP-TLS/TTLS/FAST oder PEAP konfiguriert ist.|
|identityCertificateForClientAuthentication|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Identity-Zertifikat für die Clientauthentifizierung beim EAP-Typ EAP-TLS, EAP-TTLS (mit zertifikatbasierter Authentifizierung) oder PEAP (mit Zertifikatauthentifizierung) konfiguriert ist.|

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




