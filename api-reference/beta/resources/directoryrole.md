---
title: Ressourcentyp directoryRole
description: Stellt eine Azure AD-Verzeichnisrolle dar. Azure AD-Verzeichnisrollen werden auch als *Administratorrollen* bezeichnet. Weitere Informationen zu diesen Verzeichnis-(Administrator)Rollen finden Sie unter Zuweisen von Administratorrollen in Azure AD. Mit Microsoft Graph können Sie Benutzer zu Verzeichnisrollen zuweisen, um ihnen Berechtigungen der Zielrolle zuzuweisen. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zum Aktivieren anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung mit der ID der directoryRoleTemplate, auf der die Verzeichnisrolle basiert. Erbt von directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521250"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="20506-110">Ressourcentyp directoryRole</span><span class="sxs-lookup"><span data-stu-id="20506-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20506-p102">Stellt eine Azure AD-Verzeichnisrolle dar. Azure AD-Verzeichnisrollen werden auch als *Administratorrollen* bezeichnet. Weitere Informationen zu diesen Verzeichnis-(Administrator)Rollen finden Sie unter [Zuweisen von Administratorrollen in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Mit Microsoft Graph können Sie Benutzer zu Verzeichnisrollen zuweisen, um ihnen Berechtigungen der Zielrolle zuzuweisen. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zum Aktivieren anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung mit der ID der [directoryRoleTemplate](directoryroletemplate.md), auf der die Verzeichnisrolle basiert. Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="20506-p102">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="20506-119">Standardmäßig werden Directory Rollen Recherchediensts Mandanten geltende sein.</span><span class="sxs-lookup"><span data-stu-id="20506-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="20506-120">Verzeichnis Rollen (derzeit nur das *Konto ein Benutzeradministrator* und *Helpdesk Admin*) können jedoch auch [administrative Einheiten](administrativeunit.md)zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="20506-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="20506-121">Diese Ressource unterstützt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="20506-121">This resource supports:</span></span>

- <span data-ttu-id="20506-122">Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryrole-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="20506-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="20506-123">Methoden</span><span class="sxs-lookup"><span data-stu-id="20506-123">Methods</span></span>

| <span data-ttu-id="20506-124">Methode</span><span class="sxs-lookup"><span data-stu-id="20506-124">Method</span></span>       | <span data-ttu-id="20506-125">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="20506-125">Return Type</span></span>  |<span data-ttu-id="20506-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20506-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20506-127">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="20506-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="20506-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="20506-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="20506-129">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRole-Objekts.</span><span class="sxs-lookup"><span data-stu-id="20506-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="20506-130">directoryRoles auflisten</span><span class="sxs-lookup"><span data-stu-id="20506-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="20506-131">[directoryRole-Sammlung](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="20506-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="20506-132">Dient zum Auflisten der Verzeichnisrollen, die im Mandanten aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="20506-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="20506-133">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="20506-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="20506-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="20506-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="20506-135">Fügen Sie der Verzeichnisrolle einen Benutzer durch Veröffentlichen in der Mitgliedernavitionseingenschaft hinzu.</span><span class="sxs-lookup"><span data-stu-id="20506-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="20506-136">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="20506-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="20506-137">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="20506-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="20506-138">Ruft die Benutzer, die Mitglieder der Verzeichnisrolle sind, aus der Mitgliedernavigationseigenschaft ab.</span><span class="sxs-lookup"><span data-stu-id="20506-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="20506-139">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="20506-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="20506-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="20506-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="20506-141">Dient zum Entfernen eines Benutzers aus der Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="20506-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="20506-142">Mitglieder der Liste bezogenen-Rolle</span><span class="sxs-lookup"><span data-stu-id="20506-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="20506-143">scopedRoleMembership-Sammlung</span><span class="sxs-lookup"><span data-stu-id="20506-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="20506-144">Die Elemente dieser Rolle Verzeichnis, die [administrative Einheiten](administrativeunit.md)mithilfe der Auflistung der ScopedRoleMembership Ressource zugeordnet werden aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="20506-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="20506-145">delta</span><span class="sxs-lookup"><span data-stu-id="20506-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="20506-146">directoryRole-Sammlung</span><span class="sxs-lookup"><span data-stu-id="20506-146">directoryRole collection</span></span>| <span data-ttu-id="20506-147">Rufen Sie inkrementelle Änderungen für Directory Rollen.</span><span class="sxs-lookup"><span data-stu-id="20506-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="20506-148">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20506-148">Properties</span></span>
| <span data-ttu-id="20506-149">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20506-149">Property</span></span>   | <span data-ttu-id="20506-150">Typ</span><span class="sxs-lookup"><span data-stu-id="20506-150">Type</span></span> |<span data-ttu-id="20506-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20506-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20506-152">description</span><span class="sxs-lookup"><span data-stu-id="20506-152">description</span></span>|<span data-ttu-id="20506-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20506-153">String</span></span>|<span data-ttu-id="20506-p104">Die Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="20506-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="20506-156">displayName</span><span class="sxs-lookup"><span data-stu-id="20506-156">displayName</span></span>|<span data-ttu-id="20506-157">String</span><span class="sxs-lookup"><span data-stu-id="20506-157">String</span></span>|<span data-ttu-id="20506-p105">Der Anzeigename für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="20506-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="20506-160">id</span><span class="sxs-lookup"><span data-stu-id="20506-160">id</span></span>|<span data-ttu-id="20506-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20506-161">String</span></span>|<span data-ttu-id="20506-p106">Die eindeutige ID für die Verzeichnisrolle. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="20506-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="20506-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="20506-165">roleTemplateId</span></span>|<span data-ttu-id="20506-166">String</span><span class="sxs-lookup"><span data-stu-id="20506-166">String</span></span>| <span data-ttu-id="20506-p107">Die **id** der [directoryRoleTemplate](directoryroletemplate.md), auf der diese Rolle basiert. Die Eigenschaft muss angegeben werden, wenn eine Verzeichnisrolle mit einer POST-Operation in einem Mandanten aktiviert wird. Nach der Aktivierung der Verzeichnisrolle ist die Eigenschaft schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="20506-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="20506-170">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="20506-170">Relationships</span></span>
| <span data-ttu-id="20506-171">Beziehung</span><span class="sxs-lookup"><span data-stu-id="20506-171">Relationship</span></span> | <span data-ttu-id="20506-172">Typ</span><span class="sxs-lookup"><span data-stu-id="20506-172">Type</span></span> |<span data-ttu-id="20506-173">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20506-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20506-174">members</span><span class="sxs-lookup"><span data-stu-id="20506-174">members</span></span>|<span data-ttu-id="20506-175">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="20506-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="20506-p108">Benutzer, die Mitglieder dieser Verzeichnisrolle sind. HTTP-Methoden: GET, POST, DELETE. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="20506-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="20506-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="20506-180">scopedMembers</span></span>|<span data-ttu-id="20506-181">scopedRoleMembership-Sammlung</span><span class="sxs-lookup"><span data-stu-id="20506-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="20506-182">Mitglieder dieser Rolle Directory [administrative Einheiten](administrativeunit.md)zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="20506-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="20506-183">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="20506-183">Read-only.</span></span> <span data-ttu-id="20506-184">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="20506-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20506-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20506-185">JSON representation</span></span>

<span data-ttu-id="20506-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20506-186">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
