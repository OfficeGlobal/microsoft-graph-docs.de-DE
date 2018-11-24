# <a name="deviceconfigurationdevicestatus-resource-type"></a>deviceConfigurationDeviceStatus-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceConfigurationDeviceStatuses auflisten](../api/intune_deviceconfig_deviceconfigurationdevicestatus_list.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Objekte.|
|[deviceConfigurationDeviceStatus abrufen](../api/intune_deviceconfig_deviceconfigurationdevicestatus_get.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Objekts.|
|[deviceConfigurationDeviceStatus erstellen](../api/intune_deviceconfig_deviceconfigurationdevicestatus_create.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Erstellen eines neuen [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Objekts.|
|[deviceConfigurationDeviceStatus löschen](../api/intune_deviceconfig_deviceconfigurationdevicestatus_delete.md)|Keine|Löscht ein [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Objekt.|
|[deviceConfigurationDeviceStatus aktualisieren](../api/intune_deviceconfig_deviceconfigurationdevicestatus_update.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|
|deviceDisplayName|String|Gerätename des DevicePolicyStatus|
|userName|String|Der gemeldete Benutzername|
|deviceModel|String|Das gemeldete Gerätemodell|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität|
|status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Konformitätsstatus des Richtlinienberichts. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Richtlinienberichts|
|userPrincipalName|String|UserPrincipalName.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



