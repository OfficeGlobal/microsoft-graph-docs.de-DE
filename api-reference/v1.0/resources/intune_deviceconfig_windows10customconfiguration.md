# <a name="windows10customconfiguration-resource-type"></a>windows10CustomConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Dieses Thema enthält eine Beschreibung der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Ressource windows10CustomConfiguration verfügbar gemacht werden.

Erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Windows10CustomConfigurations auflisten](../api/intune_deviceconfig_windows10customconfiguration_list.md)|[windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)-Objekte.|
|[Windows10CustomConfiguration abrufen](../api/intune_deviceconfig_windows10customconfiguration_get.md)|[windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)-Objekts.|
|[Windows10CustomConfiguration erstellen](../api/intune_deviceconfig_windows10customconfiguration_create.md)|[windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)|Erstellen eines neuen [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)-Objekts.|
|[Windows10CustomConfiguration löschen](../api/intune_deviceconfig_windows10customconfiguration_delete.md)|Keine|Löscht ein [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)-Objekt.|
|[Windows10CustomConfiguration aktualisieren](../api/intune_deviceconfig_windows10customconfiguration_update.md)|[windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)|Aktualisieren der Eigenschaften eines [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Vom Administrator bereitgestellter Name der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|omaSettings|[omaSetting](../resources/intune_deviceconfig_omasetting.md)-Sammlung|OMA-Einstellungen. Diese Sammlung kann bis zu 1000 Elemente enthalten.|

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
  "@odata.type": "microsoft.graph.windows10CustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "String",
      "description": "String",
      "omaUri": "String",
      "value": 1024
    }
  ]
}
```



