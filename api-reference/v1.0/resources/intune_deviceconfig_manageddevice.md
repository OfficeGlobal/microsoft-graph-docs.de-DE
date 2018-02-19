# <a name="manageddevice-resource-type"></a>managedDevice-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Über Intune verwaltete oder vorab registrierte Geräte
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDevices auflisten](../api/intune_deviceconfig_manageddevice_list.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedDevice](../resources/intune_deviceconfig_manageddevice.md)-Objekte.|
|[managedDevice abrufen](../api/intune_deviceconfig_manageddevice_get.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md)|Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune_deviceconfig_manageddevice.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceConfigurationStates|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Sammlung|Gerätekonfigurationsstatus für dieses Gerät.|
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Sammlung|Status der Gerätekonformitätsrichtlinie für dieses Gerät.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



