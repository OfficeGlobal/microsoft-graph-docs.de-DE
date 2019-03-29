---
title: WindowsDeliveryOptimizationConfiguration erstellen
description: Erstellen eines neuen windowsDeliveryOptimizationConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 373d47737e46ef6046ff1c88c44f7b2ff3a25029
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964185"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a>WindowsDeliveryOptimizationConfiguration erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekts.

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
Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsDeliveryOptimizationConfiguration-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsDeliveryOptimizationConfiguration erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Gibt die Downloadmethode an, die von der Zustellungsoptimierung zur Verwaltung der Netzwerkbandbreite bei umfangreichen Inhalts Verteilungsszenarien verwendet werden kann. Mögliche Werte: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
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
|modifyCacheLocation|String|Gibt das Laufwerk an, das von der BereitstellungsOptimierung für den Cache verwendet werden soll.|
|maximumCacheAgeInDays|Int32|Gibt die maximale Zeitdauer in Tagen an, die jede Datei im Bereitstellungs Optimierungs Cache aufbewahrt wird, nachdem Sie erfolgreich heruntergeladen wurde (0-49710). Gültige Werte 0 bis 49710|
|maximumCacheSize|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|Gibt die maximale Cachegröße an, die von der zugestellten Optimierung als Prozentsatz oder in GB angegeben wird.|
|vpnPeerCaching|[Aktivierung](../resources/intune-shared-enablement.md)|Gibt an, ob das Gerät an Peer-Zwischenspeicherung während der Verbindung über VPN mit dem Domänennetzwerk teilnehmen darf. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1060

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1232

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```




