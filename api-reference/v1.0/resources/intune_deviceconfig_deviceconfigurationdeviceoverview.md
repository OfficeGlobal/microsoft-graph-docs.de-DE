# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="39eda-101">deviceConfigurationDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="39eda-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="39eda-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="39eda-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39eda-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="39eda-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="39eda-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="39eda-104">Methods</span></span>
|<span data-ttu-id="39eda-105">Methode</span><span class="sxs-lookup"><span data-stu-id="39eda-105">Method</span></span>|<span data-ttu-id="39eda-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="39eda-106">Return Type</span></span>|<span data-ttu-id="39eda-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39eda-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39eda-108">deviceConfigurationDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="39eda-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="39eda-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="39eda-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="39eda-110">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="39eda-110">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="39eda-111">deviceConfigurationDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="39eda-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="39eda-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="39eda-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="39eda-113">Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="39eda-113">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="39eda-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="39eda-114">Properties</span></span>
|<span data-ttu-id="39eda-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39eda-115">Property</span></span>|<span data-ttu-id="39eda-116">Typ</span><span class="sxs-lookup"><span data-stu-id="39eda-116">Type</span></span>|<span data-ttu-id="39eda-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39eda-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39eda-118">id</span><span class="sxs-lookup"><span data-stu-id="39eda-118">id</span></span>|<span data-ttu-id="39eda-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39eda-119">String</span></span>|<span data-ttu-id="39eda-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="39eda-120">Key of the entity.</span></span>|
|<span data-ttu-id="39eda-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="39eda-121">pendingCount</span></span>|<span data-ttu-id="39eda-122">Int32</span><span class="sxs-lookup"><span data-stu-id="39eda-122">Int32</span></span>|<span data-ttu-id="39eda-123">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="39eda-123">Number of pending devices</span></span>|
|<span data-ttu-id="39eda-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="39eda-124">notApplicableCount</span></span>|<span data-ttu-id="39eda-125">Int32</span><span class="sxs-lookup"><span data-stu-id="39eda-125">Int32</span></span>|<span data-ttu-id="39eda-126">Anzahl der nicht anwendbaren Geräte</span><span class="sxs-lookup"><span data-stu-id="39eda-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="39eda-127">successCount</span><span class="sxs-lookup"><span data-stu-id="39eda-127">successCount</span></span>|<span data-ttu-id="39eda-128">Int32</span><span class="sxs-lookup"><span data-stu-id="39eda-128">Int32</span></span>|<span data-ttu-id="39eda-129">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="39eda-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="39eda-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="39eda-130">errorCount</span></span>|<span data-ttu-id="39eda-131">Int32</span><span class="sxs-lookup"><span data-stu-id="39eda-131">Int32</span></span>|<span data-ttu-id="39eda-132">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="39eda-132">Number of error devices</span></span>|
|<span data-ttu-id="39eda-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="39eda-133">failedCount</span></span>|<span data-ttu-id="39eda-134">Int32</span><span class="sxs-lookup"><span data-stu-id="39eda-134">Int32</span></span>|<span data-ttu-id="39eda-135">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="39eda-135">Number of failed devices</span></span>|
|<span data-ttu-id="39eda-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="39eda-136">lastUpdateDateTime</span></span>|<span data-ttu-id="39eda-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39eda-137">DateTimeOffset</span></span>|<span data-ttu-id="39eda-138">Zeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="39eda-138">Last update time</span></span>|
|<span data-ttu-id="39eda-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="39eda-139">configurationVersion</span></span>|<span data-ttu-id="39eda-140">Int32</span><span class="sxs-lookup"><span data-stu-id="39eda-140">Int32</span></span>|<span data-ttu-id="39eda-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="39eda-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="39eda-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="39eda-142">Relationships</span></span>
<span data-ttu-id="39eda-143">Keine</span><span class="sxs-lookup"><span data-stu-id="39eda-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39eda-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="39eda-144">JSON Representation</span></span>
<span data-ttu-id="39eda-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="39eda-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
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



