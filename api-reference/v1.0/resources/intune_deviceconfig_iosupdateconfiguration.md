# <a name="iosupdateconfiguration-resource-type"></a>iosUpdateConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mit dieser iOS-Updatekonfiguration können Sie ein Zeitfenster innerhalb einer Woche zum Installieren von Updates für iOS konfigurieren.

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosUpdateConfigurations auflisten](../api/intune_deviceconfig_iosupdateconfiguration_list.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekte.|
|[iosUpdateConfiguration abrufen](../api/intune_deviceconfig_iosupdateconfiguration_get.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekts.|
|[iosUpdateConfiguration erstellen](../api/intune_deviceconfig_iosupdateconfiguration_create.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Erstellen eines neuen [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekts.|
|[iosUpdateConfiguration löschen](../api/intune_deviceconfig_iosupdateconfiguration_delete.md)|Keine|Löscht ein [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekt.|
|[iosUpdateConfiguration aktualisieren](../api/intune_deviceconfig_iosupdateconfiguration_update.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Aktualisieren der Eigenschaften eines [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|activeHoursStart|TimeOfDay|Beginn der aktiven Stunden (als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Installation von Updates ausgeführt werden soll)|
|activeHoursEnd|TimeOfDay|Ende der aktiven Stunden (als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Installation von Updates ausgeführt werden soll)|
|scheduledInstallDays|[DayOfWeek](../resources/intune_deviceconfig_dayofweek.md) -Auflistung|Tage in der Woche, für die aktive Stunden konfiguriert sind. Diese Sammlung darf maximal 7 Elemente enthalten.|
|utcTimeOffsetInMinutes|Int32|UTC-Zeitversatz in Minuten|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024
}
```



<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune_deviceconfig_iosupdateconfiguration.md/microsoft.graph.iosUpdateConfiguration/scheduledInstallDays:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
