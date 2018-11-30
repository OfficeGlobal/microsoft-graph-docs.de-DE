---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Berechtigung
ms.openlocfilehash: 195d4840fdb25339eda3858c0bac2395ee9b1c4a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064970"
---
# <a name="permission-resource-type"></a><span data-ttu-id="2f53c-102">Berechtigung Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2f53c-102">permission resource type</span></span>

> <span data-ttu-id="2f53c-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2f53c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f53c-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f53c-105">Die **Berechtigung** Ressource enthält Informationen über eine Zugriffsberechtigung für eine Ressource [DriveItem](driveitem.md) erteilt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="2f53c-106">Freigabeberechtigungen können verschiedene Formen aufweisen.</span><span class="sxs-lookup"><span data-stu-id="2f53c-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="2f53c-107">Die **Berechtigung** Ressource stellt diese verschiedenen Formularen über Facetten für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="2f53c-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="2f53c-108">**Hinweis:** OneDrive für Unternehmen und SharePoint-Dokumentbibliotheken keine die **InheritedFrom** -Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f53c-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f53c-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2f53c-109">JSON representation</span></span>

<span data-ttu-id="2f53c-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2f53c-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2f53c-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2f53c-111">Properties</span></span>

| <span data-ttu-id="2f53c-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f53c-112">Property</span></span>            | <span data-ttu-id="2f53c-113">Typ</span><span class="sxs-lookup"><span data-stu-id="2f53c-113">Type</span></span>                        | <span data-ttu-id="2f53c-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f53c-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="2f53c-115">id</span><span class="sxs-lookup"><span data-stu-id="2f53c-115">id</span></span>                  | <span data-ttu-id="2f53c-116">String</span><span class="sxs-lookup"><span data-stu-id="2f53c-116">String</span></span>                      | <span data-ttu-id="2f53c-p103">Die eindeutige ID der Berechtigung für alle Berechtigungen für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-p103">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="2f53c-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="2f53c-119">grantedTo</span></span>           | <span data-ttu-id="2f53c-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="2f53c-120">[IdentitySet][]</span></span>             | <span data-ttu-id="2f53c-p104">Bei Berechtigungen vom Typ „Benutzer“ detaillierte Informationen zu Benutzern und Anwendungen für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-p104">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="2f53c-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="2f53c-123">grantedToIdentities</span></span> | <span data-ttu-id="2f53c-124">Auflistung ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="2f53c-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="2f53c-125">Link-Typ-Berechtigungen die Details der Benutzer, denen Berechtigung erteilt wurde.</span><span class="sxs-lookup"><span data-stu-id="2f53c-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="2f53c-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-126">Read-only.</span></span>
| <span data-ttu-id="2f53c-127">invitation</span><span class="sxs-lookup"><span data-stu-id="2f53c-127">invitation</span></span>          | <span data-ttu-id="2f53c-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="2f53c-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="2f53c-p106">Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-p106">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="2f53c-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="2f53c-131">inheritedFrom</span></span>       | <span data-ttu-id="2f53c-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="2f53c-132">[ItemReference][]</span></span>           | <span data-ttu-id="2f53c-p107">Stellt einen Verweis auf das Vorgängerelement der aktuellen Berechtigung bereit, wenn es von einem Vorgängerelement geerbt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-p107">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="2f53c-135">Link</span><span class="sxs-lookup"><span data-stu-id="2f53c-135">link</span></span>                | <span data-ttu-id="2f53c-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="2f53c-136">[SharingLink][]</span></span>             | <span data-ttu-id="2f53c-p108">Stellt Linkdetails der aktuellen Berechtigung bereit, wenn es sich um Berechtigungen vom Typ „Link“ handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-p108">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="2f53c-139">roles</span><span class="sxs-lookup"><span data-stu-id="2f53c-139">roles</span></span>               | <span data-ttu-id="2f53c-140">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="2f53c-140">Collection(String)</span></span>          | <span data-ttu-id="2f53c-p109">Die Art der Berechtigung z, B. `read` Nachfolgend finden Sie die vollständige Liste von Rollen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-p109">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="2f53c-144">shareId</span><span class="sxs-lookup"><span data-stu-id="2f53c-144">shareId</span></span>             | <span data-ttu-id="2f53c-145">String</span><span class="sxs-lookup"><span data-stu-id="2f53c-145">String</span></span>                      | <span data-ttu-id="2f53c-146">Ein eindeutiges Token, das Zugriff auf diese über die **[API teilt][]** des freigegebenen Elements verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2f53c-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="2f53c-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-147">Read-only.</span></span>
| <span data-ttu-id="2f53c-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2f53c-148">expirationDateTime</span></span>  | <span data-ttu-id="2f53c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f53c-149">DateTimeOffset</span></span>              | <span data-ttu-id="2f53c-150">Ein Format JJJJ-MM-TTThh von DateTimeOffset gibt den Ablaufzeitpunkt der Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="2f53c-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="2f53c-151">DateTime.MinValue gibt es für diese Berechtigung, kein Ablaufdatum festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="2f53c-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="2f53c-152">Optional.</span><span class="sxs-lookup"><span data-stu-id="2f53c-152">Optional.</span></span>
| <span data-ttu-id="2f53c-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="2f53c-153">hasPassword</span></span>         | <span data-ttu-id="2f53c-154">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2f53c-154">Boolean</span></span>                     | <span data-ttu-id="2f53c-155">Dies gibt an, ob das Kennwort für diese Berechtigung festgelegt ist, diese nur als Antwort angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="2f53c-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="2f53c-156">Optional und nur-Lese und für OneDrive Personal nur.</span><span class="sxs-lookup"><span data-stu-id="2f53c-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="2f53c-157">Werte des Rollen-enumeration</span><span class="sxs-lookup"><span data-stu-id="2f53c-157">Roles enumeration values</span></span>

