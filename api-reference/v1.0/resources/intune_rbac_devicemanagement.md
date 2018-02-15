# <a name="devicemanagement-resource-type"></a><span data-ttu-id="1d4c0-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1d4c0-101">deviceManagement resource type</span></span>

> <span data-ttu-id="1d4c0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d4c0-103">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="1d4c0-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="1d4c0-104">Methods</span></span>
|<span data-ttu-id="1d4c0-105">Methode</span><span class="sxs-lookup"><span data-stu-id="1d4c0-105">Method</span></span>|<span data-ttu-id="1d4c0-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1d4c0-106">Return Type</span></span>|<span data-ttu-id="1d4c0-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d4c0-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="1d4c0-108">Get deviceManagement</span></span>](../api/intune_rbac_devicemanagement_get.md)|[<span data-ttu-id="1d4c0-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1d4c0-109">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="1d4c0-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_rbac_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="1d4c0-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1d4c0-111">Update deviceManagement</span></span>](../api/intune_rbac_devicemanagement_update.md)|[<span data-ttu-id="1d4c0-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1d4c0-112">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="1d4c0-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_rbac_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-113">Update the properties of a [calendar](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="1d4c0-114">GetEffectivePermissions-Funktion</span><span class="sxs-lookup"><span data-stu-id="1d4c0-114">getEffectivePermissions function</span></span>](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|<span data-ttu-id="1d4c0-115">[rolePermission](../resources/intune_rbac_rolepermission.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-115">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="1d4c0-116">Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-116">Retrieves the effective permissions of the currently authenticated user</span></span>|

## <a name="properties"></a><span data-ttu-id="1d4c0-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d4c0-117">Properties</span></span>
|<span data-ttu-id="1d4c0-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d4c0-118">Property</span></span>|<span data-ttu-id="1d4c0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="1d4c0-119">Type</span></span>|<span data-ttu-id="1d4c0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4c0-121">id</span><span class="sxs-lookup"><span data-stu-id="1d4c0-121">id</span></span>|<span data-ttu-id="1d4c0-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1d4c0-122">String</span></span>|<span data-ttu-id="1d4c0-123">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d4c0-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1d4c0-124">Relationships</span></span>
|<span data-ttu-id="1d4c0-125">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-125">Relationship</span></span>|<span data-ttu-id="1d4c0-126">Typ</span><span class="sxs-lookup"><span data-stu-id="1d4c0-126">Type</span></span>|<span data-ttu-id="1d4c0-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4c0-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="1d4c0-128">roleDefinitions</span></span>|<span data-ttu-id="1d4c0-129">[roleDefinition](../resources/intune_rbac_roledefinition.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-129">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="1d4c0-130">Rollendefinitionen</span><span class="sxs-lookup"><span data-stu-id="1d4c0-130">The Role Definitions.</span></span>|
|<span data-ttu-id="1d4c0-131">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="1d4c0-131">roleAssignments</span></span>|<span data-ttu-id="1d4c0-132">[DeviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-132">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="1d4c0-133">Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="1d4c0-133">The Role Assignments.</span></span>|
|<span data-ttu-id="1d4c0-134">resourceOperations</span><span class="sxs-lookup"><span data-stu-id="1d4c0-134">resourceOperations</span></span>|<span data-ttu-id="1d4c0-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md) collection</span></span>|<span data-ttu-id="1d4c0-136">Ressourcenvorgänge</span><span class="sxs-lookup"><span data-stu-id="1d4c0-136">The Resource Operations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d4c0-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d4c0-137">JSON Representation</span></span>
<span data-ttu-id="1d4c0-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



