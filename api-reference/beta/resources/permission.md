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
# <a name="permission-resource-type"></a><span data-ttu-id="dd096-102">Berechtigungs Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dd096-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd096-103">Die **Permission** -Ressource enthält Informationen zu einer Freigabeberechtigung, die für eine [driveItem](driveitem.md) -Ressource erteilt wurde.</span><span class="sxs-lookup"><span data-stu-id="dd096-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="dd096-104">Freigabeberechtigungen können verschiedene Formen aufweisen.</span><span class="sxs-lookup"><span data-stu-id="dd096-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="dd096-105">Die **Permission** -Ressource stellt diese verschiedenen Formulare über Facets für die Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="dd096-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="dd096-106">**Hinweis:** In OneDrive for Business-und SharePoint-Dokumentbibliotheken wird die **geben keine inheritedfrom** -Eigenschaft nicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd096-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd096-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dd096-107">JSON representation</span></span>

<span data-ttu-id="dd096-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dd096-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dd096-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dd096-109">Properties</span></span>

| <span data-ttu-id="dd096-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd096-110">Property</span></span>            | <span data-ttu-id="dd096-111">Typ</span><span class="sxs-lookup"><span data-stu-id="dd096-111">Type</span></span>                        | <span data-ttu-id="dd096-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd096-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="dd096-113">id</span><span class="sxs-lookup"><span data-stu-id="dd096-113">id</span></span>                  | <span data-ttu-id="dd096-114">String</span><span class="sxs-lookup"><span data-stu-id="dd096-114">String</span></span>                      | <span data-ttu-id="dd096-p102">Die eindeutige ID der Berechtigung für alle Berechtigungen für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="dd096-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="dd096-117">grantedTo</span></span>           | <span data-ttu-id="dd096-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="dd096-118">[IdentitySet][]</span></span>             | <span data-ttu-id="dd096-p103">Bei Berechtigungen vom Typ „Benutzer“ detaillierte Informationen zu Benutzern und Anwendungen für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="dd096-121">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="dd096-121">grantedToIdentities</span></span> | <span data-ttu-id="dd096-122">Sammlung ([identityset][])</span><span class="sxs-lookup"><span data-stu-id="dd096-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="dd096-123">Für Verknüpfungstyp-Berechtigungen die Details der Benutzer, denen die Berechtigung erteilt wurde.</span><span class="sxs-lookup"><span data-stu-id="dd096-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="dd096-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-124">Read-only.</span></span>
| <span data-ttu-id="dd096-125">invitation</span><span class="sxs-lookup"><span data-stu-id="dd096-125">invitation</span></span>          | <span data-ttu-id="dd096-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="dd096-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="dd096-p105">Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="dd096-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="dd096-129">inheritedFrom</span></span>       | <span data-ttu-id="dd096-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="dd096-130">[ItemReference][]</span></span>           | <span data-ttu-id="dd096-p106">Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="dd096-133">Link</span><span class="sxs-lookup"><span data-stu-id="dd096-133">link</span></span>                | <span data-ttu-id="dd096-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="dd096-134">[SharingLink][]</span></span>             | <span data-ttu-id="dd096-p107">Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="dd096-137">roles</span><span class="sxs-lookup"><span data-stu-id="dd096-137">roles</span></span>               | <span data-ttu-id="dd096-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="dd096-138">Collection(String)</span></span>          | <span data-ttu-id="dd096-p108">Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="dd096-142">shareId</span><span class="sxs-lookup"><span data-stu-id="dd096-142">shareId</span></span>             | <span data-ttu-id="dd096-143">String</span><span class="sxs-lookup"><span data-stu-id="dd096-143">String</span></span>                      | <span data-ttu-id="dd096-144">Ein eindeutiges Token, das für den Zugriff auf dieses freigegebene Element über die **[Shares-API][]** verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="dd096-144">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="dd096-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd096-145">Read-only.</span></span>
| <span data-ttu-id="dd096-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dd096-146">expirationDateTime</span></span>  | <span data-ttu-id="dd096-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd096-147">DateTimeOffset</span></span>              | <span data-ttu-id="dd096-148">Ein Format von YYYY-MM-ddTHH: mm: ssZ von DateTimeOffset gibt die Ablaufzeit der Berechtigung an.</span><span class="sxs-lookup"><span data-stu-id="dd096-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="dd096-149">DateTime. MinValue gibt an, dass für diese Berechtigung kein Ablauf Satz festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="dd096-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="dd096-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="dd096-150">Optional.</span></span>
| <span data-ttu-id="dd096-151">hasPassword</span><span class="sxs-lookup"><span data-stu-id="dd096-151">hasPassword</span></span>         | <span data-ttu-id="dd096-152">Boolesch</span><span class="sxs-lookup"><span data-stu-id="dd096-152">Boolean</span></span>                     | <span data-ttu-id="dd096-153">Dies gibt an, ob für diese Berechtigung ein Kennwort festgelegt ist, es wird nur als Antwort angezeigt.</span><span class="sxs-lookup"><span data-stu-id="dd096-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="dd096-154">Optional und schreibgeschützt und nur für OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="dd096-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="dd096-155">Roles-Enumerationswerte</span><span class="sxs-lookup"><span data-stu-id="dd096-155">Roles enumeration values</span></span>

