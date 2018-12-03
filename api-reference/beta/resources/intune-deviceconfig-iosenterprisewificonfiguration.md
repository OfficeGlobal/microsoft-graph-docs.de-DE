---
title: Ressourcentyp iosEnterpriseWiFiConfiguration
description: Durch die Konfigurationen in dieses Profil bereitstellen, können Sie das Gerät iOS Verbindung zum gewünschten Wi-Fi-Endpunkt anweisen. Durch Angeben von erwartet, dass die Authentifizierungstypen-Methode und der Sicherheit durch Wi-Fi-Endpunkt, dass Sie die Wi-Fi-Verbindung nahtlos für Endbenutzer vornehmen können.
ms.openlocfilehash: 156a93afd9c94db23c0983deeda3a50e5926577e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060034"
---
# <a name="iosenterprisewificonfiguration-resource-type"></a>Ressourcentyp iosEnterpriseWiFiConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Durch die Konfigurationen in dieses Profil bereitstellen, können Sie das Gerät iOS Verbindung zum gewünschten Wi-Fi-Endpunkt anweisen. Durch Angeben von erwartet, dass die Authentifizierungstypen-Methode und der Sicherheit durch Wi-Fi-Endpunkt, dass Sie die Wi-Fi-Verbindung nahtlos für Endbenutzer vornehmen können.

Erbt vom [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste iosEnterpriseWiFiConfigurations](../api/intune-deviceconfig-iosenterprisewificonfiguration-list.md)|[IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) -Objekte.|
|[Abrufen von iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-get.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) -Objekts.|
|[Erstellen von iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-create.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Erstellen eines neuen [IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) -Objekts.|
|[IosEnterpriseWiFiConfiguration löschen](../api/intune-deviceconfig-iosenterprisewificonfiguration-delete.md)|Keines|Löscht eine [IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).|
|[IosEnterpriseWiFiConfiguration aktualisieren](../api/intune-deviceconfig-iosenterprisewificonfiguration-update.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Aktualisieren Sie die Eigenschaften eines [IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Netzwerkname|String|Netzwerk Namen von [IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) geerbt.|
|SSID|String|Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird. Geerbt von [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectAutomatically|Boolesch|Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet. Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden. Geerbt von [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolesch|Verbinden Sie, wenn das Netzwerk seinen Namen (SSID) nicht übertragen wird. Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine. Geerbt von [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird. Geerbt von [IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Proxytyp für diese Wi-Fi-Verbindung Inherited aus [IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|String|IP-Adresse oder den DNS-Hostnamen des Proxyservers bei der manueller Konfiguration ausgewählt ist. Geerbt von [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyManualPort|Int32|Die Portnummer des Proxyservers bei der manueller Konfiguration ausgewählt ist. Geerbt von [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|URL des eigentlichen Skripts Proxy Server automatische Konfiguration automatische Konfiguration aktiviert ist. Diese URL hat normalerweise den Speicherort der Datei PAC (Proxy Automatische Konfiguration). Geerbt von [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|preSharedKey|String|Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk. Geerbt von [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Extensible Authentication-Protokoll (EAP). Gibt den Typ des EAP-Protokolls festlegen für den die Wi-Fi-Endpunkt (Router). Mögliche Werte sind: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap` und `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|EAP-FAST Konfigurationsoption wenn EAP-FAST den ausgewählten EAP-Typ ist. Mögliche Werte: sind `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision` und `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|Collection von Objekten des Typs „String“|Vertrauenswürdige Zertifikat Servernamen an, wenn EAP-Typ EAP-TLS/TTLS/FAST oder PEAP konfiguriert ist. Dies ist der allgemeine Name in Zertifikate der vertrauenswürdigen Zertifizierungsstelle (CA) verwendet. Wenn Sie diese Informationen bereitstellen, können Sie die dynamische vertrauensdialogfeld umgehen, die auf Geräten für Endbenutzer angezeigt wird, wenn sie mit diesem Wi-Fi-Netzwerk zu verbinden.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Authentifizierungsmethode beim EAP-Typ PEAP oder EAP-TTLS konfiguriert ist. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Nicht-EAP-Methode für die Authentifizierung bei EAP-Typ EAP-TTLS und AuthenticationMethod-ist ist Benutzername und Kennwort. Mögliche Werte: sind `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap` und `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Identität Privacy (externe Identität) aktivieren, wenn EAP-Typ EAP - TTLS EAP - konfiguriert ist FAST oder PEAP. Diese Eigenschaft maskiert Benutzernamen mit dem Text, die, den Sie eingeben. Wenn Sie "anonymen" verwenden, wird jeder Benutzer, die mit dieser Wi-Fi-Verbindung mit der echten Benutzernamen authentifiziert "Anonym" angezeigt.|

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
|rootCertificatesForServerValidation|[IosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) -Auflistung|Vertrauenswürdige Stammzertifikate für die gültigkeitsprüfung des Servers an, wenn EAP-Typ EAP-TLS/TTLS/FAST oder PEAP konfiguriert ist. Wenn Sie diesen Wert angeben, nicht TrustedServerCertificateNames, bereitstellen müssen, und umgekehrt.|
|identityCertificateForClientAuthentication|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Identity-Zertifikat für die Clientauthentifizierung beim EAP-Typ EAP-TLS, EAP-TTLS (mit zertifikatbasierter Authentifizierung) oder PEAP (mit Zertifikatauthentifizierung) konfiguriert ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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





