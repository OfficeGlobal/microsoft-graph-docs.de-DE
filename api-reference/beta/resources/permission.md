# <a name="permission-resource-type"></a>Persmission-Ressourcentyp

Die **Permission**-Ressource enthält Informationen über eine Berechtigung, die einer [DriveItem](driveitem.md)-Ressource erteilt wurde.

Berechtigungen können verschiedene Formen aufweisen. Die **Permission**-Ressource stellt die verschiedenen Formen über Facets für die Ressource dar.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "link", "grantedTo", "invitation", "inheritedFrom", "shareId" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ                                      | Beschreibung                                                                                                                           |
|:--------------|:------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------|
| id            | String                                    | Die eindeutige ID der Berechtigung für alle Berechtigungen für das Element. Schreibgeschützt.                                                 |
| grantedTo     | [IdentitySet](identityset.md)             | Bei Berechtigungen vom Typ „Benutzer“ detaillierte Informationen zu Benutzern und Anwendungen für diese Berechtigung. Schreibgeschützt.                                    |
| invitation    | [SharingInvitation](sharinginvitation.md) | Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.                                                          |
| inheritedFrom | [ItemReference](itemreference.md)         | Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.                       |
| Link          | [SharingLink](sharinglink.md)             | Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.                                     |
| role          | Collection of String
                      | Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.                                                 |
| shareId       | String                                    | Ein eindeutiges Token für diese Berechtigung. Schreibgeschützt. |

Die [Permission](../resources/permission.md)-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die die Ressource dargestellt.

Berechtigungen für ein [**link**](sharinglink.md)-Facet stellen Freigabe-Links dar, die für das Element erstellt wurden. Freigabelinks enthalten ein eindeutiges Token, mit dem alle Benutzer, die über den Link verfügen, Zugriff auf das Element haben.

Berechtigungen mit einem [**invitation**](sharinginvitation.md)-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen für Zugriff auf die Datei hinzugefügt werden.

## <a name="roles-enumeration"></a>Rollenaufzählung

| Rolle  | Details                                                                        |
|:------|:-------------------------------------------------------------------------------|
| `read`  | Ermöglicht das Lesen der Metadaten und Inhalte des Elements.            |
| `write` | Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements. |

## <a name="methods"></a>Methoden

| Method                                              | REST-Pfad                            |
|:----------------------------------------------------|:---------------------------------------|
| [List permissions](../api/item_list_permissions.md) | `GET /drive/items/{item-id}/permissions`  |
| [Get permission](../api/permission_get.md)          | `GET /drive/items/{item-id}/permissions/{id}` |
| [Add](../api/item_invite.md)                        | `POST /drive/items/{item-id}/invite` |
| [Update](../api/permission_update.md)               | `PATH /drive/items/{item-id}/permissions/{id}` |
| [Delete](../api/permission_delete.md)               | `DELETE /drive/items/{item-id}/permissions/{id}` |


## <a name="remarks"></a>Bemerkungen

OneDrive for Business- und SharePoint-Dokumentbibliotheken geben keine **inheritedFrom**-Eigenschaft zurück.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