| <span data-ttu-id="dd096-156">Wert</span><span class="sxs-lookup"><span data-stu-id="dd096-156">Value</span></span>        | <span data-ttu-id="dd096-157">Details</span><span class="sxs-lookup"><span data-stu-id="dd096-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="dd096-158">Ermöglicht das Lesen der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="dd096-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="dd096-159">Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="dd096-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="dd096-160">Für SharePoint und OneDrive for Business stellt dies die Besitzerrolle dar.</span><span class="sxs-lookup"><span data-stu-id="dd096-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="dd096-161">Für SharePoint und OneDrive for Business stellt dies die Mitgliedsrolle dar.</span><span class="sxs-lookup"><span data-stu-id="dd096-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="dd096-162">Die Permission-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die von Ressource dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="dd096-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="dd096-163">Freigabelinks enthalten ein eindeutiges Token, das für den Zugriff auf das Element erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="dd096-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="dd096-164">Berechtigungen mit einem [**invitation**][SharingInvitation]-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen zum Zugreifen auf die Datei hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="dd096-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="dd096-165">Freigabelinks</span><span class="sxs-lookup"><span data-stu-id="dd096-165">Sharing links</span></span>

<span data-ttu-id="dd096-166">Berechtigungen mit einem [**link**][SharingLink]-Facet stellen Freigabelinks dar, die für das Element erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="dd096-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="dd096-167">Dies sind die häufigsten Arten von Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="dd096-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="dd096-168">Freigabelinks bieten eine eindeutige URL, die für den Zugriff auf eine Datei oder einen Ordner verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="dd096-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="dd096-169">Sie können so eingerichtet werden, dass Sie Zugriff auf verschiedene Arten gewähren.</span><span class="sxs-lookup"><span data-stu-id="dd096-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="dd096-170">Sie können beispielsweise die createLink [][] -API verwenden, um einen Link zu erstellen, der für alle in Ihrer Organisation signierten Personen funktioniert, oder Sie können einen Link erstellen, der für alle Benutzer funktioniert, ohne sich anmelden zu müssen.</span><span class="sxs-lookup"><span data-stu-id="dd096-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="dd096-171">Sie können die [invite][] -API verwenden, um einen Link zu erstellen, der nur für bestimmte Personen funktioniert, unabhängig davon, ob Sie sich in Ihrem Unternehmen befinden.</span><span class="sxs-lookup"><span data-stu-id="dd096-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="dd096-172">Im folgenden finden Sie einige Beispiele für Freigabelinks.</span><span class="sxs-lookup"><span data-stu-id="dd096-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="dd096-173">Link anzeigen</span><span class="sxs-lookup"><span data-stu-id="dd096-173">View link</span></span>

<span data-ttu-id="dd096-174">Dieser Ansichts Link bietet schreibgeschützten Zugriff auf alle Benutzer, die über den Link verfügen.</span><span class="sxs-lookup"><span data-stu-id="dd096-174">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="dd096-175">Bearbeitungslink</span><span class="sxs-lookup"><span data-stu-id="dd096-175">Edit link</span></span>

<span data-ttu-id="dd096-176">Dieser Bearbeitungslink bietet Lese-und Schreibzugriff für alle Personen in der Organisation mit dem Link.</span><span class="sxs-lookup"><span data-stu-id="dd096-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="dd096-177">Link "spezifische Personen"</span><span class="sxs-lookup"><span data-stu-id="dd096-177">Specific people link</span></span>

<span data-ttu-id="dd096-178">Dieser Link bietet Lese-und Schreibzugriff auf die einzelnen Personen in `grantedToIdentities` der Auflistung.</span><span class="sxs-lookup"><span data-stu-id="dd096-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="dd096-179">Freigeben von Einladungen</span><span class="sxs-lookup"><span data-stu-id="dd096-179">Sharing invitations</span></span>

<span data-ttu-id="dd096-180">Berechtigungen, die von der [invite][] -API gesendet werden, enthalten möglicherweise zusätzliche Informationen im Facet der [Einladungs][SharingInvitation] .</span><span class="sxs-lookup"><span data-stu-id="dd096-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="dd096-181">Wenn eine Einladung an eine e-Mail-Adresse gesendet wurde, die nicht mit einem bekannten Konto übereinstimmt, wird die **erhält** -Eigenschaft möglicherweise erst festgelegt, wenn der Benutzer zum ersten Mal auf den Link klickt und sich anmeldet.</span><span class="sxs-lookup"><span data-stu-id="dd096-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="dd096-182">Nachdem die Freigabeeinladung von einem Benutzer eingelöst wurde, enthält die Eigenschaft **grantedTo** die Informationen über das Konto, das die Berechtigungen eingelöst hat:</span><span class="sxs-lookup"><span data-stu-id="dd096-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="dd096-183">Methoden</span><span class="sxs-lookup"><span data-stu-id="dd096-183">Methods</span></span>

| <span data-ttu-id="dd096-184">Methode</span><span class="sxs-lookup"><span data-stu-id="dd096-184">Method</span></span>                                                   | <span data-ttu-id="dd096-185">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="dd096-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="dd096-186">Berechtigungen auflisten</span><span class="sxs-lookup"><span data-stu-id="dd096-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="dd096-187">Berechtigung abrufen</span><span class="sxs-lookup"><span data-stu-id="dd096-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="dd096-188">[Link erstellen] [CreateLink]</span><span class="sxs-lookup"><span data-stu-id="dd096-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="dd096-189">[Personen einladen] [einladen]</span><span class="sxs-lookup"><span data-stu-id="dd096-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="dd096-190">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dd096-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="dd096-191">Delete</span><span class="sxs-lookup"><span data-stu-id="dd096-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[einladen]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[Shares-API]: ../api/shares-get.md
[shares API]: ../api/shares-get.md
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
