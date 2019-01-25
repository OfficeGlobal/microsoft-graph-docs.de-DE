---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Berechtigung
localization_priority: Normal
ms.openlocfilehash: 6a5a0af9c95900232ff87aa7aedb731a83a91cc5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518849"
---
# <a name="permission-resource-type"></a><span data-ttu-id="a1b5a-102">Permission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1b5a-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1b5a-103">Die **Permission**-Ressource enthält Informationen über eine Berechtigung, die einer [DriveItem](driveitem.md)-Ressource erteilt wurde.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="a1b5a-104">Freigabeberechtigungen können verschiedene Formen aufweisen.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="a1b5a-105">Die **Permission**-Ressource stellt die verschiedenen Formen über Facets für die Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="a1b5a-106">**Hinweis:** OneDrive für Unternehmen und SharePoint-Dokumentbibliotheken keine die **InheritedFrom** -Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1b5a-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1b5a-107">JSON representation</span></span>

<span data-ttu-id="a1b5a-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a1b5a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1b5a-109">Properties</span></span>

| <span data-ttu-id="a1b5a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1b5a-110">Property</span></span>            | <span data-ttu-id="a1b5a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a1b5a-111">Type</span></span>                        | <span data-ttu-id="a1b5a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1b5a-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="a1b5a-113">id</span><span class="sxs-lookup"><span data-stu-id="a1b5a-113">id</span></span>                  | <span data-ttu-id="a1b5a-114">String</span><span class="sxs-lookup"><span data-stu-id="a1b5a-114">String</span></span>                      | <span data-ttu-id="a1b5a-p102">Die eindeutige ID der Berechtigung für alle Berechtigungen für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="a1b5a-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="a1b5a-117">grantedTo</span></span>           | <span data-ttu-id="a1b5a-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="a1b5a-118">[IdentitySet][]</span></span>             | <span data-ttu-id="a1b5a-p103">Bei Berechtigungen vom Typ „Benutzer“ detaillierte Informationen zu Benutzern und Anwendungen für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="a1b5a-121">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="a1b5a-121">grantedToIdentities</span></span> | <span data-ttu-id="a1b5a-122">Auflistung ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="a1b5a-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="a1b5a-123">Link-Typ-Berechtigungen die Details der Benutzer, denen Berechtigung erteilt wurde.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="a1b5a-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-124">Read-only.</span></span>
| <span data-ttu-id="a1b5a-125">invitation</span><span class="sxs-lookup"><span data-stu-id="a1b5a-125">invitation</span></span>          | <span data-ttu-id="a1b5a-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="a1b5a-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="a1b5a-p105">Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="a1b5a-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="a1b5a-129">inheritedFrom</span></span>       | <span data-ttu-id="a1b5a-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="a1b5a-130">[ItemReference][]</span></span>           | <span data-ttu-id="a1b5a-p106">Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="a1b5a-133">Link</span><span class="sxs-lookup"><span data-stu-id="a1b5a-133">link</span></span>                | <span data-ttu-id="a1b5a-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="a1b5a-134">[SharingLink][]</span></span>             | <span data-ttu-id="a1b5a-p107">Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="a1b5a-137">roles</span><span class="sxs-lookup"><span data-stu-id="a1b5a-137">roles</span></span>               | <span data-ttu-id="a1b5a-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a1b5a-138">Collection(String)</span></span>          | <span data-ttu-id="a1b5a-p108">Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="a1b5a-142">shareId</span><span class="sxs-lookup"><span data-stu-id="a1b5a-142">shareId</span></span>             | <span data-ttu-id="a1b5a-143">String</span><span class="sxs-lookup"><span data-stu-id="a1b5a-143">String</span></span>                      | <span data-ttu-id="a1b5a-p109">Ein eindeutiges Token, das verwendet werden kann, um über die \*\* [Freigabe][]-API\*\* auf dieses freigegebene Element zuzugreifen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-p109">A unique token that can be used to access this shared item via the **[shares API][]**. Read-only.</span></span>
| <span data-ttu-id="a1b5a-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a1b5a-146">expirationDateTime</span></span>  | <span data-ttu-id="a1b5a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1b5a-147">DateTimeOffset</span></span>              | <span data-ttu-id="a1b5a-148">Ein Format JJJJ-MM-TTThh von DateTimeOffset gibt den Ablaufzeitpunkt der Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="a1b5a-149">DateTime.MinValue gibt es für diese Berechtigung, kein Ablaufdatum festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="a1b5a-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-150">Optional.</span></span>
| <span data-ttu-id="a1b5a-151">HasPassword</span><span class="sxs-lookup"><span data-stu-id="a1b5a-151">hasPassword</span></span>         | <span data-ttu-id="a1b5a-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1b5a-152">Boolean</span></span>                     | <span data-ttu-id="a1b5a-153">Dies gibt an, ob das Kennwort für diese Berechtigung festgelegt ist, diese nur als Antwort angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="a1b5a-154">Optional und nur-Lese und für OneDrive Personal nur.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="a1b5a-155">Werte des Rollen-enumeration</span><span class="sxs-lookup"><span data-stu-id="a1b5a-155">Roles enumeration values</span></span>

