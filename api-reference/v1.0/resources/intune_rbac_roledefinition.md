# <a name="roledefinition-resource-type"></a><span data-ttu-id="8dc6f-101">Ressourcentyp „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="8dc6f-101">roleDefinition resource type</span></span>

> <span data-ttu-id="8dc6f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8dc6f-103">Hierbei handelt es sich um die Ressource für Rollendefinitionen.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-103">The Role Definition resource.</span></span> <span data-ttu-id="8dc6f-104">Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-104">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="8dc6f-105">Eine Rolle kombiniert eine Intune-Ressource wie beispielsweise eine mobile App mit den zur Rolle gehörenden Rollenberechtigungen, beispielsweise „Erstellen“ oder „Lesen“.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-105">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="8dc6f-106">Es gibt zwei Arten von Rollen: integrierte Rollen und benutzerdefinierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-106">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="8dc6f-107">Integrierte Rollen können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-107">Built-in roles cannot be modified.</span></span> <span data-ttu-id="8dc6f-108">Sowohl integrierte Rollen als auch benutzerdefinierte Rollen werden nur durchgesetzt, wenn Zuweisungen vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-108">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="8dc6f-109">Erstellen Sie eine benutzerdefinierte Rolle, wenn Sie eine Rolle definieren möchten, die beliebige der verfügbaren Ressourcen und Rollenberechtigungen in einer einzigen Rolle zusammenfasst.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-109">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="8dc6f-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="8dc6f-110">Methods</span></span>
|<span data-ttu-id="8dc6f-111">Methode</span><span class="sxs-lookup"><span data-stu-id="8dc6f-111">Method</span></span>|<span data-ttu-id="8dc6f-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8dc6f-112">Return Type</span></span>|<span data-ttu-id="8dc6f-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dc6f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8dc6f-114">Auflisten von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="8dc6f-114">List roleDefinitions</span></span>](../api/intune_rbac_roledefinition_list.md)|<span data-ttu-id="8dc6f-115">Sammlung von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8dc6f-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="8dc6f-116">Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md) auf.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-116">List properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="8dc6f-117">Abrufen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="8dc6f-117">Get roleDefinition</span></span>](../api/intune_rbac_roledefinition_get.md)|[<span data-ttu-id="8dc6f-118">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8dc6f-118">RoleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="8dc6f-119">Liest die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8dc6f-119">Read properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="8dc6f-120">Erstellen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="8dc6f-120">Create roleDefinition</span></span>](../api/intune_rbac_roledefinition_create.md)|[<span data-ttu-id="8dc6f-121">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8dc6f-121">RoleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="8dc6f-122">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8dc6f-122">Create a new [plannerBucket](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="8dc6f-123">Löschen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="8dc6f-123">Delete roleDefinition</span></span>](../api/intune_rbac_roledefinition_delete.md)|<span data-ttu-id="8dc6f-124">Keiner</span><span class="sxs-lookup"><span data-stu-id="8dc6f-124">None</span></span>|<span data-ttu-id="8dc6f-125">Löscht Objekte des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8dc6f-125">Deletes a [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>|
|[<span data-ttu-id="8dc6f-126">Aktualisieren von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="8dc6f-126">Update roleDefinition</span></span>](../api/intune_rbac_roledefinition_update.md)|[<span data-ttu-id="8dc6f-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8dc6f-127">RoleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="8dc6f-128">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8dc6f-128">Update the properties of a [calendar](../resources/intune_rbac_roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8dc6f-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8dc6f-129">Properties</span></span>
|<span data-ttu-id="8dc6f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8dc6f-130">Property</span></span>|<span data-ttu-id="8dc6f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8dc6f-131">Type</span></span>|<span data-ttu-id="8dc6f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dc6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc6f-133">id</span><span class="sxs-lookup"><span data-stu-id="8dc6f-133">id</span></span>|<span data-ttu-id="8dc6f-134">String</span><span class="sxs-lookup"><span data-stu-id="8dc6f-134">String</span></span>|<span data-ttu-id="8dc6f-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-135">Key of the setting.</span></span> <span data-ttu-id="8dc6f-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="8dc6f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8dc6f-137">displayName</span></span>|<span data-ttu-id="8dc6f-138">String</span><span class="sxs-lookup"><span data-stu-id="8dc6f-138">String</span></span>|<span data-ttu-id="8dc6f-139">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="8dc6f-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="8dc6f-140">description</span><span class="sxs-lookup"><span data-stu-id="8dc6f-140">description</span></span>|<span data-ttu-id="8dc6f-141">String</span><span class="sxs-lookup"><span data-stu-id="8dc6f-141">String</span></span>|<span data-ttu-id="8dc6f-142">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="8dc6f-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="8dc6f-143">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="8dc6f-143">rolePermissions</span></span>|<span data-ttu-id="8dc6f-144">Sammlung von Objekten des Typs [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="8dc6f-144">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="8dc6f-145">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8dc6f-146">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="8dc6f-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8dc6f-147">isBuiltIn</span></span>|<span data-ttu-id="8dc6f-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dc6f-148">Boolean</span></span>|<span data-ttu-id="8dc6f-149">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-149">Type of Role.</span></span> <span data-ttu-id="8dc6f-150">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dc6f-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8dc6f-151">Relationships</span></span>
|<span data-ttu-id="8dc6f-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8dc6f-152">Relationship</span></span>|<span data-ttu-id="8dc6f-153">Typ</span><span class="sxs-lookup"><span data-stu-id="8dc6f-153">Type</span></span>|<span data-ttu-id="8dc6f-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dc6f-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc6f-155">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="8dc6f-155">roleAssignments</span></span>|<span data-ttu-id="8dc6f-156">Sammlung von Objekten des Typs [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8dc6f-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="8dc6f-157">Liste der Rollenzuweisungen für die Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="8dc6f-157">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dc6f-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8dc6f-158">JSON Representation</span></span>
<span data-ttu-id="8dc6f-159">Unten sehen Sie eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8dc6f-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



