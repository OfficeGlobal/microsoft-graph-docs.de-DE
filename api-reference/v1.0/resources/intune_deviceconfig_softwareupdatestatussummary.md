# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="27882-101">softwareUpdateStatusSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27882-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="27882-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="27882-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27882-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="27882-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="27882-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="27882-104">Methods</span></span>
|<span data-ttu-id="27882-105">Methode</span><span class="sxs-lookup"><span data-stu-id="27882-105">Method</span></span>|<span data-ttu-id="27882-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="27882-106">Return Type</span></span>|<span data-ttu-id="27882-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27882-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27882-108">SoftwareUpdateStatusSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="27882-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="27882-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="27882-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="27882-110">Lesen von Beziehungen und Eigenschaften des [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="27882-110">Read properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="27882-111">SoftwareUpdateStatusSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="27882-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="27882-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="27882-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="27882-113">Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="27882-113">Update the properties of a [calendar](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27882-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27882-114">Properties</span></span>
|<span data-ttu-id="27882-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27882-115">Property</span></span>|<span data-ttu-id="27882-116">Typ</span><span class="sxs-lookup"><span data-stu-id="27882-116">Type</span></span>|<span data-ttu-id="27882-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27882-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27882-118">id</span><span class="sxs-lookup"><span data-stu-id="27882-118">id</span></span>|<span data-ttu-id="27882-119">String</span><span class="sxs-lookup"><span data-stu-id="27882-119">String</span></span>|<span data-ttu-id="27882-120">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="27882-120">Key of the setting.</span></span>|
|<span data-ttu-id="27882-121">displayName</span><span class="sxs-lookup"><span data-stu-id="27882-121">displayName</span></span>|<span data-ttu-id="27882-122">String</span><span class="sxs-lookup"><span data-stu-id="27882-122">String</span></span>|<span data-ttu-id="27882-123">Der Name der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="27882-123">The Name parameter specifies the name of the retention policy tag.</span></span>|
|<span data-ttu-id="27882-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27882-124">compliantDeviceCount</span></span>|<span data-ttu-id="27882-125">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-125">Int32</span></span>|<span data-ttu-id="27882-126">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="27882-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="27882-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27882-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="27882-128">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-128">Int32</span></span>|<span data-ttu-id="27882-129">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="27882-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="27882-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27882-130">remediatedDeviceCount</span></span>|<span data-ttu-id="27882-131">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-131">Int32</span></span>|<span data-ttu-id="27882-132">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="27882-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="27882-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27882-133">errorDeviceCount</span></span>|<span data-ttu-id="27882-134">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-134">Int32</span></span>|<span data-ttu-id="27882-135">Anzahl der Geräte mit Fehler</span><span class="sxs-lookup"><span data-stu-id="27882-135">Number of devices had error.</span></span>|
|<span data-ttu-id="27882-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27882-136">unknownDeviceCount</span></span>|<span data-ttu-id="27882-137">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-137">Int32</span></span>|<span data-ttu-id="27882-138">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="27882-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="27882-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27882-139">conflictDeviceCount</span></span>|<span data-ttu-id="27882-140">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-140">Int32</span></span>|<span data-ttu-id="27882-141">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="27882-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="27882-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27882-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="27882-143">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-143">Int32</span></span>|<span data-ttu-id="27882-144">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="27882-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="27882-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="27882-145">compliantUserCount</span></span>|<span data-ttu-id="27882-146">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-146">Int32</span></span>|<span data-ttu-id="27882-147">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="27882-147">Number of users: 542</span></span>|
|<span data-ttu-id="27882-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="27882-148">nonCompliantUserCount</span></span>|<span data-ttu-id="27882-149">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-149">Int32</span></span>|<span data-ttu-id="27882-150">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="27882-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="27882-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="27882-151">remediatedUserCount</span></span>|<span data-ttu-id="27882-152">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-152">Int32</span></span>|<span data-ttu-id="27882-153">Anzahl der korrigierten Benutzer</span><span class="sxs-lookup"><span data-stu-id="27882-153">Number of users: 542</span></span>|
|<span data-ttu-id="27882-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="27882-154">errorUserCount</span></span>|<span data-ttu-id="27882-155">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-155">Int32</span></span>|<span data-ttu-id="27882-156">Anzahl der Benutzer, bei denen ein Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="27882-156">Number of users had error.</span></span>|
|<span data-ttu-id="27882-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="27882-157">unknownUserCount</span></span>|<span data-ttu-id="27882-158">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-158">Int32</span></span>|<span data-ttu-id="27882-159">Anzahl der unbekannten Benutzer</span><span class="sxs-lookup"><span data-stu-id="27882-159">Number of users: 542</span></span>|
|<span data-ttu-id="27882-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="27882-160">conflictUserCount</span></span>|<span data-ttu-id="27882-161">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-161">Int32</span></span>|<span data-ttu-id="27882-162">Anzahl der Benutzer mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="27882-162">Number of users: 542</span></span>|
|<span data-ttu-id="27882-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="27882-163">notApplicableUserCount</span></span>|<span data-ttu-id="27882-164">Int32</span><span class="sxs-lookup"><span data-stu-id="27882-164">Int32</span></span>|<span data-ttu-id="27882-165">Anzahl der nicht anwendbaren Benutzer.</span><span class="sxs-lookup"><span data-stu-id="27882-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27882-166">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="27882-166">Relationships</span></span>
<span data-ttu-id="27882-167">Keine</span><span class="sxs-lookup"><span data-stu-id="27882-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27882-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27882-168">JSON Representation</span></span>
<span data-ttu-id="27882-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27882-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```



