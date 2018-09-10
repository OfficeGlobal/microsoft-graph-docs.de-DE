# <a name="roleassignment-resource-type"></a><span data-ttu-id="69fd2-101">roleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="69fd2-101">roleAssignment resource type</span></span>

> <span data-ttu-id="69fd2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69fd2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69fd2-103">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="69fd2-103">The Role Assignment resource.</span></span> <span data-ttu-id="69fd2-104">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="69fd2-104">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="69fd2-105">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="69fd2-105">There can be one or more role assignments per role.</span></span> <span data-ttu-id="69fd2-106">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="69fd2-106">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="69fd2-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="69fd2-107">Methods</span></span>
|<span data-ttu-id="69fd2-108">Methode</span><span class="sxs-lookup"><span data-stu-id="69fd2-108">Method</span></span>|<span data-ttu-id="69fd2-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="69fd2-109">Return Type</span></span>|<span data-ttu-id="69fd2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69fd2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69fd2-111">RoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="69fd2-111">List roleAssignments</span></span>](../api/intune_rbac_roleassignment_list.md)|<span data-ttu-id="69fd2-112">Sammlung von Objekten des Typs [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="69fd2-112">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="69fd2-113">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="69fd2-113">List properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="69fd2-114">RoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="69fd2-114">Get roleAssignment</span></span>](../api/intune_rbac_roleassignment_get.md)|[<span data-ttu-id="69fd2-115">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="69fd2-115">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="69fd2-116">Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="69fd2-116">Read properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="69fd2-117">RoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="69fd2-117">Create roleAssignment</span></span>](../api/intune_rbac_roleassignment_create.md)|[<span data-ttu-id="69fd2-118">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="69fd2-118">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="69fd2-119">Erstellen eines neuen [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="69fd2-119">Create a new [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="69fd2-120">RoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="69fd2-120">Delete roleAssignment</span></span>](../api/intune_rbac_roleassignment_delete.md)|<span data-ttu-id="69fd2-121">Keine</span><span class="sxs-lookup"><span data-stu-id="69fd2-121">None</span></span>|<span data-ttu-id="69fd2-122">Löscht ein [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="69fd2-122">Deletes a [roleAssignment](../resources/intune_rbac_roleassignment.md).</span></span>|
|[<span data-ttu-id="69fd2-123">RoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="69fd2-123">Update roleAssignment</span></span>](../api/intune_rbac_roleassignment_update.md)|[<span data-ttu-id="69fd2-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="69fd2-124">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="69fd2-125">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="69fd2-125">Update the properties of a [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69fd2-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69fd2-126">Properties</span></span>
|<span data-ttu-id="69fd2-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69fd2-127">Property</span></span>|<span data-ttu-id="69fd2-128">Typ</span><span class="sxs-lookup"><span data-stu-id="69fd2-128">Type</span></span>|<span data-ttu-id="69fd2-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69fd2-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69fd2-130">ID</span><span class="sxs-lookup"><span data-stu-id="69fd2-130">id</span></span>|<span data-ttu-id="69fd2-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69fd2-131">String</span></span>|<span data-ttu-id="69fd2-132">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="69fd2-132">Key of the entity.</span></span> <span data-ttu-id="69fd2-133">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="69fd2-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="69fd2-134">displayName</span><span class="sxs-lookup"><span data-stu-id="69fd2-134">displayName</span></span>|<span data-ttu-id="69fd2-135">String</span><span class="sxs-lookup"><span data-stu-id="69fd2-135">String</span></span>|<span data-ttu-id="69fd2-136">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="69fd2-136">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="69fd2-137">description</span><span class="sxs-lookup"><span data-stu-id="69fd2-137">description</span></span>|<span data-ttu-id="69fd2-138">String</span><span class="sxs-lookup"><span data-stu-id="69fd2-138">String</span></span>|<span data-ttu-id="69fd2-139">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="69fd2-139">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="69fd2-140">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="69fd2-140">resourceScopes</span></span>|<span data-ttu-id="69fd2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="69fd2-141">String collection</span></span>|<span data-ttu-id="69fd2-142">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="69fd2-142">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="69fd2-143">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="69fd2-143">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69fd2-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69fd2-144">Relationships</span></span>
|<span data-ttu-id="69fd2-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="69fd2-145">Relationship</span></span>|<span data-ttu-id="69fd2-146">Typ</span><span class="sxs-lookup"><span data-stu-id="69fd2-146">Type</span></span>|<span data-ttu-id="69fd2-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69fd2-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69fd2-148">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="69fd2-148">roleDefinition</span></span>|[<span data-ttu-id="69fd2-149">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="69fd2-149">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="69fd2-150">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="69fd2-150">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69fd2-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69fd2-151">JSON Representation</span></span>
<span data-ttu-id="69fd2-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="69fd2-152">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```








