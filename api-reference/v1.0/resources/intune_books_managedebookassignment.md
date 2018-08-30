# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften zum Zuweisen eines E-Books zu einer Gruppe.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedEBookAssignments auflisten](../api/intune_books_managedebookassignment_list.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Objekte.|
|[managedEBookAssignment abrufen](../api/intune_books_managedebookassignment_get.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Lesen von Eigenschaften und Beziehungen des [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Objekts.|
|[managedEBookAssignment erstellen](../api/intune_books_managedebookassignment_create.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Erstellen eines neuen [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Objekts.|
|[managedEBookAssignment löschen](../api/intune_books_managedebookassignment_delete.md)|Keine|Löscht ein [ManagedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Objekt.|
|[managedEBookAssignment aktualisieren](../api/intune_books_managedebookassignment_update.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Aktualisieren der Eigenschaften eines [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|Ziel|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Zuweisungsziel für das E-Book|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|Installationspriorität für das E-Book. Mögliche Werte: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



