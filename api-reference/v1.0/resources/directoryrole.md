# <a name="directoryrole-resource-type"></a><span data-ttu-id="0297f-101">Ressourcentyp directoryRole</span><span class="sxs-lookup"><span data-stu-id="0297f-101">directoryRole resource type</span></span>

<span data-ttu-id="0297f-102">Stellt eine Azure AD-Directory-Rolle.</span><span class="sxs-lookup"><span data-stu-id="0297f-102">Represents an Azure AD directory role.</span></span> <span data-ttu-id="0297f-103">Azure Active Directory Directory Rollen sind auch bekannt als *Administratorrollen*.</span><span class="sxs-lookup"><span data-stu-id="0297f-103">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="0297f-104">Weitere Informationen zu Rollen Verzeichnis (Administrator) finden Sie unter [Zuweisen von Administratorrollen in Azure Active Directory](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="0297f-104">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="0297f-105">Mit dem Microsoft Graph können Sie Directory Rollen erteilen sie die Berechtigungen der Zielrolle Benutzer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="0297f-105">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="0297f-106">Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="0297f-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="0297f-107">Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="0297f-107">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="0297f-108">Zum Aktivieren von anderen verfügbaren Verzeichnis Rollen senden Sie eine POST-Anforderung mit der ID der [DirectoryRoleTemplate](directoryroletemplate.md) , auf dem die Rolle Directory basiert.</span><span class="sxs-lookup"><span data-stu-id="0297f-108">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="0297f-109">Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="0297f-109">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="0297f-110">Diese Ressource unterstützt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="0297f-110">This resource supports:</span></span>

- <span data-ttu-id="0297f-111">Verwenden einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryrole_delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="0297f-111">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="0297f-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="0297f-112">Methods</span></span>

| <span data-ttu-id="0297f-113">Methode</span><span class="sxs-lookup"><span data-stu-id="0297f-113">Method</span></span>       | <span data-ttu-id="0297f-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0297f-114">Return Type</span></span>  |<span data-ttu-id="0297f-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0297f-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0297f-116">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="0297f-116">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="0297f-117">directoryRole</span><span class="sxs-lookup"><span data-stu-id="0297f-117">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="0297f-118">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRole-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0297f-118">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="0297f-119">directoryRoles auflisten</span><span class="sxs-lookup"><span data-stu-id="0297f-119">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="0297f-120">[directoryRole-Sammlung](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="0297f-120">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="0297f-121">Dient zum Auflisten der Verzeichnisrollen, die im Mandanten aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="0297f-121">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="0297f-122">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0297f-122">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="0297f-123">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0297f-123">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="0297f-124">Fügen Sie der Verzeichnisrolle einen Benutzer durch Veröffentlichen in der Mitgliedernavitionseingenschaft hinzu.</span><span class="sxs-lookup"><span data-stu-id="0297f-124">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="0297f-125">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="0297f-125">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="0297f-126">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0297f-126">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="0297f-127">Ruft die Benutzer, die Mitglieder der Verzeichnisrolle sind, aus der Mitgliedernavigationseigenschaft ab.</span><span class="sxs-lookup"><span data-stu-id="0297f-127">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="0297f-128">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="0297f-128">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="0297f-129">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0297f-129">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="0297f-130">Dient zum Entfernen eines Benutzers aus der Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="0297f-130">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="0297f-131">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="0297f-131">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="0297f-132">directoryRole</span><span class="sxs-lookup"><span data-stu-id="0297f-132">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="0297f-133">Dient zum Aktivieren einer Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="0297f-133">Activate a directory role.</span></span>|
|[<span data-ttu-id="0297f-134">delta</span><span class="sxs-lookup"><span data-stu-id="0297f-134">delta</span></span>](../api/directoryrole_delta.md)|<span data-ttu-id="0297f-135">directoryRole-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0297f-135">directoryRole collection</span></span>| <span data-ttu-id="0297f-136">Rufen Sie inkrementelle Änderungen für Directory Rollen.</span><span class="sxs-lookup"><span data-stu-id="0297f-136">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="0297f-137">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0297f-137">Properties</span></span>
| <span data-ttu-id="0297f-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0297f-138">Property</span></span>   | <span data-ttu-id="0297f-139">Typ</span><span class="sxs-lookup"><span data-stu-id="0297f-139">Type</span></span> | <span data-ttu-id="0297f-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0297f-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0297f-141">description</span><span class="sxs-lookup"><span data-stu-id="0297f-141">description</span></span>|<span data-ttu-id="0297f-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0297f-142">String</span></span>|<span data-ttu-id="0297f-p102">Die Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0297f-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="0297f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0297f-145">displayName</span></span>|<span data-ttu-id="0297f-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0297f-146">String</span></span>|<span data-ttu-id="0297f-p103">Der Anzeigename für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0297f-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="0297f-149">id</span><span class="sxs-lookup"><span data-stu-id="0297f-149">id</span></span>|<span data-ttu-id="0297f-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0297f-150">String</span></span>|<span data-ttu-id="0297f-p104">Die eindeutige ID für die Verzeichnisrolle. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0297f-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="0297f-154">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="0297f-154">roleTemplateId</span></span>|<span data-ttu-id="0297f-155">String</span><span class="sxs-lookup"><span data-stu-id="0297f-155">String</span></span>| <span data-ttu-id="0297f-p105">Die **id** der [directoryRoleTemplate](directoryroletemplate.md), auf der diese Rolle basiert. Die Eigenschaft muss angegeben werden, wenn eine Verzeichnisrolle mit einer POST-Operation in einem Mandanten aktiviert wird. Nach der Aktivierung der Verzeichnisrolle ist die Eigenschaft schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0297f-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0297f-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0297f-159">Relationships</span></span>
| <span data-ttu-id="0297f-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0297f-160">Relationship</span></span> | <span data-ttu-id="0297f-161">Typ</span><span class="sxs-lookup"><span data-stu-id="0297f-161">Type</span></span> |<span data-ttu-id="0297f-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0297f-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0297f-163">Elemente</span><span class="sxs-lookup"><span data-stu-id="0297f-163">members</span></span>|<span data-ttu-id="0297f-164">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0297f-164">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="0297f-p106">Benutzer, die Mitglieder dieser Verzeichnisrolle sind. HTTP-Methoden: GET, POST, DELETE. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0297f-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0297f-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0297f-169">JSON representation</span></span>

<span data-ttu-id="0297f-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0297f-170">Here is a JSON representation of the resource</span></span>

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
