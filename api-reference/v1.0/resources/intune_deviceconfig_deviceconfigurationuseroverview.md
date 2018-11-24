# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="2b315-101">deviceConfigurationUserOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2b315-101">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="2b315-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2b315-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b315-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="2b315-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="2b315-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="2b315-104">Methods</span></span>
|<span data-ttu-id="2b315-105">Methode</span><span class="sxs-lookup"><span data-stu-id="2b315-105">Method</span></span>|<span data-ttu-id="2b315-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2b315-106">Return Type</span></span>|<span data-ttu-id="2b315-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b315-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b315-108">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="2b315-108">Get deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[<span data-ttu-id="2b315-109">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="2b315-109">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="2b315-110">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b315-110">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="2b315-111">deviceConfigurationUserOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2b315-111">Update deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_update.md)|[<span data-ttu-id="2b315-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="2b315-112">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="2b315-113">Aktualisieren der Eigenschaften eines [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b315-113">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b315-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2b315-114">Properties</span></span>
|<span data-ttu-id="2b315-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b315-115">Property</span></span>|<span data-ttu-id="2b315-116">Typ</span><span class="sxs-lookup"><span data-stu-id="2b315-116">Type</span></span>|<span data-ttu-id="2b315-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b315-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b315-118">id</span><span class="sxs-lookup"><span data-stu-id="2b315-118">id</span></span>|<span data-ttu-id="2b315-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b315-119">String</span></span>|<span data-ttu-id="2b315-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2b315-120">Key of the entity.</span></span>|
|<span data-ttu-id="2b315-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="2b315-121">pendingCount</span></span>|<span data-ttu-id="2b315-122">Int32</span><span class="sxs-lookup"><span data-stu-id="2b315-122">Int32</span></span>|<span data-ttu-id="2b315-123">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="2b315-123">Number of pending Users</span></span>|
|<span data-ttu-id="2b315-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2b315-124">notApplicableCount</span></span>|<span data-ttu-id="2b315-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2b315-125">Int32</span></span>|<span data-ttu-id="2b315-126">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="2b315-126">Number of not applicable users</span></span>|
|<span data-ttu-id="2b315-127">successCount</span><span class="sxs-lookup"><span data-stu-id="2b315-127">successCount</span></span>|<span data-ttu-id="2b315-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2b315-128">Int32</span></span>|<span data-ttu-id="2b315-129">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="2b315-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="2b315-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="2b315-130">errorCount</span></span>|<span data-ttu-id="2b315-131">Int32</span><span class="sxs-lookup"><span data-stu-id="2b315-131">Int32</span></span>|<span data-ttu-id="2b315-132">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="2b315-132">Number of error Users</span></span>|
|<span data-ttu-id="2b315-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="2b315-133">failedCount</span></span>|<span data-ttu-id="2b315-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2b315-134">Int32</span></span>|<span data-ttu-id="2b315-135">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="2b315-135">Number of failed Users</span></span>|
|<span data-ttu-id="2b315-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2b315-136">lastUpdateDateTime</span></span>|<span data-ttu-id="2b315-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b315-137">DateTimeOffset</span></span>|<span data-ttu-id="2b315-138">Zeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="2b315-138">Last update time</span></span>|
|<span data-ttu-id="2b315-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="2b315-139">configurationVersion</span></span>|<span data-ttu-id="2b315-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2b315-140">Int32</span></span>|<span data-ttu-id="2b315-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="2b315-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b315-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2b315-142">Relationships</span></span>
<span data-ttu-id="2b315-143">Keine</span><span class="sxs-lookup"><span data-stu-id="2b315-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2b315-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2b315-144">JSON Representation</span></span>
<span data-ttu-id="2b315-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2b315-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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