| <span data-ttu-id="2f53c-158">Wert</span><span class="sxs-lookup"><span data-stu-id="2f53c-158">Value</span></span>        | <span data-ttu-id="2f53c-159">Details</span><span class="sxs-lookup"><span data-stu-id="2f53c-159">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="2f53c-160">Ermöglicht das Lesen der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="2f53c-160">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="2f53c-161">Ermöglicht das Lesen und Ändern der Metadaten und Inhalte des Elements.</span><span class="sxs-lookup"><span data-stu-id="2f53c-161">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="2f53c-162">Für SharePoint und OneDrive for Business stellt dies die Besitzerrolle dar.</span><span class="sxs-lookup"><span data-stu-id="2f53c-162">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="2f53c-163">Für SharePoint und OneDrive for Business stellt dies die Mitgliedsrolle dar.</span><span class="sxs-lookup"><span data-stu-id="2f53c-163">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="2f53c-164">Die Permission-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die von Ressource dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="2f53c-164">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="2f53c-165">Anwendungsfreigabe Links enthalten ein eindeutiges Token erforderlich, um Zugriff auf das Element.</span><span class="sxs-lookup"><span data-stu-id="2f53c-165">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="2f53c-166">Berechtigungen mit einem [**invitation**][SharingInvitation]-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen zum Zugreifen auf die Datei hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="2f53c-166">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="2f53c-167">Freigabelinks</span><span class="sxs-lookup"><span data-stu-id="2f53c-167">Sharing links</span></span>

<span data-ttu-id="2f53c-168">Berechtigungen mit einem [**Link**][SharingLink] Facetten darstellen Freigabe von Links, die auf das Element erstellt.</span><span class="sxs-lookup"><span data-stu-id="2f53c-168">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="2f53c-169">Dies sind die am häufigsten verwendeten Arten von Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="2f53c-169">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="2f53c-170">Anwendungsfreigabe Links finden Sie eine eindeutige URL, die verwendet werden kann, um eine Datei oder einen Ordner zugreifen.</span><span class="sxs-lookup"><span data-stu-id="2f53c-170">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="2f53c-171">Sie können Sie so gewähren Sie Zugriff auf verschiedene Arten festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="2f53c-171">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="2f53c-172">Beispielsweise können [CreateLink][] API zum Erstellen einer Verknüpfung, die für alle Benutzer in Ihrer Organisation angemeldet funktioniert, oder Sie können eine Verknüpfung, die für jeden Benutzer funktioniert, ohne zur Anmeldung bei erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f53c-172">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="2f53c-173">Die [einladen][] API können Sie erstellen eine Verknüpfung, die nur für bestimmte Personen funktioniert, ob sie in Ihrem Unternehmen oder nicht sind.</span><span class="sxs-lookup"><span data-stu-id="2f53c-173">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="2f53c-174">Hier sind einige Beispiele für Links freigeben.</span><span class="sxs-lookup"><span data-stu-id="2f53c-174">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="2f53c-175">Verknüpfung anzeigen</span><span class="sxs-lookup"><span data-stu-id="2f53c-175">View link</span></span>