| <span data-ttu-id="a1b5a-156">Wert</span><span class="sxs-lookup"><span data-stu-id="a1b5a-156">Value</span></span>        | <span data-ttu-id="a1b5a-157">Details</span><span class="sxs-lookup"><span data-stu-id="a1b5a-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="a1b5a-158">Ermöglicht das Lesen der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="a1b5a-159">Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="a1b5a-160">Für SharePoint und OneDrive for Business stellt dies die Besitzerrolle dar.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="a1b5a-161">Für SharePoint und OneDrive for Business stellt dies die Mitgliedsrolle dar.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="a1b5a-162">Die Permission-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die von Ressource dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="a1b5a-163">Anwendungsfreigabe Links enthalten ein eindeutiges Token erforderlich, um Zugriff auf das Element.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="a1b5a-164">Berechtigungen mit einem [**invitation**][SharingInvitation]-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen zum Zugreifen auf die Datei hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="a1b5a-165">Freigabelinks</span><span class="sxs-lookup"><span data-stu-id="a1b5a-165">Sharing links</span></span>

<span data-ttu-id="a1b5a-166">Berechtigungen mit einem [**Link**][SharingLink] Facetten darstellen Freigabe von Links, die auf das Element erstellt.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="a1b5a-167">Dies sind die am häufigsten verwendeten Arten von Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="a1b5a-168">Anwendungsfreigabe Links finden Sie eine eindeutige URL, die verwendet werden kann, um eine Datei oder einen Ordner zugreifen.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="a1b5a-169">Sie können Sie so gewähren Sie Zugriff auf verschiedene Arten festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="a1b5a-170">Beispielsweise können [CreateLink][] API zum Erstellen einer Verknüpfung, die für alle Benutzer in Ihrer Organisation angemeldet funktioniert, oder Sie können eine Verknüpfung, die für jeden Benutzer funktioniert, ohne zur Anmeldung bei erstellen.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="a1b5a-171">Die [einladen][] API können Sie erstellen eine Verknüpfung, die nur für bestimmte Personen funktioniert, ob sie in Ihrem Unternehmen oder nicht sind.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="a1b5a-172">Hier sind einige Beispiele für Links freigeben.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="a1b5a-173">Anzeigelink</span><span class="sxs-lookup"><span data-stu-id="a1b5a-173">View link</span></span>

<span data-ttu-id="a1b5a-174">Diese Ansicht Verknüpfung bietet schreibgeschützten Zugriff für alle Benutzer mit den Link.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-174">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="a1b5a-175">Bearbeitungslink</span><span class="sxs-lookup"><span data-stu-id="a1b5a-175">Edit link</span></span>

<span data-ttu-id="a1b5a-176">Dieser Bearbeitungslink bietet Lese- und Schreibzugriff für alle Benutzer in der Organisation mit den Link.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="a1b5a-177">Verknüpfen bestimmte Personen</span><span class="sxs-lookup"><span data-stu-id="a1b5a-177">Specific people link</span></span>

<span data-ttu-id="a1b5a-178">Dieser Link enthält Lese- und Schreibzugriff auf bestimmte Personen in der `grantedToIdentities` Auflistung.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="a1b5a-179">Freigeben von Einladungen</span><span class="sxs-lookup"><span data-stu-id="a1b5a-179">Sharing invitations</span></span>

<span data-ttu-id="a1b5a-180">Berechtigungen, die von der [einladen][] API gesendet möglicherweise zusätzliche Informationen in der [Einladung][SharingInvitation] Facetten.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="a1b5a-181">Wenn Sie eine Einladung an eine e-Mail-Adresse gesendet wurde, der ein bekanntes Konto übereinstimmt, kann die **GrantedTo** -Eigenschaft nicht festgelegt werden, bis die Einladung eingelöst, das beim ersten auftritt, der Benutzer klickt auf die Verknüpfung und sich anmeldet.</span><span class="sxs-lookup"><span data-stu-id="a1b5a-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="a1b5a-182">Nachdem die Freigabeeinladung von einem Benutzer eingelöst wurde, enthält die Eigenschaft **grantedTo** die Informationen über das Konto, das die Berechtigungen eingelöst hat:</span><span class="sxs-lookup"><span data-stu-id="a1b5a-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="a1b5a-183">Methoden</span><span class="sxs-lookup"><span data-stu-id="a1b5a-183">Methods</span></span>

| <span data-ttu-id="a1b5a-184">Methode</span><span class="sxs-lookup"><span data-stu-id="a1b5a-184">Method</span></span>                                                   | <span data-ttu-id="a1b5a-185">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="a1b5a-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="a1b5a-186">Berechtigungen auflisten</span><span class="sxs-lookup"><span data-stu-id="a1b5a-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="a1b5a-187">Get permission</span><span class="sxs-lookup"><span data-stu-id="a1b5a-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="a1b5a-188">[Link erstellen] [createLink]</span><span class="sxs-lookup"><span data-stu-id="a1b5a-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="a1b5a-189">[Einladen von Personen] [einladen]</span><span class="sxs-lookup"><span data-stu-id="a1b5a-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="a1b5a-190">Update</span><span class="sxs-lookup"><span data-stu-id="a1b5a-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="a1b5a-191">Delete</span><span class="sxs-lookup"><span data-stu-id="a1b5a-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[Einladen]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[Freigaben-API]: ../api/shares-get.md
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
