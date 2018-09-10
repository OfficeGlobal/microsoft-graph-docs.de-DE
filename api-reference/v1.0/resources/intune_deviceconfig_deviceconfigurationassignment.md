# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="33eb2-101">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="33eb2-101">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="33eb2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="33eb2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33eb2-103">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="33eb2-103">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="33eb2-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="33eb2-104">Methods</span></span>
|<span data-ttu-id="33eb2-105">Methode</span><span class="sxs-lookup"><span data-stu-id="33eb2-105">Method</span></span>|<span data-ttu-id="33eb2-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="33eb2-106">Return Type</span></span>|<span data-ttu-id="33eb2-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33eb2-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="33eb2-108">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="33eb2-108">List deviceConfigurationAssignments</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|<span data-ttu-id="33eb2-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="33eb2-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="33eb2-110">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="33eb2-110">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="33eb2-111">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="33eb2-111">Get deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[<span data-ttu-id="33eb2-112">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="33eb2-112">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="33eb2-113">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="33eb2-113">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="33eb2-114">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="33eb2-114">Create deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[<span data-ttu-id="33eb2-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="33eb2-115">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="33eb2-116">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="33eb2-116">Create a new [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="33eb2-117">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="33eb2-117">Delete deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|<span data-ttu-id="33eb2-118">Keine</span><span class="sxs-lookup"><span data-stu-id="33eb2-118">None</span></span>|<span data-ttu-id="33eb2-119">Löscht ein [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="33eb2-119">Deletes a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="33eb2-120">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="33eb2-120">Update deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[<span data-ttu-id="33eb2-121">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="33eb2-121">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="33eb2-122">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="33eb2-122">Update the properties of a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="33eb2-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="33eb2-123">Properties</span></span>
|<span data-ttu-id="33eb2-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33eb2-124">Property</span></span>|<span data-ttu-id="33eb2-125">Typ</span><span class="sxs-lookup"><span data-stu-id="33eb2-125">Type</span></span>|<span data-ttu-id="33eb2-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33eb2-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33eb2-127">ID</span><span class="sxs-lookup"><span data-stu-id="33eb2-127">id</span></span>|<span data-ttu-id="33eb2-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33eb2-128">String</span></span>|<span data-ttu-id="33eb2-129">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="33eb2-129">The key of the assignment.</span></span>|
|<span data-ttu-id="33eb2-130">Ziel</span><span class="sxs-lookup"><span data-stu-id="33eb2-130">target</span></span>|[<span data-ttu-id="33eb2-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="33eb2-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="33eb2-132">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33eb2-132">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33eb2-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="33eb2-133">Relationships</span></span>
<span data-ttu-id="33eb2-134">Keine</span><span class="sxs-lookup"><span data-stu-id="33eb2-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33eb2-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33eb2-135">JSON Representation</span></span>
<span data-ttu-id="33eb2-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="33eb2-136">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








