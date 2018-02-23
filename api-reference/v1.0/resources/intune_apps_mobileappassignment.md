# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Klasse, die die Eigenschaften für die Gruppenzuordnung einer mobilen App enthält.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[mobileAppAssignments auflisten](../api/intune_apps_mobileappassignment_list.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Objekte.|
|[mobileAppAssignment abrufen](../api/intune_apps_mobileappassignment_get.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Objekts.|
|[mobileAppAssignment erstellen](../api/intune_apps_mobileappassignment_create.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Erstellen eines neuen [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Objekts.|
|[mobileAppAssignment löschen](../api/intune_apps_mobileappassignment_delete.md)|Keine|Löschen einer [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[mobileAppAssignment aktualisieren](../api/intune_apps_mobileappassignment_update.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Aktualisieren der Eigenschaften eines [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|Priorität|Zeichenfolge|Die vom Administrator definierte Installationspriorität. Mögliche Werte: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|Ziel|[deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|Die vom Administrator definierte Zielgruppenzuordnung.|
|Einstellungen|[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)|Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



