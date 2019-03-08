---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Berechtigung
localization_priority: Priority
ms.openlocfilehash: f2781726be786c5eb0d4ed8103dc3b9a62137597
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482224"
---
# <a name="permission-resource-type"></a>Permission-Ressourcentyp

Die **Permission**-Ressource enthält Informationen über eine Berechtigung, die einer [DriveItem](driveitem.md)-Ressource erteilt wurde.

Freigabeberechtigungen können verschiedene Formen aufweisen.
Die **Permission**-Ressource stellt die verschiedenen Formen über Facets für die Ressource dar.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "invitation",
    "inheritedFrom",
    "shareId"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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

| Eigenschaft      | Typ                                      | Beschreibung
|:--------------|:------------------------------------------|:-----------------
| id            | String                                    | Die eindeutige ID der Berechtigung für alle Berechtigungen für das Element. Schreibgeschützt.
| grantedTo     | [IdentitySet](identityset.md)             | Bei Berechtigungen vom Typ „Benutzer“ detaillierte Informationen zu Benutzern und Anwendungen für diese Berechtigung. Schreibgeschützt.
| invitation    | [SharingInvitation][]                     | Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.
| inheritedFrom | [ItemReference](itemreference.md)         | Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.
| Link          | [SharingLink][]                           | Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.
| Rollen         | Collection of String
                      | Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.
| shareId       | String                                    | Ein eindeutiges Token, das verwendet werden kann, um über die [**Freigabe**-API](../api/shares-get.md) auf dieses freigegebene Element zuzugreifen. Schreibgeschützt.

Die Permission-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die von Ressource dargestellt wird.

Berechtigungen mit einem [**link**][SharingLink]-Facet stellen Freigabelinks dar, die für das Element erstellt wurden. Freigabelinks enthalten ein eindeutiges Token, mit dem alle Benutzer, die über den Link verfügen, Zugriff auf das Element haben.

Berechtigungen mit einem [**invitation**][SharingInvitation]-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen zum Zugreifen auf die Datei hinzugefügt werden.

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a>Rollenaufzählung

| Rolle        | Details                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Ermöglicht das Lesen der Metadaten und Inhalte des Elements.            |
| `write`     | Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements. |
| `sp.owner`  | Für SharePoint und OneDrive for Business stellt dies die Besitzerrolle dar.       |
| `sp.member` | Für SharePoint und OneDrive for Business stellt dies die Mitgliedsrolle dar.      |

## <a name="sharing-links"></a>Freigabelinks
Der am häufigsten verwendete Berechtigungstyp sind Freigabelinks. Freigabelinks geben eine eindeutige URL an, die sowohl die freigegebene Ressource als auch ein Authentifizierungstoken enthält, das Zugriff auf die Ressource gewährt. Benutzer müssen sich nicht anmelden, um auf den Inhalt zuzugreifen, der mit einem Freigabelink freigegeben wird. Benutzer können einen Link freigeben, der schreibgeschützten Zugriff oder Schreibzugriff auf den Inhalt ermöglicht.

### <a name="view-link"></a>Anzeigelink
Ein Anzeigelink bietet schreibgeschützten Zugriff auf ein Element.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->
```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="edit-link"></a>Bearbeitungslink
Ein Bearbeitungslink bietet Lese- und Schreibzugriff auf ein Element.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->
```json
{
  "id": "2",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="sharing-invitation"></a>Freigabeeinladung
Außer durch die Erstellung von Freigabelinks können Benutzer auch durch eine E-Mail-Adresse eingeladen werden. In diesem Szenario erstellt die Berechtigung eine Einladung, die an die E-Mail-Adresse des Benutzers gesendet wird.

#### <a name="invitation-to-an-email-address"></a>Einladung an eine E-Mail-Adresse
Wenn die Berechtigung über eine E-Mail-Adresse an einen Empfänger gesendet wurde, der nicht über ein entsprechendes Konto verfügt, kann die Eigenschaft **grantedTo** erst dann festgelegt werden, nachdem die Einladung eingelöst wurde; dies geschieht, wenn ein Benutzer das erste Mal auf den Link klickt und sich anmeldet.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

Nachdem die Freigabeeinladung von einem Benutzer eingelöst wurde, enthält die Eigenschaft **grantedTo** die Informationen über das Konto, das die Berechtigungen eingelöst hat:

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "grantedTo": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "John Doe"
    }
  },
  "invitation": {
    "email": "jd@outlook.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

## <a name="methods"></a>Methoden

| Method                                                   | REST-Pfad
|:---------------------------------------------------------|:-----------------------
| [Berechtigungen auflisten](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Get permission](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [Hinzufügen](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [Update](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Delete](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a>Bemerkungen

OneDrive for Business- und SharePoint-Dokumentbibliotheken geben keine **inheritedFrom**-Eigenschaft zurück.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
