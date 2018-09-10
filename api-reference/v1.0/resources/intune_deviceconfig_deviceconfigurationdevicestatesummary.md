# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="75d7a-101">deviceConfigurationDeviceStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="75d7a-101">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="75d7a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="75d7a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75d7a-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="75d7a-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="75d7a-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="75d7a-104">Methods</span></span>
|<span data-ttu-id="75d7a-105">Methode</span><span class="sxs-lookup"><span data-stu-id="75d7a-105">Method</span></span>|<span data-ttu-id="75d7a-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="75d7a-106">Return Type</span></span>|<span data-ttu-id="75d7a-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75d7a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75d7a-108">deviceConfigurationDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="75d7a-108">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[<span data-ttu-id="75d7a-109">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="75d7a-109">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="75d7a-110">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="75d7a-110">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="75d7a-111">deviceConfigurationDeviceStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="75d7a-111">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[<span data-ttu-id="75d7a-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="75d7a-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="75d7a-113">Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="75d7a-113">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75d7a-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="75d7a-114">Properties</span></span>
|<span data-ttu-id="75d7a-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75d7a-115">Property</span></span>|<span data-ttu-id="75d7a-116">Typ</span><span class="sxs-lookup"><span data-stu-id="75d7a-116">Type</span></span>|<span data-ttu-id="75d7a-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75d7a-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75d7a-118">ID</span><span class="sxs-lookup"><span data-stu-id="75d7a-118">id</span></span>|<span data-ttu-id="75d7a-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="75d7a-119">String</span></span>|<span data-ttu-id="75d7a-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="75d7a-120">Key of the entity.</span></span>|
|<span data-ttu-id="75d7a-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75d7a-121">unknownDeviceCount</span></span>|<span data-ttu-id="75d7a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="75d7a-122">Int32</span></span>|<span data-ttu-id="75d7a-123">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="75d7a-123">Number of unknown devices</span></span>|
|<span data-ttu-id="75d7a-124">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75d7a-124">notApplicableDeviceCount</span></span>|<span data-ttu-id="75d7a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="75d7a-125">Int32</span></span>|<span data-ttu-id="75d7a-126">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="75d7a-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="75d7a-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75d7a-127">compliantDeviceCount</span></span>|<span data-ttu-id="75d7a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="75d7a-128">Int32</span></span>|<span data-ttu-id="75d7a-129">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="75d7a-129">Number of compliant devices</span></span>|
|<span data-ttu-id="75d7a-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75d7a-130">remediatedDeviceCount</span></span>|<span data-ttu-id="75d7a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="75d7a-131">Int32</span></span>|<span data-ttu-id="75d7a-132">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="75d7a-132">Number of remediated devices</span></span>|
|<span data-ttu-id="75d7a-133">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75d7a-133">nonCompliantDeviceCount</span></span>|<span data-ttu-id="75d7a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="75d7a-134">Int32</span></span>|<span data-ttu-id="75d7a-135">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="75d7a-135">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="75d7a-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75d7a-136">errorDeviceCount</span></span>|<span data-ttu-id="75d7a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="75d7a-137">Int32</span></span>|<span data-ttu-id="75d7a-138">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="75d7a-138">Number of error devices</span></span>|
|<span data-ttu-id="75d7a-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75d7a-139">conflictDeviceCount</span></span>|<span data-ttu-id="75d7a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="75d7a-140">Int32</span></span>|<span data-ttu-id="75d7a-141">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="75d7a-141">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="75d7a-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="75d7a-142">Relationships</span></span>
<span data-ttu-id="75d7a-143">Keine</span><span class="sxs-lookup"><span data-stu-id="75d7a-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="75d7a-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="75d7a-144">JSON Representation</span></span>
<span data-ttu-id="75d7a-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="75d7a-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
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








