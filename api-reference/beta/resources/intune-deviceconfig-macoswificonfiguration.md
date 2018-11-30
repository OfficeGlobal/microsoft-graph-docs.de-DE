---
title: Ressourcentyp macOSWiFiConfiguration
description: Durch die Konfigurationen in dieses Profil bereitstellen können Sie das Gerät Mac OS Verbindung zum gewünschten Wi-Fi-Endpunkt anweisen. Durch Angeben von erwartet, dass die Authentifizierungstypen-Methode und der Sicherheit durch Wi-Fi-Endpunkt, dass Sie die Wi-Fi-Verbindung nahtlos für Endbenutzer vornehmen können.
ms.openlocfilehash: 79dd9cc4b9e98bb0aa3d65a2d15afb6867ecee63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064053"
---
# <a name="macoswificonfiguration-resource-type"></a>Ressourcentyp macOSWiFiConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Durch die Konfigurationen in dieses Profil bereitstellen können Sie das Gerät Mac OS Verbindung zum gewünschten Wi-Fi-Endpunkt anweisen. Durch Angeben von erwartet, dass die Authentifizierungstypen-Methode und der Sicherheit durch Wi-Fi-Endpunkt, dass Sie die Wi-Fi-Verbindung nahtlos für Endbenutzer vornehmen können.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste macOSWiFiConfigurations](../api/intune-deviceconfig-macoswificonfiguration-list.md)|[MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) -Objekte.|
|[Abrufen von macOSWiFiConfiguration](../api/intune-deviceconfig-macoswificonfiguration-get.md)|[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) -Objekts.|
|[Erstellen von macOSWiFiConfiguration](../api/intune-deviceconfig-macoswificonfiguration-create.md)|[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|Erstellen eines neuen [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) -Objekts.|
|[MacOSWiFiConfiguration löschen](../api/intune-deviceconfig-macoswificonfiguration-delete.md)|Keines|Löscht eine [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).|
|[MacOSWiFiConfiguration aktualisieren](../api/intune-deviceconfig-macoswificonfiguration-update.md)|[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|Aktualisieren Sie die Eigenschaften eines [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) -Objekts.|

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
|Netzwerkname|String|Netzwerkname|
|SSID|String|Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird.|
|connectAutomatically|Boolesch|Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet. Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden.|
|connectWhenNetworkNameIsHidden|Boolesch|Verbinden Sie, wenn das Netzwerk seinen Namen (SSID) nicht übertragen wird. Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine.|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird. Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Proxytyp für diese Wi-Fi-Verbindung. Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|String|IP-Adresse oder den DNS-Hostnamen des Proxyservers bei der manueller Konfiguration ausgewählt ist.|
|proxyManualPort|Int32|Die Portnummer des Proxyservers bei der manueller Konfiguration ausgewählt ist.|
|proxyAutomaticConfigurationUrl|String|URL des eigentlichen Skripts Proxy Server automatische Konfiguration automatische Konfiguration aktiviert ist. Diese URL hat normalerweise den Speicherort der Datei PAC (Proxy Automatische Konfiguration).|
|preSharedKey|String|Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk.|

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
  "@odata.type": "microsoft.graph.macOSWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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
  "preSharedKey": "String"
}
```





