# <a name="roledefinition-resource-type"></a>Ressourcentyp „roleDefinition“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Hierbei handelt es sich um die Ressource für Rollendefinitionen. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. Eine Rolle kombiniert eine Intune-Ressource wie beispielsweise eine mobile App mit den zur Rolle gehörenden Rollenberechtigungen, beispielsweise „Erstellen“ oder „Lesen“. Es gibt zwei Arten von Rollen: integrierte Rollen und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Sowohl integrierte Rollen als auch benutzerdefinierte Rollen werden nur durchgesetzt, wenn Zuweisungen vorhanden sind. Erstellen Sie eine benutzerdefinierte Rolle, wenn Sie eine Rolle definieren möchten, die beliebige der verfügbaren Ressourcen und Rollenberechtigungen in einer einzigen Rolle zusammenfasst.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „roleDefinition“](../api/intune_rbac_roledefinition_list.md)|Sammlung von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md) auf.|
|[Abrufen von „roleDefinition“](../api/intune_rbac_roledefinition_get.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Erstellen von „roleDefinition“](../api/intune_rbac_roledefinition_create.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Erstellt neue Objekte des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Löschen von „roleDefinition“](../api/intune_rbac_roledefinition_delete.md)|Keiner|Löscht Objekte des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Aktualisieren von „roleDefinition“](../api/intune_rbac_roledefinition_update.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Er ist schreibgeschützt und wird automatisch generiert.|
|displayName|String|Anzeigename der Rollendefinition|
|description|String|Beschreibung der Rollendefinition|
|rolePermissions|Sammlung von Objekten des Typs [rolePermission](../resources/intune_rbac_rolepermission.md)|Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden. Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.|
|isBuiltIn|Boolean|Rollentyp. Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|roleAssignments|Sammlung von Objekten des Typs [roleAssignment](../resources/intune_rbac_roleassignment.md)|Liste der Rollenzuweisungen für die Rollendefinition|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
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



