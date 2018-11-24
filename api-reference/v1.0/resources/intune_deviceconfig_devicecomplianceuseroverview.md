# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="6cd81-101">deviceComplianceUserOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6cd81-101">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="6cd81-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6cd81-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cd81-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="6cd81-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="6cd81-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="6cd81-104">Methods</span></span>
|<span data-ttu-id="6cd81-105">Methode</span><span class="sxs-lookup"><span data-stu-id="6cd81-105">Method</span></span>|<span data-ttu-id="6cd81-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6cd81-106">Return Type</span></span>|<span data-ttu-id="6cd81-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6cd81-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6cd81-108">deviceComplianceUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="6cd81-108">Get deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[<span data-ttu-id="6cd81-109">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="6cd81-109">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="6cd81-110">Lesen von Eigenschaften und Beziehungen des [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6cd81-110">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="6cd81-111">deviceComplianceUserOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6cd81-111">Update deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[<span data-ttu-id="6cd81-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="6cd81-112">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="6cd81-113">Aktualisieren der Eigenschaften eines [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6cd81-113">Update the properties of a [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6cd81-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6cd81-114">Properties</span></span>
|<span data-ttu-id="6cd81-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6cd81-115">Property</span></span>|<span data-ttu-id="6cd81-116">Typ</span><span class="sxs-lookup"><span data-stu-id="6cd81-116">Type</span></span>|<span data-ttu-id="6cd81-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6cd81-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cd81-118">id</span><span class="sxs-lookup"><span data-stu-id="6cd81-118">id</span></span>|<span data-ttu-id="6cd81-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6cd81-119">String</span></span>|<span data-ttu-id="6cd81-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6cd81-120">Key of the entity.</span></span>|
|<span data-ttu-id="6cd81-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6cd81-121">pendingCount</span></span>|<span data-ttu-id="6cd81-122">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd81-122">Int32</span></span>|<span data-ttu-id="6cd81-123">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="6cd81-123">Number of pending Users</span></span>|
|<span data-ttu-id="6cd81-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6cd81-124">notApplicableCount</span></span>|<span data-ttu-id="6cd81-125">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd81-125">Int32</span></span>|<span data-ttu-id="6cd81-126">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="6cd81-126">Number of not applicable users</span></span>|
|<span data-ttu-id="6cd81-127">successCount</span><span class="sxs-lookup"><span data-stu-id="6cd81-127">successCount</span></span>|<span data-ttu-id="6cd81-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd81-128">Int32</span></span>|<span data-ttu-id="6cd81-129">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="6cd81-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="6cd81-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="6cd81-130">errorCount</span></span>|<span data-ttu-id="6cd81-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd81-131">Int32</span></span>|<span data-ttu-id="6cd81-132">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="6cd81-132">Number of error Users</span></span>|
|<span data-ttu-id="6cd81-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="6cd81-133">failedCount</span></span>|<span data-ttu-id="6cd81-134">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd81-134">Int32</span></span>|<span data-ttu-id="6cd81-135">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="6cd81-135">Number of failed Users</span></span>|
|<span data-ttu-id="6cd81-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6cd81-136">lastUpdateDateTime</span></span>|<span data-ttu-id="6cd81-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cd81-137">DateTimeOffset</span></span>|<span data-ttu-id="6cd81-138">Zeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="6cd81-138">Last update time</span></span>|
|<span data-ttu-id="6cd81-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6cd81-139">configurationVersion</span></span>|<span data-ttu-id="6cd81-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd81-140">Int32</span></span>|<span data-ttu-id="6cd81-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="6cd81-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cd81-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6cd81-142">Relationships</span></span>
<span data-ttu-id="6cd81-143">Keine</span><span class="sxs-lookup"><span data-stu-id="6cd81-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6cd81-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6cd81-144">JSON Representation</span></span>
<span data-ttu-id="6cd81-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6cd81-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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



