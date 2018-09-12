# <a name="iosvppebookassignment-resource-type"></a>iosVppEBookAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften zum Zuweisen eines iOS-VPP-E-Books zu einer Gruppe.

Erbt von [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosVppEBookAssignments auflisten](../api/intune_books_iosvppebookassignment_list.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)-Objekte.|
|[iosVppEBookAssignment abrufen](../api/intune_books_iosvppebookassignment_get.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Lesen von Eigenschaften und Beziehungen des [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)-Objekts.|
|[iosVppEBookAssignment erstellen](../api/intune_books_iosvppebookassignment_create.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Erstellen eines neuen [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)-Objekts.|
|[iosVppEBookAssignment löschen](../api/intune_books_iosvppebookassignment_delete.md)|Keine|Löscht ein [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)-Objekt.|
|[iosVppEBookAssignment aktualisieren](../api/intune_books_iosvppebookassignment_update.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Aktualisieren der Eigenschaften eines [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität. Geerbt von [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Zuweisungsziel für das E-Book. Geerbt von [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|Die Installationsabsicht für eBook. Geerbt von [managedEBookAssignment](../resources/intune_books_managedebookassignment.md). Mögliche Werte sind: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedEBookAssignment",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```








