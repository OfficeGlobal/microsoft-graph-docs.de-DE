---
title: Ressourcentyp directoryRole
description: Stellt eine Azure AD-Directory-Rolle. Azure Active Directory Directory Rollen sind auch bekannt als *Administratorrollen*. Weitere Informationen zu Rollen Verzeichnis (Administrator) finden Sie unter Zuweisen von Administratorrollen in Azure Active Directory. Mit dem Microsoft Graph können Sie Directory Rollen erteilen sie die Berechtigungen der Zielrolle Benutzer zuweisen. Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden. Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert. Zum Aktivieren von anderen verfügbaren Verzeichnis Rollen senden Sie eine POST-Anforderung mit der ID der DirectoryRoleTemplate, auf dem die Rolle Directory basiert. Erbt von directoryObject.
ms.openlocfilehash: 7087befbf18a569defda697e1e2c9eb9d7d34bb9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019290"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="57ceb-110">Ressourcentyp directoryRole</span><span class="sxs-lookup"><span data-stu-id="57ceb-110">directoryRole resource type</span></span>

<span data-ttu-id="57ceb-111">Stellt eine Azure AD-Directory-Rolle.</span><span class="sxs-lookup"><span data-stu-id="57ceb-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="57ceb-112">Azure Active Directory Directory Rollen sind auch bekannt als *Administratorrollen*.</span><span class="sxs-lookup"><span data-stu-id="57ceb-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="57ceb-113">Weitere Informationen zu Rollen Verzeichnis (Administrator) finden Sie unter [Zuweisen von Administratorrollen in Azure Active Directory](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="57ceb-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="57ceb-114">Mit dem Microsoft Graph können Sie Directory Rollen erteilen sie die Berechtigungen der Zielrolle Benutzer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="57ceb-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="57ceb-115">Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="57ceb-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="57ceb-116">Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="57ceb-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="57ceb-117">Zum Aktivieren von anderen verfügbaren Verzeichnis Rollen senden Sie eine POST-Anforderung mit der ID der [DirectoryRoleTemplate](directoryroletemplate.md) , auf dem die Rolle Directory basiert.</span><span class="sxs-lookup"><span data-stu-id="57ceb-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="57ceb-118">Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="57ceb-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="57ceb-119">Diese Ressource unterstützt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="57ceb-119">This resource supports:</span></span>

- <span data-ttu-id="57ceb-120">Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryrole-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="57ceb-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="57ceb-121">Methoden</span><span class="sxs-lookup"><span data-stu-id="57ceb-121">Methods</span></span>

| <span data-ttu-id="57ceb-122">Methode</span><span class="sxs-lookup"><span data-stu-id="57ceb-122">Method</span></span>       | <span data-ttu-id="57ceb-123">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="57ceb-123">Return Type</span></span>  |<span data-ttu-id="57ceb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57ceb-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="57ceb-125">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="57ceb-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="57ceb-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="57ceb-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="57ceb-127">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRole-Objekts.</span><span class="sxs-lookup"><span data-stu-id="57ceb-127">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="57ceb-128">directoryRoles auflisten</span><span class="sxs-lookup"><span data-stu-id="57ceb-128">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="57ceb-129">[directoryRole-Sammlung](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="57ceb-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="57ceb-130">Dient zum Auflisten der Verzeichnisrollen, die im Mandanten aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="57ceb-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="57ceb-131">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="57ceb-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="57ceb-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="57ceb-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="57ceb-133">Fügen Sie der Verzeichnisrolle einen Benutzer durch Veröffentlichen in der Mitgliedernavitionseingenschaft hinzu.</span><span class="sxs-lookup"><span data-stu-id="57ceb-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="57ceb-134">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="57ceb-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="57ceb-135">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="57ceb-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="57ceb-136">Ruft die Benutzer, die Mitglieder der Verzeichnisrolle sind, aus der Mitgliedernavigationseigenschaft ab.</span><span class="sxs-lookup"><span data-stu-id="57ceb-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="57ceb-137">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="57ceb-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="57ceb-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="57ceb-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="57ceb-139">Dient zum Entfernen eines Benutzers aus der Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="57ceb-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="57ceb-140">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="57ceb-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="57ceb-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="57ceb-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="57ceb-142">Dient zum Aktivieren einer Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="57ceb-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="57ceb-143">delta</span><span class="sxs-lookup"><span data-stu-id="57ceb-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="57ceb-144">directoryRole-Sammlung</span><span class="sxs-lookup"><span data-stu-id="57ceb-144">directoryRole collection</span></span>| <span data-ttu-id="57ceb-145">Rufen Sie inkrementelle Änderungen für Directory Rollen.</span><span class="sxs-lookup"><span data-stu-id="57ceb-145">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="57ceb-146">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="57ceb-146">Properties</span></span>
| <span data-ttu-id="57ceb-147">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57ceb-147">Property</span></span>   | <span data-ttu-id="57ceb-148">Typ</span><span class="sxs-lookup"><span data-stu-id="57ceb-148">Type</span></span> | <span data-ttu-id="57ceb-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57ceb-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="57ceb-150">description</span><span class="sxs-lookup"><span data-stu-id="57ceb-150">description</span></span>|<span data-ttu-id="57ceb-151">String</span><span class="sxs-lookup"><span data-stu-id="57ceb-151">String</span></span>|<span data-ttu-id="57ceb-p103">Die Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="57ceb-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="57ceb-154">displayName</span><span class="sxs-lookup"><span data-stu-id="57ceb-154">displayName</span></span>|<span data-ttu-id="57ceb-155">String</span><span class="sxs-lookup"><span data-stu-id="57ceb-155">String</span></span>|<span data-ttu-id="57ceb-p104">Der Anzeigename für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="57ceb-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="57ceb-158">id</span><span class="sxs-lookup"><span data-stu-id="57ceb-158">id</span></span>|<span data-ttu-id="57ceb-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57ceb-159">String</span></span>|<span data-ttu-id="57ceb-p105">Die eindeutige ID für die Verzeichnisrolle. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="57ceb-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="57ceb-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="57ceb-163">roleTemplateId</span></span>|<span data-ttu-id="57ceb-164">String</span><span class="sxs-lookup"><span data-stu-id="57ceb-164">String</span></span>| <span data-ttu-id="57ceb-p106">Die **id** der [directoryRoleTemplate](directoryroletemplate.md), auf der diese Rolle basiert. Die Eigenschaft muss angegeben werden, wenn eine Verzeichnisrolle mit einer POST-Operation in einem Mandanten aktiviert wird. Nach der Aktivierung der Verzeichnisrolle ist die Eigenschaft schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="57ceb-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="57ceb-168">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="57ceb-168">Relationships</span></span>
| <span data-ttu-id="57ceb-169">Beziehung</span><span class="sxs-lookup"><span data-stu-id="57ceb-169">Relationship</span></span> | <span data-ttu-id="57ceb-170">Typ</span><span class="sxs-lookup"><span data-stu-id="57ceb-170">Type</span></span> |<span data-ttu-id="57ceb-171">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57ceb-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57ceb-172">Elemente</span><span class="sxs-lookup"><span data-stu-id="57ceb-172">members</span></span>|<span data-ttu-id="57ceb-173">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="57ceb-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="57ceb-p107">Benutzer, die Mitglieder dieser Verzeichnisrolle sind. HTTP-Methoden: GET, POST, DELETE. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="57ceb-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57ceb-178">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="57ceb-178">JSON representation</span></span>

<span data-ttu-id="57ceb-179">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="57ceb-179">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
