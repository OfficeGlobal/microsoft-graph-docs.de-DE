---
title: windowsDeliveryOptimizationConfiguration-Ressourcentyp
description: Konfiguration der Windows-BereitstellungsOptimierung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62fef7e874f004c28f71287895e84005c93905b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162090"
---
# <a name="windowsdeliveryoptimizationconfiguration-resource-type"></a>windowsDeliveryOptimizationConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Konfiguration der Windows-BereitstellungsOptimierung


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsDeliveryOptimizationConfigurations aufListen](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-list.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekte.|
|[WindowsDeliveryOptimizationConfiguration abrufen](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-get.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekts.|
|[WindowsDeliveryOptimizationConfiguration erstellen](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-create.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Erstellen eines neuen [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekts.|
|[WindowsDeliveryOptimizationConfiguration löschen](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-delete.md)|Keine|Löscht eine [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).|
|[WindowsDeliveryOptimizationConfiguration aktualisieren](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-update.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Aktualisieren der Eigenschaften eines [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Gibt die Downloadmethode an, die von der Zustellungsoptimierung zur Verwaltung der Netzwerkbandbreite bei umfangreichen Inhalts Verteilungsszenarien verwendet werden kann. Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.|
|restrictPeerSelectionBy|[deliveryOptimizationRestrictPeerSelectionByOptions](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|Gibt an, dass die Peer Auswahl über die ausgewählte Option eingeschränkt werden soll.
Option 1 (subNetzmaske) gilt nur für die Bereitstellungs Optimierungs Modi Download Modus LAN (1) und Gruppe (2). Mögliche Werte sind: `notConfigured` und `subnetMask`.|
|groupIdSource|[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|Gibt an, dass die Peer Auswahl auf eine Specfic-Quelle beschränkt werden soll.
Die in dieser Richtlinie festgelegten Optionen gelten nur für den Downloadmodus für den Bereitstellungs Optimierungsmodus (2). Wenn die Gruppe (2) nicht als Download Modus festgelegt ist, wird diese Richtlinie ignoriert. Bei Option 3-DHCP-Options-ID fragt der Client die DHCP-Optionskennung 234 ab und verwendet den zurückgegebenen GUID-Wert als Gruppen-ID.|
|bandwidthMode|[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|Gibt die Nutzung von Vordergrund-und Hintergrund Bandbreite unter Verwendung von Prozentsätzen, absoluten Werten oder Stunden an.|
|backgroundDownloadFromHttpDelayInSeconds|Int64|Gibt die Anzahl der Sekunden an, die eine HTTP-Quelle in einem Hintergrund Download verzögert werden soll, der die Verwendung von Peer-to-Peer ermöglicht. Gültige Werte 0 bis 4294967295|
|foregroundDownloadFromHttpDelayInSeconds|Int64|Gibt die Anzahl von Sekunden an, die eine HTTP-Quelle in einem Vordergrund heruntergeladen wird, für die Peer-to-Peer (0-86400) verwendet werden darf. Gültige Werte 0 bis 86400
Durch Angeben von 0 wird die zuStellungsOptimierung zum Verwalten dieser Einstellung mithilfe des Cloud-Diensts festgelegt. Gültige Werte 0 bis 86400|
|minimumRamAllowedToPeerInGigabytes|Int32|Gibt die minimale RAM-Größe in GB an, um die Peer Zwischenspeicherung zu verwenden (1-100000). Gültige Werte 1 bis 100000|
|minimumDiskSizeAllowedToPeerInGigabytes|Int32|Gibt die minimale Datenträgergröße in GB für die Verwendung der Peer Zwischenspeicherung an (1-100000). Gültige Werte 1 bis 100000
Empfohlene Werte: 64 GB bis 256 GB. Gültige Werte 1 bis 100000|
|minimumFileSizeToCacheInMegabytes|Int32|Gibt die minimale Größe der Inhaltsdatei in MB an, die für die Verwendung der Peer Zwischenspeicherung aktiviert ist (1-100000). Gültige Werte 1 bis 100000
Empfohlene Werte: 1 MB bis 100.000 MB. Gültige Werte 1 bis 100000|
|minimumBatteryPercentageAllowedToUpload|Int32|Gibt den Mindestprozentsatz für die Batterie an, damit das Gerät Daten hochladen kann (0-100). Gültige Werte: 0 bis 100.
Der Standardwert ist 0. Der Wert 0 (null) ist "unbegrenzt" und der Standardwert des Cloud-Diensts wird verwendet. Gültige Werte: 0 bis 100.|
|modifyCacheLocation|Zeichenfolge|Gibt das Laufwerk an, das von der BereitstellungsOptimierung für den Cache verwendet werden soll.|
|maximumCacheAgeInDays|Int32|Gibt die maximale Zeitdauer in Tagen an, die jede Datei im Bereitstellungs Optimierungs Cache aufbewahrt wird, nachdem Sie erfolgreich heruntergeladen wurde (0-49710). Gültige Werte 0 bis 49710|
|maximumCacheSize|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|Gibt die maximale Cachegröße an, die von der zugestellten Optimierung als Prozentsatz oder in GB angegeben wird.|
|vpnPeerCaching|[Aktivierung](../resources/intune-shared-enablement.md)|Gibt an, ob das Gerät an Peer-Zwischenspeicherung während der Verbindung über VPN mit dem Domänennetzwerk teilnehmen darf. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|

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
  "@odata.type": "microsoft.graph.windowsDeliveryOptimizationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "deliveryOptimizationMode": "String",
  "restrictPeerSelectionBy": "String",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 1024,
  "foregroundDownloadFromHttpDelayInSeconds": 1024,
  "minimumRamAllowedToPeerInGigabytes": 1024,
  "minimumDiskSizeAllowedToPeerInGigabytes": 1024,
  "minimumFileSizeToCacheInMegabytes": 1024,
  "minimumBatteryPercentageAllowedToUpload": 1024,
  "modifyCacheLocation": "String",
  "maximumCacheAgeInDays": 1024,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "String"
}
```




