# <a name="windowsphone81customconfiguration-resource-type"></a>windowsPhone81CustomConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Dieses Thema enthält eine Beschreibung der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Ressource windowsPhone81CustomConfiguration verfügbar gemacht werden.

Erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsPhone81CustomConfigurations auflisten](../api/intune_deviceconfig_windowsphone81customconfiguration_list.md)|[windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)-Objekte.|
|[WindowsPhone81CustomConfiguration abrufen](../api/intune_deviceconfig_windowsphone81customconfiguration_get.md)|[windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)-Objekts.|
|[WindowsPhone81CustomConfiguration erstellen](../api/intune_deviceconfig_windowsphone81customconfiguration_create.md)|[windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)|Erstellen eines neuen [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)-Objekts.|
|[WindowsPhone81CustomConfiguration löschen](../api/intune_deviceconfig_windowsphone81customconfiguration_delete.md)|Keine|Löscht ein [WindowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)-Objekt.|
|[WindowsPhone81CustomConfiguration aktualisieren](../api/intune_deviceconfig_windowsphone81customconfiguration_update.md)|[windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)|Aktualisieren der Eigenschaften eines [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|omaSettings|[omaSetting](../resources/intune_deviceconfig_omasetting.md)-Sammlung|OMA-Einstellungen. Diese Sammlung kann bis zu 1000 Elemente enthalten.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über Gerätestatus der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über Benutzerstatus der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Status der Gerätekonfigurationseinstellungen der Geräte. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81CustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "String",
      "description": "String",
      "omaUri": "String",
      "value": 1024
    }
  ]
}
```



