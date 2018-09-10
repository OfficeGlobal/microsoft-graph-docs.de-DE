# <a name="enrollmentconfigurationassignment-resource-type"></a>enrollmentConfigurationAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[enrollmentConfigurationAssignments auflisten](../api/intune_onboarding_enrollmentconfigurationassignment_list.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekte.|
|[enrollmentConfigurationAssignment abrufen](../api/intune_onboarding_enrollmentconfigurationassignment_get.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|Lesen von Eigenschaften und Beziehungen des [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekts.|
|[enrollmentConfigurationAssignment erstellen](../api/intune_onboarding_enrollmentconfigurationassignment_create.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|Erstellen eines neuen [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekts.|
|[enrollmentConfigurationAssignment löschen](../api/intune_onboarding_enrollmentconfigurationassignment_delete.md)|Keine|Löscht ein [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekt.|
|[enrollmentConfigurationAssignment aktualisieren](../api/intune_onboarding_enrollmentconfigurationassignment_update.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|Aktualisieren der Eigenschaften eines [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Noch nicht dokumentiert.|
|Ziel|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Noch nicht dokumentiert.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








