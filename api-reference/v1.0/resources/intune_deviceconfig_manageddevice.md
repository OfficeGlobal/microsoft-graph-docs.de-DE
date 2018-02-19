# <a name="manageddevice-resource-type"></a><span data-ttu-id="047b6-101">managedDevice-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="047b6-101">managedDevice resource type</span></span>

> <span data-ttu-id="047b6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="047b6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="047b6-103">Über Intune verwaltete oder vorab registrierte Geräte</span><span class="sxs-lookup"><span data-stu-id="047b6-103">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="047b6-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="047b6-104">Methods</span></span>
|<span data-ttu-id="047b6-105">Methode</span><span class="sxs-lookup"><span data-stu-id="047b6-105">Method</span></span>|<span data-ttu-id="047b6-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="047b6-106">Return Type</span></span>|<span data-ttu-id="047b6-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="047b6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="047b6-108">managedDevices auflisten</span><span class="sxs-lookup"><span data-stu-id="047b6-108">List managedDevices</span></span>](../api/intune_deviceconfig_manageddevice_list.md)|<span data-ttu-id="047b6-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="047b6-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) collection</span></span>|<span data-ttu-id="047b6-110">Auflisten von Eigenschaften und Beziehungen der [managedDevice](../resources/intune_deviceconfig_manageddevice.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="047b6-110">List properties and relationships of the [managedDevice](../resources/intune_deviceconfig_manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="047b6-111">managedDevice abrufen</span><span class="sxs-lookup"><span data-stu-id="047b6-111">Get managedDevice</span></span>](../api/intune_deviceconfig_manageddevice_get.md)|[<span data-ttu-id="047b6-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="047b6-112">managedDevice</span></span>](../resources/intune_deviceconfig_manageddevice.md)|<span data-ttu-id="047b6-113">Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune_deviceconfig_manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="047b6-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_manageddevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="047b6-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="047b6-114">Properties</span></span>
|<span data-ttu-id="047b6-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="047b6-115">Property</span></span>|<span data-ttu-id="047b6-116">Typ</span><span class="sxs-lookup"><span data-stu-id="047b6-116">Type</span></span>|<span data-ttu-id="047b6-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="047b6-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="047b6-118">id</span><span class="sxs-lookup"><span data-stu-id="047b6-118">id</span></span>|<span data-ttu-id="047b6-119">String</span><span class="sxs-lookup"><span data-stu-id="047b6-119">String</span></span>|<span data-ttu-id="047b6-120">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="047b6-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="047b6-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="047b6-121">Relationships</span></span>
|<span data-ttu-id="047b6-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="047b6-122">Relationship</span></span>|<span data-ttu-id="047b6-123">Typ</span><span class="sxs-lookup"><span data-stu-id="047b6-123">Type</span></span>|<span data-ttu-id="047b6-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="047b6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="047b6-125">deviceConfigurationStates</span><span class="sxs-lookup"><span data-stu-id="047b6-125">deviceConfigurationStates</span></span>|<span data-ttu-id="047b6-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="047b6-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) collection</span></span>|<span data-ttu-id="047b6-127">Gerätekonfigurationsstatus für dieses Gerät.</span><span class="sxs-lookup"><span data-stu-id="047b6-127">Device configuration states for this device.</span></span>|
|<span data-ttu-id="047b6-128">deviceCompliancePolicyStates</span><span class="sxs-lookup"><span data-stu-id="047b6-128">deviceCompliancePolicyStates</span></span>|<span data-ttu-id="047b6-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="047b6-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) collection</span></span>|<span data-ttu-id="047b6-130">Status der Gerätekonformitätsrichtlinie für dieses Gerät.</span><span class="sxs-lookup"><span data-stu-id="047b6-130">Device compliance policy states for this device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="047b6-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="047b6-131">JSON Representation</span></span>
<span data-ttu-id="047b6-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="047b6-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



