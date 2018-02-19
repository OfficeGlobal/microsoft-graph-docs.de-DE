# <a name="deviceconfigurationdevicestatesummary-resource-type"></a>deviceConfigurationDeviceStateSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceConfigurationDeviceStateSummary abrufen](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)-Objekts.|
|[deviceConfigurationDeviceStateSummary aktualisieren](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|
|unknownDeviceCount|Int32|Anzahl unbekannter Geräte|
|notApplicableDeviceCount|Int32|Anzahl nicht anwendbarer Geräte|
|compliantDeviceCount|Int32|Anzahl der konformen Geräte|
|remediatedDeviceCount|Int32|Anzahl korrigierter Geräte|
|nonCompliantDeviceCount|Int32|Anzahl der nicht konformen Geräte|
|errorDeviceCount|Int32|Anzahl der fehlerhaften Geräte|
|conflictDeviceCount|Int32|Anzahl der Geräte mit Konflikten|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
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



