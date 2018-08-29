# <a name="directoryrole-resource-type"></a><span data-ttu-id="fc173-101">Ressourcentyp directoryRole</span><span class="sxs-lookup"><span data-stu-id="fc173-101">directoryRole resource type</span></span>

<span data-ttu-id="fc173-p101">Stellt eine Azure AD-Verzeichnisrolle dar. Azure AD-Verzeichnisrollen werden auch als *Administratorrollen* bezeichnet. Weitere Informationen zu diesen Verzeichnis-(Administrator)Rollen finden Sie unter [Zuweisen von Administratorrollen in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Mit Microsoft Graph können Sie Benutzer zu Verzeichnisrollen zuweisen, um ihnen Berechtigungen der Zielrolle zuzuweisen. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zum Aktivieren anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung mit der ID der [directoryRoleTemplate](directoryroletemplate.md), auf der die Verzeichnisrolle basiert. Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="fc173-p101">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fc173-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="fc173-110">Methods</span></span>

| <span data-ttu-id="fc173-111">Methode</span><span class="sxs-lookup"><span data-stu-id="fc173-111">Method</span></span>       | <span data-ttu-id="fc173-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fc173-112">Return Type</span></span>  |<span data-ttu-id="fc173-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc173-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc173-114">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="fc173-114">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="fc173-115">directoryRole</span><span class="sxs-lookup"><span data-stu-id="fc173-115">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="fc173-116">Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRole-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc173-116">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="fc173-117">directoryRoles auflisten</span><span class="sxs-lookup"><span data-stu-id="fc173-117">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="fc173-118">[directoryRole-Sammlung](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="fc173-118">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="fc173-119">Dient zum Auflisten der Verzeichnisrollen, die im Mandanten aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="fc173-119">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="fc173-120">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="fc173-120">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="fc173-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc173-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="fc173-122">Fügen Sie der Verzeichnisrolle einen Benutzer durch Veröffentlichen in der Mitgliedernavitionseingenschaft hinzu.</span><span class="sxs-lookup"><span data-stu-id="fc173-122">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="fc173-123">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="fc173-123">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="fc173-124">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fc173-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="fc173-125">Ruft die Benutzer, die Mitglieder der Verzeichnisrolle sind, aus der Mitgliedernavigationseigenschaft ab.</span><span class="sxs-lookup"><span data-stu-id="fc173-125">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="fc173-126">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="fc173-126">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="fc173-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc173-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="fc173-128">Dient zum Entfernen eines Benutzers aus der Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="fc173-128">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="fc173-129">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="fc173-129">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="fc173-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="fc173-130">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="fc173-131">Dient zum Aktivieren einer Verzeichnisrolle.</span><span class="sxs-lookup"><span data-stu-id="fc173-131">Activate a directory role.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc173-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fc173-132">Properties</span></span>
| <span data-ttu-id="fc173-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc173-133">Property</span></span>   | <span data-ttu-id="fc173-134">Typ</span><span class="sxs-lookup"><span data-stu-id="fc173-134">Type</span></span> | <span data-ttu-id="fc173-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc173-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fc173-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc173-136">description</span></span>|<span data-ttu-id="fc173-137">String</span><span class="sxs-lookup"><span data-stu-id="fc173-137">String</span></span>|<span data-ttu-id="fc173-p102">Die Beschreibung für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc173-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="fc173-140">displayName</span><span class="sxs-lookup"><span data-stu-id="fc173-140">displayName</span></span>|<span data-ttu-id="fc173-141">String</span><span class="sxs-lookup"><span data-stu-id="fc173-141">String</span></span>|<span data-ttu-id="fc173-p103">Der Anzeigename für die Verzeichnisrolle. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc173-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="fc173-144">id</span><span class="sxs-lookup"><span data-stu-id="fc173-144">id</span></span>|<span data-ttu-id="fc173-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc173-145">String</span></span>|<span data-ttu-id="fc173-p104">Die eindeutige ID für die Verzeichnisrolle. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc173-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="fc173-149">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="fc173-149">roleTemplateId</span></span>|<span data-ttu-id="fc173-150">String</span><span class="sxs-lookup"><span data-stu-id="fc173-150">String</span></span>| <span data-ttu-id="fc173-p105">Die **id** der [directoryRoleTemplate](directoryroletemplate.md), auf der diese Rolle basiert. Die Eigenschaft muss angegeben werden, wenn eine Verzeichnisrolle mit einer POST-Operation in einem Mandanten aktiviert wird. Nach der Aktivierung der Verzeichnisrolle ist die Eigenschaft schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc173-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fc173-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fc173-154">Relationships</span></span>
| <span data-ttu-id="fc173-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fc173-155">Relationship</span></span> | <span data-ttu-id="fc173-156">Typ</span><span class="sxs-lookup"><span data-stu-id="fc173-156">Type</span></span> |<span data-ttu-id="fc173-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc173-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc173-158">Elemente</span><span class="sxs-lookup"><span data-stu-id="fc173-158">members</span></span>|<span data-ttu-id="fc173-159">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fc173-159">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="fc173-p106">Benutzer, die Mitglieder dieser Verzeichnisrolle sind. HTTP-Methoden: GET, POST, DELETE. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="fc173-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc173-164">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fc173-164">JSON representation</span></span>

<span data-ttu-id="fc173-165">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fc173-165">Here is a JSON representation of the resource</span></span>

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
