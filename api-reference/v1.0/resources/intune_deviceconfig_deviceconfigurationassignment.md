# <a name="deviceconfigurationassignment-resource-type"></a>deviceConfigurationAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceConfigurationAssignments auflisten](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekte.|
|[deviceConfigurationAssignment abrufen](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekts.|
|[deviceConfigurationAssignment erstellen](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekts.|
|[deviceConfigurationAssignment löschen](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|Keine|Löscht ein [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekt.|
|[deviceConfigurationAssignment aktualisieren](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Zuweisung|
|Ziel|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Das Zuweisungsziel für die Gerätekonfiguration.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








