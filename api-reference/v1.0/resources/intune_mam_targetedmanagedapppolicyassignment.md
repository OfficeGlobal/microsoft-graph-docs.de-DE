# <a name="targetedmanagedapppolicyassignment-resource-type"></a>targetedManagedAppPolicyAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der Typ der Bereitstellung von Gruppen oder Apps
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[targetedManagedAppPolicyAssignments auflisten](../api/intune_mam_targetedmanagedapppolicyassignment_list.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)-Objekte.|
|[targetedManagedAppPolicyAssignment abrufen](../api/intune_mam_targetedmanagedapppolicyassignment_get.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Lesen von Eigenschaften und Beziehungen des [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)-Objekts.|
|[targetedManagedAppPolicyAssignment löschen](../api/intune_mam_targetedmanagedapppolicyassignment_delete.md)|Keine|Löscht ein [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)-Objekt.|
|[targetedManagedAppPolicyAssignment aktualisieren](../api/intune_mam_targetedmanagedapppolicyassignment_update.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Id|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Bezeichner für die Bereitstellung einer Gruppe oder App|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



