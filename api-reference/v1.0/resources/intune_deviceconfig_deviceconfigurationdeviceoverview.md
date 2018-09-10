# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="93c24-101">deviceConfigurationDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93c24-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="93c24-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93c24-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93c24-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="93c24-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="93c24-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="93c24-104">Methods</span></span>
|<span data-ttu-id="93c24-105">Methode</span><span class="sxs-lookup"><span data-stu-id="93c24-105">Method</span></span>|<span data-ttu-id="93c24-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="93c24-106">Return Type</span></span>|<span data-ttu-id="93c24-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93c24-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93c24-108">deviceConfigurationDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="93c24-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="93c24-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="93c24-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="93c24-110">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="93c24-110">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="93c24-111">deviceConfigurationDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="93c24-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="93c24-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="93c24-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="93c24-113">Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="93c24-113">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="93c24-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93c24-114">Properties</span></span>
|<span data-ttu-id="93c24-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93c24-115">Property</span></span>|<span data-ttu-id="93c24-116">Typ</span><span class="sxs-lookup"><span data-stu-id="93c24-116">Type</span></span>|<span data-ttu-id="93c24-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93c24-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93c24-118">ID</span><span class="sxs-lookup"><span data-stu-id="93c24-118">id</span></span>|<span data-ttu-id="93c24-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93c24-119">String</span></span>|<span data-ttu-id="93c24-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="93c24-120">Key of the entity.</span></span>|
|<span data-ttu-id="93c24-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="93c24-121">pendingCount</span></span>|<span data-ttu-id="93c24-122">Int32</span><span class="sxs-lookup"><span data-stu-id="93c24-122">Int32</span></span>|<span data-ttu-id="93c24-123">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="93c24-123">Number of pending devices</span></span>|
|<span data-ttu-id="93c24-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="93c24-124">notApplicableCount</span></span>|<span data-ttu-id="93c24-125">Int32</span><span class="sxs-lookup"><span data-stu-id="93c24-125">Int32</span></span>|<span data-ttu-id="93c24-126">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="93c24-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="93c24-127">successCount</span><span class="sxs-lookup"><span data-stu-id="93c24-127">successCount</span></span>|<span data-ttu-id="93c24-128">Int32</span><span class="sxs-lookup"><span data-stu-id="93c24-128">Int32</span></span>|<span data-ttu-id="93c24-129">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="93c24-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="93c24-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="93c24-130">errorCount</span></span>|<span data-ttu-id="93c24-131">Int32</span><span class="sxs-lookup"><span data-stu-id="93c24-131">Int32</span></span>|<span data-ttu-id="93c24-132">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="93c24-132">Number of error devices</span></span>|
|<span data-ttu-id="93c24-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="93c24-133">failedCount</span></span>|<span data-ttu-id="93c24-134">Int32</span><span class="sxs-lookup"><span data-stu-id="93c24-134">Int32</span></span>|<span data-ttu-id="93c24-135">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="93c24-135">Number of failed devices</span></span>|
|<span data-ttu-id="93c24-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="93c24-136">lastUpdateDateTime</span></span>|<span data-ttu-id="93c24-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93c24-137">DateTimeOffset</span></span>|<span data-ttu-id="93c24-138">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="93c24-138">Last update time</span></span>|
|<span data-ttu-id="93c24-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="93c24-139">configurationVersion</span></span>|<span data-ttu-id="93c24-140">Int32</span><span class="sxs-lookup"><span data-stu-id="93c24-140">Int32</span></span>|<span data-ttu-id="93c24-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="93c24-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="93c24-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="93c24-142">Relationships</span></span>
<span data-ttu-id="93c24-143">Keine</span><span class="sxs-lookup"><span data-stu-id="93c24-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="93c24-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93c24-144">JSON Representation</span></span>
<span data-ttu-id="93c24-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93c24-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}-->
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








