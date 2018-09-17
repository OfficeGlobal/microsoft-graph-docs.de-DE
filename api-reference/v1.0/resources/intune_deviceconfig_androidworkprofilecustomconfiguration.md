# <a name="androidworkprofilecustomconfiguration-resource-type"></a>Ressourcentyp androidWorkProfileCustomConfiguration

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Benutzerdefinierte Konfiguration für das Android-Arbeitsprofil

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von androidWorkProfileCustomConfigurations](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_list.md)|[AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)-Objekte.|
|[Abrufen von androidWorkProfileCustomConfiguration](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_get.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|Leseeigenschaften und Beziehungen des [AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)-Objekts.|
|[Erstellen von androidWorkProfileCustomConfiguration](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_create.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|Erstellen eines neuen [AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)-Objekts.|
|[AndroidWorkProfileCustomConfiguration löschen](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_delete.md)|Keine|Löscht [AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).|
|[AndroidWorkProfileCustomConfiguration aktualisieren](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_update.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|Aktualisieren der Eigenschaften eines [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|omaSettings|Collection von Objekten des Typs [omaSetting](../resources/intune_deviceconfig_omasetting.md)|OMA-Einstellungen. Diese Collection darf maximal 500 Elemente enthalten.|

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
  "@odata.type": "microsoft.graph.androidWorkProfileCustomConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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








