# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune_deviceconfig_devicemanagement_get.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune_deviceconfig_devicemanagement_update.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner|
|settings|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|Einstellungen auf Kontoebene|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceConfigurations|[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)-Sammlung|Die Gerätekonfigurationen|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)-Sammlung|Die Gerätekompatibilitätsrichtlinie|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|Die Softwareaktualisierungs-Statuszusammenfassung|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|Die Gerätekompatibilitäts-Statuszusammenfassung für dieses Konto|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Sammlung|Die Zusammenfassungsstatus von Kompatibilitätsrichtlinieneinstellungen für dieses Konto|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|Die Gerätekonfigurations-Gerätestatuszusammenfassung für dieses Konto.|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Sammlung|Die IOS-Softwareupdate-Installationsstatus für dieses Konto|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



