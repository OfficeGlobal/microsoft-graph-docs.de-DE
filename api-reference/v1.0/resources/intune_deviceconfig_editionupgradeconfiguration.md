# <a name="editionupgradeconfiguration-resource-type"></a>editionUpgradeConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Editionsupgradekonfiguration Windows 10

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[editionUpgradeConfigurations auflisten](../api/intune_deviceconfig_editionupgradeconfiguration_list.md)|[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)-Objekte.|
|[editionUpgradeConfiguration abrufen](../api/intune_deviceconfig_editionupgradeconfiguration_get.md)|[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)-Objekts.|
|[editionUpgradeConfiguration erstellen](../api/intune_deviceconfig_editionupgradeconfiguration_create.md)|[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)|Erstellen eines neuen [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)-Objekts.|
|[editionUpgradeConfiguration löschen](../api/intune_deviceconfig_editionupgradeconfiguration_delete.md)|Keine|Löscht eine [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).|
|[editionUpgradeConfiguration aktualisieren](../api/intune_deviceconfig_editionupgradeconfiguration_update.md)|[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)|Aktualisieren der Eigenschaften eines [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|licenseType|[editionUpgradeLicenseType](../resources/intune_deviceconfig_editionupgradelicensetype.md)|Lizenztyp der Editionsaktualisierung. Mögliche Werte: `productKey`, `licenseFile`.|
|targetEdition|[windows10EditionType](../resources/intune_deviceconfig_windows10editiontype.md)|Zieledition der Editionsaktualisierung. Mögliche Werte: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.|
|Lizenz|Zeichenfolge|Inhalt der Edition Upgrade-Lizenzdatei|
|productKey|Zeichenfolge|Produktschlüssel des Editionsupgrades.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Aufgaben|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.editionUpgradeConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "licenseType": "String",
  "targetEdition": "String",
  "license": "String",
  "productKey": "String"
}
```








