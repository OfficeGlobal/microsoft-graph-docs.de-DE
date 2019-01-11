---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Berechtigung
localization_priority: Normal
ms.openlocfilehash: 34798437f1bf27c68c390b0f04618985de5cecf3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843316"
---
# <a name="permission-resource-type"></a>Berechtigung Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **Berechtigung** Ressource enthält Informationen über eine Zugriffsberechtigung für eine Ressource [DriveItem](driveitem.md) erteilt.

Freigabeberechtigungen können verschiedene Formen aufweisen.
Die **Berechtigung** Ressource stellt diese verschiedenen Formularen über Facetten für die Ressource.

>**Hinweis:** OneDrive für Unternehmen und SharePoint-Dokumentbibliotheken keine die **InheritedFrom** -Eigenschaft zurückgegeben.

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
| grantedToIdentities | Auflistung ([IdentitySet][]) | Link-Typ-Berechtigungen die Details der Benutzer, denen Berechtigung erteilt wurde. Schreibgeschützt.
| invitation          | [SharingInvitation][]       | Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.
| inheritedFrom       | [ItemReference][]           | Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.
| Link                | [SharingLink][]             | Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.
| roles               | Collection(String)          | Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.
| shareId             | String                      | Ein eindeutiges Token, das Zugriff auf diese über die **[API teilt][]** des freigegebenen Elements verwendet werden können. Schreibgeschützt.
| expirationDateTime  | DateTimeOffset              | Ein Format JJJJ-MM-TTThh von DateTimeOffset gibt den Ablaufzeitpunkt der Berechtigung. DateTime.MinValue gibt es für diese Berechtigung, kein Ablaufdatum festgelegt ist. Optional.
| hasPassword         | Boolean                     | Dies gibt an, ob das Kennwort für diese Berechtigung festgelegt ist, diese nur als Antwort angezeigt wird. Optional und nur-Lese und für OneDrive Personal nur.

### <a name="roles-enumeration-values"></a>Werte des Rollen-enumeration

| Wert        | Details                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Ermöglicht das Lesen der Metadaten und Inhalte des Elements.            |
| `write`     | Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements. |
| `sp.owner`  | Für SharePoint und OneDrive for Business stellt dies die Besitzerrolle dar.       |
| `sp.member` | Für SharePoint und OneDrive for Business stellt dies die Mitgliedsrolle dar.      |

Die Permission-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die von Ressource dargestellt wird.

Anwendungsfreigabe Links enthalten ein eindeutiges Token erforderlich, um Zugriff auf das Element.

Berechtigungen mit einem [**invitation**][SharingInvitation]-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen zum Zugreifen auf die Datei hinzugefügt werden.

## <a name="sharing-links"></a>Freigabelinks

Berechtigungen mit einem [**Link**][SharingLink] Facetten darstellen Freigabe von Links, die auf das Element erstellt.
Dies sind die am häufigsten verwendeten Arten von Berechtigungen.
Anwendungsfreigabe Links finden Sie eine eindeutige URL, die verwendet werden kann, um eine Datei oder einen Ordner zugreifen.
Sie können Sie so gewähren Sie Zugriff auf verschiedene Arten festgelegt werden.
Beispielsweise können [CreateLink][] API zum Erstellen einer Verknüpfung, die für alle Benutzer in Ihrer Organisation angemeldet funktioniert, oder Sie können eine Verknüpfung, die für jeden Benutzer funktioniert, ohne zur Anmeldung bei erstellen.
Die [einladen][] API können Sie erstellen eine Verknüpfung, die nur für bestimmte Personen funktioniert, ob sie in Ihrem Unternehmen oder nicht sind.

Hier sind einige Beispiele für Links freigeben.

### <a name="view-link"></a>Verknüpfung anzeigen

Diese Ansicht Verknüpfung bietet schreibgeschützten Zugriff für alle Benutzer mit den Link.

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

Dieser Bearbeitungslink bietet Lese- und Schreibzugriff für alle Benutzer in der Organisation mit den Link.

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

### <a name="specific-people-link"></a>Verknüpfen bestimmte Personen

Dieser Link enthält Lese- und Schreibzugriff auf bestimmte Personen in der `grantedToIdentities` Auflistung.

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

Berechtigungen, die von der [einladen][] API gesendet möglicherweise zusätzliche Informationen in der [Einladung][SharingInvitation] Facetten.
Wenn Sie eine Einladung an eine e-Mail-Adresse gesendet wurde, der ein bekanntes Konto übereinstimmt, kann die **GrantedTo** -Eigenschaft nicht festgelegt werden, bis die Einladung eingelöst, das beim ersten auftritt, der Benutzer klickt auf die Verknüpfung und sich anmeldet.

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
| [Get permission](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [Link erstellen] [createLink]                                | `POST /drive/items/{item-id}/createLink`
| [Einladen von Personen] [einladen]                                  | `POST /drive/items/{item-id}/invite`
| [Update](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Delete](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[einladen]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[Freigaben-API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
