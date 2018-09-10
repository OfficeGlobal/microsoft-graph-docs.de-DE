# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="46c62-101">deviceCompliancePolicyDeviceStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="46c62-101">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="46c62-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46c62-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46c62-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="46c62-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="46c62-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="46c62-104">Methods</span></span>
|<span data-ttu-id="46c62-105">Methode</span><span class="sxs-lookup"><span data-stu-id="46c62-105">Method</span></span>|<span data-ttu-id="46c62-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="46c62-106">Return Type</span></span>|<span data-ttu-id="46c62-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46c62-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="46c62-108">deviceCompliancePolicyDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="46c62-108">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[<span data-ttu-id="46c62-109">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="46c62-109">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="46c62-110">Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="46c62-110">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="46c62-111">deviceCompliancePolicyDeviceStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="46c62-111">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[<span data-ttu-id="46c62-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="46c62-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="46c62-113">Aktualisieren der Eigenschaften eines [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="46c62-113">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="46c62-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46c62-114">Properties</span></span>
|<span data-ttu-id="46c62-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46c62-115">Property</span></span>|<span data-ttu-id="46c62-116">Typ</span><span class="sxs-lookup"><span data-stu-id="46c62-116">Type</span></span>|<span data-ttu-id="46c62-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46c62-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46c62-118">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="46c62-118">inGracePeriodCount</span></span>|<span data-ttu-id="46c62-119">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-119">Int32</span></span>|<span data-ttu-id="46c62-120">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="46c62-120">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="46c62-121">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="46c62-121">configManagerCount</span></span>|<span data-ttu-id="46c62-122">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-122">Int32</span></span>|<span data-ttu-id="46c62-123">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="46c62-123">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="46c62-124">id</span><span class="sxs-lookup"><span data-stu-id="46c62-124">id</span></span>|<span data-ttu-id="46c62-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46c62-125">String</span></span>|<span data-ttu-id="46c62-126">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="46c62-126">Key of the entity.</span></span>|
|<span data-ttu-id="46c62-127">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46c62-127">unknownDeviceCount</span></span>|<span data-ttu-id="46c62-128">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-128">Int32</span></span>|<span data-ttu-id="46c62-129">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="46c62-129">Number of unknown devices</span></span>|
|<span data-ttu-id="46c62-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46c62-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="46c62-131">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-131">Int32</span></span>|<span data-ttu-id="46c62-132">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="46c62-132">Number of not applicable devices</span></span>|
|<span data-ttu-id="46c62-133">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46c62-133">compliantDeviceCount</span></span>|<span data-ttu-id="46c62-134">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-134">Int32</span></span>|<span data-ttu-id="46c62-135">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="46c62-135">Number of compliant devices</span></span>|
|<span data-ttu-id="46c62-136">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46c62-136">remediatedDeviceCount</span></span>|<span data-ttu-id="46c62-137">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-137">Int32</span></span>|<span data-ttu-id="46c62-138">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="46c62-138">Number of remediated devices</span></span>|
|<span data-ttu-id="46c62-139">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46c62-139">nonCompliantDeviceCount</span></span>|<span data-ttu-id="46c62-140">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-140">Int32</span></span>|<span data-ttu-id="46c62-141">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="46c62-141">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="46c62-142">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46c62-142">errorDeviceCount</span></span>|<span data-ttu-id="46c62-143">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-143">Int32</span></span>|<span data-ttu-id="46c62-144">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="46c62-144">Number of error devices</span></span>|
|<span data-ttu-id="46c62-145">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46c62-145">conflictDeviceCount</span></span>|<span data-ttu-id="46c62-146">Int32</span><span class="sxs-lookup"><span data-stu-id="46c62-146">Int32</span></span>|<span data-ttu-id="46c62-147">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="46c62-147">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="46c62-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="46c62-148">Relationships</span></span>
<span data-ttu-id="46c62-149">Keine</span><span class="sxs-lookup"><span data-stu-id="46c62-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46c62-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46c62-150">JSON Representation</span></span>
<span data-ttu-id="46c62-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46c62-151">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```








