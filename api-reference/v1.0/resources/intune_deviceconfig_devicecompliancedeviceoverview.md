# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="295c1-101">deviceComplianceDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="295c1-101">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="295c1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="295c1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="295c1-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="295c1-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="295c1-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="295c1-104">Methods</span></span>
|<span data-ttu-id="295c1-105">Methode</span><span class="sxs-lookup"><span data-stu-id="295c1-105">Method</span></span>|<span data-ttu-id="295c1-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="295c1-106">Return Type</span></span>|<span data-ttu-id="295c1-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="295c1-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="295c1-108">deviceComplianceDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="295c1-108">Get deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_get.md)|[<span data-ttu-id="295c1-109">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="295c1-109">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="295c1-110">Lesen von Eigenschaften und Beziehungen des [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="295c1-110">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="295c1-111">deviceComplianceDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="295c1-111">Update deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_update.md)|[<span data-ttu-id="295c1-112">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="295c1-112">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="295c1-113">Aktualisieren der Eigenschaften eines [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="295c1-113">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="295c1-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="295c1-114">Properties</span></span>
|<span data-ttu-id="295c1-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="295c1-115">Property</span></span>|<span data-ttu-id="295c1-116">Typ</span><span class="sxs-lookup"><span data-stu-id="295c1-116">Type</span></span>|<span data-ttu-id="295c1-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="295c1-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="295c1-118">id</span><span class="sxs-lookup"><span data-stu-id="295c1-118">id</span></span>|<span data-ttu-id="295c1-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="295c1-119">String</span></span>|<span data-ttu-id="295c1-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="295c1-120">Key of the entity.</span></span>|
|<span data-ttu-id="295c1-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="295c1-121">pendingCount</span></span>|<span data-ttu-id="295c1-122">Int32</span><span class="sxs-lookup"><span data-stu-id="295c1-122">Int32</span></span>|<span data-ttu-id="295c1-123">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="295c1-123">Number of pending devices</span></span>|
|<span data-ttu-id="295c1-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="295c1-124">notApplicableCount</span></span>|<span data-ttu-id="295c1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="295c1-125">Int32</span></span>|<span data-ttu-id="295c1-126">Anzahl der nicht anwendbaren Geräte</span><span class="sxs-lookup"><span data-stu-id="295c1-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="295c1-127">successCount</span><span class="sxs-lookup"><span data-stu-id="295c1-127">successCount</span></span>|<span data-ttu-id="295c1-128">Int32</span><span class="sxs-lookup"><span data-stu-id="295c1-128">Int32</span></span>|<span data-ttu-id="295c1-129">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="295c1-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="295c1-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="295c1-130">errorCount</span></span>|<span data-ttu-id="295c1-131">Int32</span><span class="sxs-lookup"><span data-stu-id="295c1-131">Int32</span></span>|<span data-ttu-id="295c1-132">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="295c1-132">Number of error devices</span></span>|
|<span data-ttu-id="295c1-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="295c1-133">failedCount</span></span>|<span data-ttu-id="295c1-134">Int32</span><span class="sxs-lookup"><span data-stu-id="295c1-134">Int32</span></span>|<span data-ttu-id="295c1-135">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="295c1-135">Number of failed devices</span></span>|
|<span data-ttu-id="295c1-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="295c1-136">lastUpdateDateTime</span></span>|<span data-ttu-id="295c1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="295c1-137">DateTimeOffset</span></span>|<span data-ttu-id="295c1-138">Zeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="295c1-138">Last update time</span></span>|
|<span data-ttu-id="295c1-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="295c1-139">configurationVersion</span></span>|<span data-ttu-id="295c1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="295c1-140">Int32</span></span>|<span data-ttu-id="295c1-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="295c1-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="295c1-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="295c1-142">Relationships</span></span>
<span data-ttu-id="295c1-143">Keine</span><span class="sxs-lookup"><span data-stu-id="295c1-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="295c1-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="295c1-144">JSON Representation</span></span>
<span data-ttu-id="295c1-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="295c1-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



