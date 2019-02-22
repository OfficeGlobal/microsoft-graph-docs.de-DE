---
title: iosWiFiConfiguration-Ressourcentyp
description: Durch die Bereitstellung der Konfigurationen in diesem Profil können Sie das iOS-Gerät anweisen, eine Verbindung mit dem gewünschten WLAN-Endpunkt herzustellen. Durch die Angabe der Authentifizierungsmethode und der von WLAN-Endpunkten erwarteten Sicherheitstypen können Sie die WLAN-Verbindung für Endbenutzer nahtlos ausführen. Dieses Profil bietet begrenzte und einfachere Sicherheitstypen als Enterprise-Wi-Fi-Profil.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a2fdf4f17983c0e7fc3688ee630549101cb9295
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166584"
---
# <a name="ioswificonfiguration-resource-type"></a>iosWiFiConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Durch die Bereitstellung der Konfigurationen in diesem Profil können Sie das iOS-Gerät anweisen, eine Verbindung mit dem gewünschten WLAN-Endpunkt herzustellen. Durch die Angabe der Authentifizierungsmethode und der von WLAN-Endpunkten erwarteten Sicherheitstypen können Sie die WLAN-Verbindung für Endbenutzer nahtlos ausführen. Dieses Profil bietet begrenzte und einfachere Sicherheitstypen als Enterprise-Wi-Fi-Profil.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[IosWiFiConfigurations aufListen](../api/intune-deviceconfig-ioswificonfiguration-list.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekte.|
|[IosWiFiConfiguration abrufen](../api/intune-deviceconfig-ioswificonfiguration-get.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Lesen von Eigenschaften und Beziehungen des [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekts.|
|[IosWiFiConfiguration erstellen](../api/intune-deviceconfig-ioswificonfiguration-create.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Erstellen eines neuen [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekts.|
|[IosWiFiConfiguration löschen](../api/intune-deviceconfig-ioswificonfiguration-delete.md)|Keine|Löscht eine [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).|
|[IosWiFiConfiguration aktualisieren](../api/intune-deviceconfig-ioswificonfiguration-update.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Aktualisieren der Eigenschaften eines [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekts.|

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
|networkName|Zeichenfolge|Netzwerk Name|
|SSID|Zeichenfolge|Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird.|
|connectAutomatically|Boolescher Wert|Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet. Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden.|
|connectWhenNetworkNameIsHidden|Boolescher Wert|Verbinden, wenn das Netzwerk seinen Namen (SSID) nicht sendet. Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt.|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet. Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.|
|Proxy Settings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Proxytyp für diese WLAN-Verbindung. Mögliche Werte sind: `none`, `manual` und `automatic`.|
|proxyManualAddress|Zeichenfolge|Die IP-Adresse oder der DNS-Hostname des Proxyservers, wenn die manuelle Konfiguration ausgewählt ist.|
|proxyManualPort|Int32|Der Proxy Server, wenn die manuelle Konfiguration ausgewählt ist.|
|proxyAutomaticConfigurationUrl|Zeichenfolge|URL des automatischen Konfigurationsskripts des Proxyservers, wenn die automatische Konfiguration ausgewählt ist. Diese URL ist in der Regel der Speicherort der PAC (Proxy Auto Configuration)-Datei.|
|PresharedKey wurde|Zeichenfolge|Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk.|

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
  "@odata.type": "microsoft.graph.iosWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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




