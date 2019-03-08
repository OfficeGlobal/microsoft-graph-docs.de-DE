---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Berechtigung
localization_priority: Normal
ms.openlocfilehash: 12390583dcb1a87a5c9492ae3dcbcb132a66f69c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482077"
---
# <a name="permission-resource-type"></a>Berechtigungs Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **Permission** -Ressource enthält Informationen zu einer Freigabeberechtigung, die für eine [driveItem](driveitem.md) -Ressource erteilt wurde.

Freigabeberechtigungen können verschiedene Formen aufweisen.
Die **Permission** -Ressource stellt diese verschiedenen Formulare über Facets für die Ressource dar.

>**Hinweis:** In OneDrive for Business-und SharePoint-Dokumentbibliotheken wird die **geben keine inheritedfrom** -Eigenschaft nicht zurückgegeben.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "grantedToIdentities",
    "invitation",
    "inheritedFrom",
    "shareId",
    "expirationDateTime",
    "hasPassword"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->

```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "grantedToIdentities": [{"@odata.type": "microsoft.graph.identitySet"}],
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string",
  "expirationDateTime": "string (timestamp)",
  "hasPassword": "boolean"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                        | Beschreibung
|:--------------------|:----------------------------|:-------------------------
| id                  | String                      | Die eindeutige ID der Berechtigung für alle Berechtigungen für das Element. Schreibgeschützt.
| grantedTo           | [IdentitySet][]             | Bei Berechtigungen vom Typ „Benutzer“ detaillierte Informationen zu Benutzern und Anwendungen für diese Berechtigung. Schreibgeschützt.
| grantedToIdentities | Sammlung ([identityset][]) | Für Verknüpfungstyp-Berechtigungen die Details der Benutzer, denen die Berechtigung erteilt wurde. Schreibgeschützt.
| invitation          | [SharingInvitation][]       | Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.
| inheritedFrom       | [ItemReference][]           | Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.
| Link                | [SharingLink][]             | Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.
| roles               | Collection(String)          | Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.
| shareId             | String                      | Ein eindeutiges Token, das für den Zugriff auf dieses freigegebene Element über die **[Shares-API][]** verwendet werden kann. Schreibgeschützt.
| expirationDateTime  | DateTimeOffset              | Ein Format von YYYY-MM-ddTHH: mm: ssZ von DateTimeOffset gibt die Ablaufzeit der Berechtigung an. DateTime. MinValue gibt an, dass für diese Berechtigung kein Ablauf Satz festgelegt ist. Optional.
| hasPassword         | Boolesch                     | Dies gibt an, ob für diese Berechtigung ein Kennwort festgelegt ist, es wird nur als Antwort angezeigt. Optional und schreibgeschützt und nur für OneDrive Personal.

### <a name="roles-enumeration-values"></a>Roles-Enumerationswerte

| Wert        | Details                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Ermöglicht das Lesen der Metadaten und Inhalte des Elements.            |
| `write`     | Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements. |
| `sp.owner`  | Für SharePoint und OneDrive for Business stellt dies die Besitzerrolle dar.       |
| `sp.member` | Für SharePoint und OneDrive for Business stellt dies die Mitgliedsrolle dar.      |

Die Permission-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die von Ressource dargestellt wird.

Freigabelinks enthalten ein eindeutiges Token, das für den Zugriff auf das Element erforderlich ist.

Berechtigungen mit einem [**invitation**][SharingInvitation]-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen zum Zugreifen auf die Datei hinzugefügt werden.

## <a name="sharing-links"></a>Freigabelinks

Berechtigungen mit einem [**link**][SharingLink]-Facet stellen Freigabelinks dar, die für das Element erstellt wurden.
Dies sind die häufigsten Arten von Berechtigungen.
Freigabelinks bieten eine eindeutige URL, die für den Zugriff auf eine Datei oder einen Ordner verwendet werden kann.
Sie können so eingerichtet werden, dass Sie Zugriff auf verschiedene Arten gewähren.
Sie können beispielsweise die createLink [][] -API verwenden, um einen Link zu erstellen, der für alle in Ihrer Organisation signierten Personen funktioniert, oder Sie können einen Link erstellen, der für alle Benutzer funktioniert, ohne sich anmelden zu müssen.
Sie können die [invite][] -API verwenden, um einen Link zu erstellen, der nur für bestimmte Personen funktioniert, unabhängig davon, ob Sie sich in Ihrem Unternehmen befinden.

Im folgenden finden Sie einige Beispiele für Freigabelinks.

### <a name="view-link"></a>Link anzeigen

Dieser Ansichts Link bietet schreibgeschützten Zugriff auf alle Benutzer, die über den Link verfügen.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->

```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "scope": "anonymous",
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a>Bearbeitungslink

Dieser Bearbeitungslink bietet Lese-und Schreibzugriff für alle Personen in der Organisation mit dem Link.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->

```json
{
  "id": "2ceefb3g32hh",
  "roles": ["write"],
  "link": {
    "scope": "organization",
    "type": "edit",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/fj277ghautbb422707565gnvg23",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a>Link "spezifische Personen"

Dieser Link bietet Lese-und Schreibzugriff auf die einzelnen Personen in `grantedToIdentities` der Auflistung.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

```json
{
  "id": "3",
  "grantedToIdentities": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName": "Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName": "Judith Clemons"
      }
    }
  ],
  "roles": ["write"],
  "link": {
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/a577ghg9hgh737613bmbjf839026561fmzhsr85ng9f3hjck2t5s",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="sharing-invitations"></a>Freigeben von Einladungen

Berechtigungen, die von der [invite][] -API gesendet werden, enthalten möglicherweise zusätzliche Informationen im Facet der [Einladungs][SharingInvitation] .
Wenn eine Einladung an eine e-Mail-Adresse gesendet wurde, die nicht mit einem bekannten Konto übereinstimmt, wird die **erhält** -Eigenschaft möglicherweise erst festgelegt, wenn der Benutzer zum ersten Mal auf den Link klickt und sich anmeldet.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
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
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a>Methoden

| Methode                                                   | REST-Pfad
|:---------------------------------------------------------|:-----------------------
| [Berechtigungen auflisten](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Berechtigung abrufen](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [Link erstellen] [CreateLink]                                | `POST /drive/items/{item-id}/createLink`
| [Personen einladen] [einladen]                                  | `POST /drive/items/{item-id}/invite`
| [Aktualisieren](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Delete](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[einladen]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[Shares-API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission",
  "suppressions": [
    "Error: /api-reference/beta/resources/permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