<span data-ttu-id="2f53c-176">Diese Ansicht Verknüpfung bietet schreibgeschützten Zugriff für alle Benutzer mit den Link.</span><span class="sxs-lookup"><span data-stu-id="2f53c-176">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="2f53c-177">Bearbeitungslink</span><span class="sxs-lookup"><span data-stu-id="2f53c-177">Edit link</span></span>

<span data-ttu-id="2f53c-178">Dieser Bearbeitungslink bietet Lese- und Schreibzugriff für alle Benutzer in der Organisation mit den Link.</span><span class="sxs-lookup"><span data-stu-id="2f53c-178">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="2f53c-179">Verknüpfen bestimmte Personen</span><span class="sxs-lookup"><span data-stu-id="2f53c-179">Specific people link</span></span>

<span data-ttu-id="2f53c-180">Dieser Link enthält Lese- und Schreibzugriff auf bestimmte Personen in der `grantedToIdentities` Auflistung.</span><span class="sxs-lookup"><span data-stu-id="2f53c-180">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="2f53c-181">Freigeben von Einladungen</span><span class="sxs-lookup"><span data-stu-id="2f53c-181">Sharing invitations</span></span>

<span data-ttu-id="2f53c-182">Berechtigungen, die von der [einladen][] API gesendet möglicherweise zusätzliche Informationen in der [Einladung][SharingInvitation] Facetten.</span><span class="sxs-lookup"><span data-stu-id="2f53c-182">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="2f53c-183">Wenn Sie eine Einladung an eine e-Mail-Adresse gesendet wurde, der ein bekanntes Konto übereinstimmt, kann die **GrantedTo** -Eigenschaft nicht festgelegt werden, bis die Einladung eingelöst, das beim ersten auftritt, der Benutzer klickt auf die Verknüpfung und sich anmeldet.</span><span class="sxs-lookup"><span data-stu-id="2f53c-183">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="2f53c-184">Nachdem die Freigabeeinladung von einem Benutzer eingelöst wurde, enthält die Eigenschaft **grantedTo** die Informationen über das Konto, das die Berechtigungen eingelöst hat:</span><span class="sxs-lookup"><span data-stu-id="2f53c-184">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="2f53c-185">Methoden</span><span class="sxs-lookup"><span data-stu-id="2f53c-185">Methods</span></span>

| <span data-ttu-id="2f53c-186">Methode</span><span class="sxs-lookup"><span data-stu-id="2f53c-186">Method</span></span>                                                   | <span data-ttu-id="2f53c-187">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="2f53c-187">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="2f53c-188">Berechtigungen auflisten</span><span class="sxs-lookup"><span data-stu-id="2f53c-188">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="2f53c-189">Get permission</span><span class="sxs-lookup"><span data-stu-id="2f53c-189">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="2f53c-190">[Link erstellen] [createLink]</span><span class="sxs-lookup"><span data-stu-id="2f53c-190">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="2f53c-191">[Einladen von Personen] [einladen]</span><span class="sxs-lookup"><span data-stu-id="2f53c-191">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="2f53c-192">Update</span><span class="sxs-lookup"><span data-stu-id="2f53c-192">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="2f53c-193">Delete</span><span class="sxs-lookup"><span data-stu-id="2f53c-193">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[einladen]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[Freigaben-API]: ../api/shares-get.md
[shares API]: ../api/shares-get.md
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
