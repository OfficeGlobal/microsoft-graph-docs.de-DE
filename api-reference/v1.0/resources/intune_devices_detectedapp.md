# <a name="detectedapp-resource-type"></a><span data-ttu-id="315df-101">detectedApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="315df-101">detectedApp resource type</span></span>

> <span data-ttu-id="315df-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="315df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="315df-103">Eine verwaltete oder nicht verwaltete App, die auf einem verwalteten Gerät installiert ist.</span><span class="sxs-lookup"><span data-stu-id="315df-103">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="315df-104">Nicht verwaltete Apps werden nur für als unternehmenseigen gekennzeichnete Geräte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="315df-104">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="315df-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="315df-105">Methods</span></span>
|<span data-ttu-id="315df-106">Methode</span><span class="sxs-lookup"><span data-stu-id="315df-106">Method</span></span>|<span data-ttu-id="315df-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="315df-107">Return Type</span></span>|<span data-ttu-id="315df-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="315df-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="315df-109">detectedApps auflisten</span><span class="sxs-lookup"><span data-stu-id="315df-109">List detectedApps</span></span>](../api/intune_devices_detectedapp_list.md)|<span data-ttu-id="315df-110">[detectedApp](../resources/intune_devices_detectedapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="315df-110">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="315df-111">Auflisten von Eigenschaften und Beziehungen der [detectedApp](../resources/intune_devices_detectedapp.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="315df-111">List properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="315df-112">detectedApp abrufen</span><span class="sxs-lookup"><span data-stu-id="315df-112">Get detectedApp</span></span>](../api/intune_devices_detectedapp_get.md)|[<span data-ttu-id="315df-113">detectedApp</span><span class="sxs-lookup"><span data-stu-id="315df-113">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="315df-114">Auflisten von Eigenschaften und Beziehungen des [detectedApp](../resources/intune_devices_detectedapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="315df-114">Read properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="315df-115">detectedApp erstellen</span><span class="sxs-lookup"><span data-stu-id="315df-115">Create detectedApp</span></span>](../api/intune_devices_detectedapp_create.md)|[<span data-ttu-id="315df-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="315df-116">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="315df-117">Erstellen eines neuen [detectedApp](../resources/intune_devices_detectedapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="315df-117">Create a new [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="315df-118">detectedApp löschen</span><span class="sxs-lookup"><span data-stu-id="315df-118">Delete detectedApp</span></span>](../api/intune_devices_detectedapp_delete.md)|<span data-ttu-id="315df-119">Keine</span><span class="sxs-lookup"><span data-stu-id="315df-119">None</span></span>|<span data-ttu-id="315df-120">Löscht ein [detectedApp](../resources/intune_devices_detectedapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="315df-120">Deletes a [detectedApp](../resources/intune_devices_detectedapp.md).</span></span>|
|[<span data-ttu-id="315df-121">detectedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="315df-121">Update detectedApp</span></span>](../api/intune_devices_detectedapp_update.md)|[<span data-ttu-id="315df-122">detectedApp</span><span class="sxs-lookup"><span data-stu-id="315df-122">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="315df-123">Aktualisieren der Eigenschaften eines [detectedApp](../resources/intune_devices_detectedapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="315df-123">Update the properties of a [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="315df-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="315df-124">Properties</span></span>
|<span data-ttu-id="315df-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="315df-125">Property</span></span>|<span data-ttu-id="315df-126">Typ</span><span class="sxs-lookup"><span data-stu-id="315df-126">Type</span></span>|<span data-ttu-id="315df-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="315df-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="315df-128">ID</span><span class="sxs-lookup"><span data-stu-id="315df-128">id</span></span>|<span data-ttu-id="315df-129">String</span><span class="sxs-lookup"><span data-stu-id="315df-129">String</span></span>|<span data-ttu-id="315df-130">Eindeutiger Bezeichner für die erkannte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="315df-130">The unique Identifier for the detected application.</span></span> <span data-ttu-id="315df-131">Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="315df-131">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="315df-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="315df-132">Read-only.</span></span>|
|<span data-ttu-id="315df-133">displayName</span><span class="sxs-lookup"><span data-stu-id="315df-133">displayName</span></span>|<span data-ttu-id="315df-134">String</span><span class="sxs-lookup"><span data-stu-id="315df-134">String</span></span>|<span data-ttu-id="315df-135">Name der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="315df-135">Name of the discovered application.</span></span> <span data-ttu-id="315df-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="315df-136">Read-only</span></span>|
|<span data-ttu-id="315df-137">version</span><span class="sxs-lookup"><span data-stu-id="315df-137">version</span></span>|<span data-ttu-id="315df-138">String</span><span class="sxs-lookup"><span data-stu-id="315df-138">String</span></span>|<span data-ttu-id="315df-139">Version der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="315df-139">Version of the discovered application.</span></span> <span data-ttu-id="315df-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="315df-140">Read-only</span></span>|
|<span data-ttu-id="315df-141">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="315df-141">sizeInByte</span></span>|<span data-ttu-id="315df-142">Int64</span><span class="sxs-lookup"><span data-stu-id="315df-142">Int64</span></span>|<span data-ttu-id="315df-143">Größe der ermittelten Anwendung in Byte.</span><span class="sxs-lookup"><span data-stu-id="315df-143">Discovered application size in bytes.</span></span> <span data-ttu-id="315df-144">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="315df-144">Read-only</span></span>|
|<span data-ttu-id="315df-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="315df-145">deviceCount</span></span>|<span data-ttu-id="315df-146">Int32</span><span class="sxs-lookup"><span data-stu-id="315df-146">Int32</span></span>|<span data-ttu-id="315df-147">Die Anzahl von Geräten, auf denen diese Anwendung installiert ist.</span><span class="sxs-lookup"><span data-stu-id="315df-147">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="315df-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="315df-148">Relationships</span></span>
|<span data-ttu-id="315df-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="315df-149">Relationship</span></span>|<span data-ttu-id="315df-150">Typ</span><span class="sxs-lookup"><span data-stu-id="315df-150">Type</span></span>|<span data-ttu-id="315df-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="315df-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="315df-152">managedDevices</span><span class="sxs-lookup"><span data-stu-id="315df-152">managedDevices</span></span>|<span data-ttu-id="315df-153">[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="315df-153">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="315df-154">Die Geräte, auf denen die ermittelte Anwendung installiert ist.</span><span class="sxs-lookup"><span data-stu-id="315df-154">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="315df-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="315df-155">JSON Representation</span></span>
<span data-ttu-id="315df-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="315df-156">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```








