# <a name="deviceandappmanagementroledefinition-resource-type"></a>deviceAndAppManagementRoleDefinition-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.

Erbt von [RoleDefinition](../resources/intune_rbac_roledefinition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceAndAppManagementRoleDefinitions auflisten](../api/intune_rbac_deviceandappmanagementroledefinition_list.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekte.|
|[deviceAndAppManagementRoleDefinition abrufen](../api/intune_rbac_deviceandappmanagementroledefinition_get.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekts.|
|[deviceAndAppManagementRoleDefinition erstellen](../api/intune_rbac_deviceandappmanagementroledefinition_create.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekts.|
|[deviceAndAppManagementRoleDefinition löschen](../api/intune_rbac_deviceandappmanagementroledefinition_delete.md)|Keine|Löscht ein [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekt|
|[deviceAndAppManagementRoleDefinition aktualisieren](../api/intune_rbac_deviceandappmanagementroledefinition_update.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Dies ist schreibgeschützt und wird automatisch generiert. Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|displayName|String|Anzeigename der Rollendefinition. Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|description|String|Beschreibung der Rollendefinition. Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|rolePermissions|[rolePermission](../resources/intune_rbac_rolepermission.md)-Sammlung|Liste der Rollenberechtigungen, die diese Rolle ausführen kann. Diese müssen mit dem actionName übereinstimmen, der als Teil der rolePermission definiert ist. Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|isBuiltIn|Boolean|Rollentyp. Wird auf „true“ festgelegt, wenn es sich um eine integrierte, oder auf „false“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt. Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/intune_rbac_roleassignment.md)-Sammlung|Liste von Rollenzuweisungen für diese Rollendefinition. Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```


