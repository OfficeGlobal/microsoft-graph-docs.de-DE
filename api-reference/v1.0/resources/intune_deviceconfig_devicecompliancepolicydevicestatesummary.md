# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="9e38c-101">deviceCompliancePolicyDeviceStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e38c-101">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="9e38c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9e38c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e38c-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="9e38c-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="9e38c-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="9e38c-104">Methods</span></span>
|<span data-ttu-id="9e38c-105">Methode</span><span class="sxs-lookup"><span data-stu-id="9e38c-105">Method</span></span>|<span data-ttu-id="9e38c-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9e38c-106">Return Type</span></span>|<span data-ttu-id="9e38c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e38c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e38c-108">deviceCompliancePolicyDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="9e38c-108">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[<span data-ttu-id="9e38c-109">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9e38c-109">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="9e38c-110">Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e38c-110">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="9e38c-111">deviceCompliancePolicyDeviceStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9e38c-111">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[<span data-ttu-id="9e38c-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9e38c-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="9e38c-113">Aktualisieren der Eigenschaften eines [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e38c-113">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e38c-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e38c-114">Properties</span></span>
|<span data-ttu-id="9e38c-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e38c-115">Property</span></span>|<span data-ttu-id="9e38c-116">Typ</span><span class="sxs-lookup"><span data-stu-id="9e38c-116">Type</span></span>|<span data-ttu-id="9e38c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e38c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e38c-118">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-118">inGracePeriodCount</span></span>|<span data-ttu-id="9e38c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-119">Int32</span></span>|<span data-ttu-id="9e38c-120">Anzahl von Geräten, die sich in der Karenzzeit befinden</span><span class="sxs-lookup"><span data-stu-id="9e38c-120">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="9e38c-121">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-121">configManagerCount</span></span>|<span data-ttu-id="9e38c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-122">Int32</span></span>|<span data-ttu-id="9e38c-123">Anzahl von Geräten, deren Compliance mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="9e38c-123">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="9e38c-124">id</span><span class="sxs-lookup"><span data-stu-id="9e38c-124">id</span></span>|<span data-ttu-id="9e38c-125">String</span><span class="sxs-lookup"><span data-stu-id="9e38c-125">String</span></span>|<span data-ttu-id="9e38c-126">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="9e38c-126">Key of the entity.</span></span>|
|<span data-ttu-id="9e38c-127">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-127">unknownDeviceCount</span></span>|<span data-ttu-id="9e38c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-128">Int32</span></span>|<span data-ttu-id="9e38c-129">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="9e38c-129">Number of unknown devices</span></span>|
|<span data-ttu-id="9e38c-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="9e38c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-131">Int32</span></span>|<span data-ttu-id="9e38c-132">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="9e38c-132">Number of not applicable devices</span></span>|
|<span data-ttu-id="9e38c-133">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-133">compliantDeviceCount</span></span>|<span data-ttu-id="9e38c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-134">Int32</span></span>|<span data-ttu-id="9e38c-135">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="9e38c-135">Number of compliant devices</span></span>|
|<span data-ttu-id="9e38c-136">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-136">remediatedDeviceCount</span></span>|<span data-ttu-id="9e38c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-137">Int32</span></span>|<span data-ttu-id="9e38c-138">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="9e38c-138">Number of remediated devices</span></span>|
|<span data-ttu-id="9e38c-139">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-139">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9e38c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-140">Int32</span></span>|<span data-ttu-id="9e38c-141">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="9e38c-141">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="9e38c-142">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-142">errorDeviceCount</span></span>|<span data-ttu-id="9e38c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-143">Int32</span></span>|<span data-ttu-id="9e38c-144">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="9e38c-144">Number of error devices</span></span>|
|<span data-ttu-id="9e38c-145">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e38c-145">conflictDeviceCount</span></span>|<span data-ttu-id="9e38c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9e38c-146">Int32</span></span>|<span data-ttu-id="9e38c-147">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="9e38c-147">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e38c-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e38c-148">Relationships</span></span>
<span data-ttu-id="9e38c-149">Keine</span><span class="sxs-lookup"><span data-stu-id="9e38c-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e38c-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e38c-150">JSON Representation</span></span>
<span data-ttu-id="9e38c-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e38c-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
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



