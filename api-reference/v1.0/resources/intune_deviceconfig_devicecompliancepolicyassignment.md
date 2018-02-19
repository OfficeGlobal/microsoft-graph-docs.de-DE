# <a name="devicecompliancepolicyassignment-resource-type"></a>deviceCompliancePolicyAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zuweisung der Gerätekonformitätsrichtlinie.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceCompliancePolicyAssignments auflisten](../api/intune_deviceconfig_devicecompliancepolicyassignment_list.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)-Objekte.|
|[deviceCompliancePolicyAssignment abrufen](../api/intune_deviceconfig_devicecompliancepolicyassignment_get.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Lesen von Eigenschaften und Beziehungen des [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)-Objekts.|
|[deviceCompliancePolicyAssignment erstellen](../api/intune_deviceconfig_devicecompliancepolicyassignment_create.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Erstellen eines neuen [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)-Objekts.|
|[deviceCompliancePolicyAssignment löschen](../api/intune_deviceconfig_devicecompliancepolicyassignment_delete.md)|Keine|Löscht ein [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)-Objekt.|
|[deviceCompliancePolicyAssignment aktualisieren](../api/intune_deviceconfig_devicecompliancepolicyassignment_update.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Aktualisieren der Eigenschaften eines [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_deviceconfig_deviceandappmanagementassignmenttarget.md)|Ziel für die Zuweisung der Compliance-Richtlinie|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



