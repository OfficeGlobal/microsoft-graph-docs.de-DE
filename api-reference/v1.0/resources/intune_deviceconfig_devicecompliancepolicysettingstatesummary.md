# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>deviceCompliancePolicySettingStateSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zusammenfassung des Zustands der Gerätekonformitätsrichtlinien-Einstellung für das Konto.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceCompliancePolicySettingStateSummaries auflisten](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_list.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekte.|
|[deviceCompliancePolicySettingStateSummary abrufen](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Lesen von Eigenschaften und Beziehungen der [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekte.|
|[deviceCompliancePolicySettingStateSummary erstellen](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Erstellen eines neuen [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekts.|
|[deviceCompliancePolicySettingStateSummary löschen](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_delete.md)|Keine|Löschen einer [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).|
|[deviceCompliancePolicySettingStateSummary aktualisieren](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Aktualisieren der Eigenschaften eines [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|setting|Zeichenfolge|Der Klassenname und der Eigenschaftenname der Einstellung.|
|settingName|Zeichenfolge|Der Name der Einstellung.|
|platformType|Zeichenfolge|Die Plattform der Einstellung. Mögliche Werte: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.|
|id|Zeichenfolge|Schlüssel der Entität|
|unknownDeviceCount|Int32|Anzahl unbekannter Geräte|
|notApplicableDeviceCount|Int32|Anzahl nicht anwendbarer Geräte|
|compliantDeviceCount|Int32|Anzahl der konformen Geräte|
|remediatedDeviceCount|Int32|Anzahl korrigierter Geräte|
|nonCompliantDeviceCount|Int32|Anzahl der nicht konformen Geräte|
|errorDeviceCount|Int32|Anzahl der fehlerhaften Geräte|
|conflictDeviceCount|Int32|Anzahl der Geräte mit Konflikten|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceComplianceSettingStates|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Sammlung|Noch nicht dokumentiert.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



