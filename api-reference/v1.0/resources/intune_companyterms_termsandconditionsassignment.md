# <a name="termsandconditionsassignment-resource-type"></a>termsAndConditionsAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[termsAndConditionsAssignments auflisten](../api/intune_companyterms_termsandconditionsassignment_list.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekte.|
|[termsAndConditionsAssignment abrufen](../api/intune_companyterms_termsandconditionsassignment_get.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekts.|
|[termsAndConditionsAssignment erstellen](../api/intune_companyterms_termsandconditionsassignment_create.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekts.|
|[termsAndConditionsAssignment löschen](../api/intune_companyterms_termsandconditionsassignment_delete.md)|Keine|Löscht ein [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[termsAndConditionsAssignment aktualisieren](../api/intune_companyterms_termsandconditionsassignment_update.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner der Entität.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_companyterms_deviceandappmanagementassignmenttarget.md)|Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



