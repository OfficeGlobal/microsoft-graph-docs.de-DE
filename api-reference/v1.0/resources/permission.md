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
# <a name="permission-resource-type"></a><span data-ttu-id="e7d8d-102">Permission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e7d8d-102">Permission resource type</span></span>

<span data-ttu-id="e7d8d-103">Die **Permission**-Ressource enthält Informationen über eine Berechtigung, die einer [DriveItem](driveitem.md)-Ressource erteilt wurde.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-103">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="e7d8d-104">Freigabeberechtigungen können verschiedene Formen aufweisen.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="e7d8d-105">Die **Permission**-Ressource stellt die verschiedenen Formen über Facets für die Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-105">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7d8d-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e7d8d-106">JSON representation</span></span>

<span data-ttu-id="e7d8d-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e7d8d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e7d8d-108">Properties</span></span>

| <span data-ttu-id="e7d8d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7d8d-109">Property</span></span>      | <span data-ttu-id="e7d8d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e7d8d-110">Type</span></span>                                      | <span data-ttu-id="e7d8d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7d8d-111">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="e7d8d-112">id</span><span class="sxs-lookup"><span data-stu-id="e7d8d-112">id</span></span>            | <span data-ttu-id="e7d8d-113">String</span><span class="sxs-lookup"><span data-stu-id="e7d8d-113">String</span></span>                                    | <span data-ttu-id="e7d8d-p102">Die eindeutige ID der Berechtigung für alle Berechtigungen für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="e7d8d-116">grantedTo</span><span class="sxs-lookup"><span data-stu-id="e7d8d-116">grantedTo</span></span>     | [<span data-ttu-id="e7d8d-117">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e7d8d-117">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="e7d8d-p103">Bei Berechtigungen vom Typ „Benutzer“ detaillierte Informationen zu Benutzern und Anwendungen für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="e7d8d-120">invitation</span><span class="sxs-lookup"><span data-stu-id="e7d8d-120">invitation</span></span>    | <span data-ttu-id="e7d8d-121">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="e7d8d-121">[SharingInvitation][]</span></span>                     | <span data-ttu-id="e7d8d-p104">Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p104">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="e7d8d-124">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="e7d8d-124">inheritedFrom</span></span> | [<span data-ttu-id="e7d8d-125">ItemReference</span><span class="sxs-lookup"><span data-stu-id="e7d8d-125">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="e7d8d-p105">Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p105">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="e7d8d-128">Link</span><span class="sxs-lookup"><span data-stu-id="e7d8d-128">link</span></span>          | <span data-ttu-id="e7d8d-129">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="e7d8d-129">[SharingLink][]</span></span>                           | <span data-ttu-id="e7d8d-p106">Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p106">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="e7d8d-132">Rollen</span><span class="sxs-lookup"><span data-stu-id="e7d8d-132">roles</span></span>         | <span data-ttu-id="e7d8d-133">Collection of String
</span><span class="sxs-lookup"><span data-stu-id="e7d8d-133">Collection of String</span></span>                      | <span data-ttu-id="e7d8d-p107">Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p107">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="e7d8d-137">shareId</span><span class="sxs-lookup"><span data-stu-id="e7d8d-137">shareId</span></span>       | <span data-ttu-id="e7d8d-138">String</span><span class="sxs-lookup"><span data-stu-id="e7d8d-138">String</span></span>                                    | <span data-ttu-id="e7d8d-p108">Ein eindeutiges Token, das verwendet werden kann, um über die [**Freigabe**-API](../api/shares-get.md) auf dieses freigegebene Element zuzugreifen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p108">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>

<span data-ttu-id="e7d8d-141">Die Permission-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die von Ressource dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-141">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="e7d8d-p109">Berechtigungen mit einem [**link**][SharingLink]-Facet stellen Freigabelinks dar, die für das Element erstellt wurden. Freigabelinks enthalten ein eindeutiges Token, mit dem alle Benutzer, die über den Link verfügen, Zugriff auf das Element haben.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p109">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="e7d8d-144">Berechtigungen mit einem [**invitation**][SharingInvitation]-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen zum Zugreifen auf die Datei hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-144">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a><span data-ttu-id="e7d8d-147">Rollenaufzählung</span><span class="sxs-lookup"><span data-stu-id="e7d8d-147">Roles enumeration</span></span>

| <span data-ttu-id="e7d8d-148">Rolle</span><span class="sxs-lookup"><span data-stu-id="e7d8d-148">Role</span></span>        | <span data-ttu-id="e7d8d-149">Details</span><span class="sxs-lookup"><span data-stu-id="e7d8d-149">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="e7d8d-150">Ermöglicht das Lesen der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-150">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="e7d8d-151">Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-151">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="e7d8d-152">Für SharePoint und OneDrive for Business stellt dies die Besitzerrolle dar.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-152">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="e7d8d-153">Für SharePoint und OneDrive for Business stellt dies die Mitgliedsrolle dar.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-153">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

## <a name="sharing-links"></a><span data-ttu-id="e7d8d-154">Freigabelinks</span><span class="sxs-lookup"><span data-stu-id="e7d8d-154">Sharing links</span></span>
<span data-ttu-id="e7d8d-p110">Der am häufigsten verwendete Berechtigungstyp sind Freigabelinks. Freigabelinks geben eine eindeutige URL an, die sowohl die freigegebene Ressource als auch ein Authentifizierungstoken enthält, das Zugriff auf die Ressource gewährt. Benutzer müssen sich nicht anmelden, um auf den Inhalt zuzugreifen, der mit einem Freigabelink freigegeben wird. Benutzer können einen Link freigeben, der schreibgeschützten Zugriff oder Schreibzugriff auf den Inhalt ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p110">The most common type of permissions are sharing links. Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource. Users don't need to sign-in to access the content shared with a sharing link. Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="e7d8d-159">Anzeigelink</span><span class="sxs-lookup"><span data-stu-id="e7d8d-159">View Link</span></span>
<span data-ttu-id="e7d8d-160">Ein Anzeigelink bietet schreibgeschützten Zugriff auf ein Element.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-160">A view link provides read-only access to an item.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="e7d8d-161">Bearbeitungslink</span><span class="sxs-lookup"><span data-stu-id="e7d8d-161">Edit link</span></span>
<span data-ttu-id="e7d8d-162">Ein Bearbeitungslink bietet Lese- und Schreibzugriff auf ein Element.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-162">An edit link provides read and write access to an item.</span></span>

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

### <a name="sharing-invitation"></a><span data-ttu-id="e7d8d-163">Freigabeeinladung</span><span class="sxs-lookup"><span data-stu-id="e7d8d-163">Sharing Invitation</span></span>
<span data-ttu-id="e7d8d-p111">Außer durch die Erstellung von Freigabelinks können Benutzer auch durch eine E-Mail-Adresse eingeladen werden. In diesem Szenario erstellt die Berechtigung eine Einladung, die an die E-Mail-Adresse des Benutzers gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-p111">In addition to creating sharing links, a user can be invited by e-mail address. In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="e7d8d-166">Einladung an eine E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="e7d8d-166">Invitation to an email address</span></span>
<span data-ttu-id="e7d8d-167">Wenn die Berechtigung über eine E-Mail-Adresse an einen Empfänger gesendet wurde, der nicht über ein entsprechendes Konto verfügt, kann die Eigenschaft **grantedTo** erst dann festgelegt werden, nachdem die Einladung eingelöst wurde; dies geschieht, wenn ein Benutzer das erste Mal auf den Link klickt und sich anmeldet.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-167">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

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

<span data-ttu-id="e7d8d-168">Nachdem die Freigabeeinladung von einem Benutzer eingelöst wurde, enthält die Eigenschaft **grantedTo** die Informationen über das Konto, das die Berechtigungen eingelöst hat:</span><span class="sxs-lookup"><span data-stu-id="e7d8d-168">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="e7d8d-169">Methoden</span><span class="sxs-lookup"><span data-stu-id="e7d8d-169">Methods</span></span>

| <span data-ttu-id="e7d8d-170">Method</span><span class="sxs-lookup"><span data-stu-id="e7d8d-170">Method</span></span>                                                   | <span data-ttu-id="e7d8d-171">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="e7d8d-171">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="e7d8d-172">Berechtigungen auflisten</span><span class="sxs-lookup"><span data-stu-id="e7d8d-172">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="e7d8d-173">Get permission</span><span class="sxs-lookup"><span data-stu-id="e7d8d-173">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="e7d8d-174">Hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e7d8d-174">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="e7d8d-175">Update</span><span class="sxs-lookup"><span data-stu-id="e7d8d-175">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="e7d8d-176">Delete</span><span class="sxs-lookup"><span data-stu-id="e7d8d-176">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a><span data-ttu-id="e7d8d-177">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="e7d8d-177">Remarks</span></span>

<span data-ttu-id="e7d8d-178">OneDrive for Business- und SharePoint-Dokumentbibliotheken geben keine **inheritedFrom**-Eigenschaft zurück.</span><span class="sxs-lookup"><span data-stu-id="e7d8d-178">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
