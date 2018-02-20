# <a name="macoscustomconfiguration-resource-type"></a>macOSCustomConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Dieses Thema enthält eine Beschreibung der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Ressource macOSCustomConfiguration verfügbar gemacht werden.

Erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MacOSCustomConfigurations auflisten](../api/intune_deviceconfig_macoscustomconfiguration_list.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)-Objekte.|
|[MacOSCustomConfiguration abrufen](../api/intune_deviceconfig_macoscustomconfiguration_get.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)-Objekts.|
|[MacOSCustomConfiguration erstellen](../api/intune_deviceconfig_macoscustomconfiguration_create.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)|Erstellen eines neuen [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)-Objekts.|
|[MacOSCustomConfiguration löschen](../api/intune_deviceconfig_macoscustomconfiguration_delete.md)|Keine|Löscht ein [MacOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)-Objekt.|
|[MacOSCustomConfiguration aktualisieren](../api/intune_deviceconfig_macoscustomconfiguration_update.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)|Aktualisieren der Eigenschaften eines [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Vom Administrator bereitgestellter Name der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|payloadName|String|Name, der dem Benutzer angezeigt wird.|
|payloadFileName|String|Name der Nutzlastdatei (*.mobileconfig | *.xml).|
|payload|Binary|Nutzlast. (UTF8-codiertes Bytearray)|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Die Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über Gerätestatus der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über Benutzerstatus der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Status der Gerätekonfigurationseinstellungen der Geräte. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSCustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```


