# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a>managedDeviceMobileAppConfigurationAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält die Eigenschaften, mit denen eine MDM-App-Konfiguration zu einer Gruppe zugewiesen wird.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurationAssignments auflisten](../api/intune_apps_manageddevicemobileappconfigurationassignment_list.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Objekte.|
|[managedDeviceMobileAppConfigurationAssignment abrufen](../api/intune_apps_manageddevicemobileappconfigurationassignment_get.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Objekts.|
|[managedDeviceMobileAppConfigurationAssignment erstellen](../api/intune_apps_manageddevicemobileappconfigurationassignment_create.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Erstellen eines neuen [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Objekts.|
|[managedDeviceMobileAppConfigurationAssignment löschen](../api/intune_apps_manageddevicemobileappconfigurationassignment_delete.md)|Keine|Löscht ein [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Objekt.|
|[managedDeviceMobileAppConfigurationAssignment aktualisieren](../api/intune_apps_manageddevicemobileappconfigurationassignment_update.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner der Entität.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



