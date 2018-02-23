# <a name="roleassignment-resource-type"></a>roleAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[RoleAssignments auflisten](../api/intune_rbac_roleassignment_list.md)|Sammlung von Objekten des Typs [roleAssignment](../resources/intune_rbac_roleassignment.md)|Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekte.|
|[RoleAssignment abrufen](../api/intune_rbac_roleassignment_get.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekts.|
|[RoleAssignment erstellen](../api/intune_rbac_roleassignment_create.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Erstellen eines neuen [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekts.|
|[RoleAssignment löschen](../api/intune_rbac_roleassignment_delete.md)|Keine|Löscht ein [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekt.|
|[RoleAssignment aktualisieren](../api/intune_rbac_roleassignment_update.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Er ist schreibgeschützt und wird automatisch generiert.|
|displayName|String|Der Anzeigename der Rollenzuweisung.|
|description|String|Beschreibung der Rollenzuweisung.|
|resourceScopes|String-Sammlung|Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.  Dies sind IDs aus Azure Active Directory.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Die Rollendefinition, in der diese Zuweisung enthalten ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



