# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="e6870-101">deviceConfigurationUserOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e6870-101">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="e6870-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e6870-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6870-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e6870-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="e6870-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="e6870-104">Methods</span></span>
|<span data-ttu-id="e6870-105">Methode</span><span class="sxs-lookup"><span data-stu-id="e6870-105">Method</span></span>|<span data-ttu-id="e6870-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e6870-106">Return Type</span></span>|<span data-ttu-id="e6870-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6870-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6870-108">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="e6870-108">Get deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[<span data-ttu-id="e6870-109">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="e6870-109">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="e6870-110">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6870-110">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="e6870-111">deviceConfigurationUserOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e6870-111">Update deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_update.md)|[<span data-ttu-id="e6870-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="e6870-112">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="e6870-113">Aktualisieren der Eigenschaften eines [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6870-113">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6870-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e6870-114">Properties</span></span>
|<span data-ttu-id="e6870-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6870-115">Property</span></span>|<span data-ttu-id="e6870-116">Typ</span><span class="sxs-lookup"><span data-stu-id="e6870-116">Type</span></span>|<span data-ttu-id="e6870-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6870-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6870-118">id</span><span class="sxs-lookup"><span data-stu-id="e6870-118">id</span></span>|<span data-ttu-id="e6870-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6870-119">String</span></span>|<span data-ttu-id="e6870-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e6870-120">Key of the entity.</span></span>|
|<span data-ttu-id="e6870-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e6870-121">pendingCount</span></span>|<span data-ttu-id="e6870-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e6870-122">Int32</span></span>|<span data-ttu-id="e6870-123">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="e6870-123">Number of pending Users</span></span>|
|<span data-ttu-id="e6870-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e6870-124">notApplicableCount</span></span>|<span data-ttu-id="e6870-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e6870-125">Int32</span></span>|<span data-ttu-id="e6870-126">Anzahl der nicht anwendbaren Benutzer</span><span class="sxs-lookup"><span data-stu-id="e6870-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="e6870-127">successCount</span><span class="sxs-lookup"><span data-stu-id="e6870-127">successCount</span></span>|<span data-ttu-id="e6870-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e6870-128">Int32</span></span>|<span data-ttu-id="e6870-129">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="e6870-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="e6870-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="e6870-130">errorCount</span></span>|<span data-ttu-id="e6870-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e6870-131">Int32</span></span>|<span data-ttu-id="e6870-132">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="e6870-132">Number of error Users</span></span>|
|<span data-ttu-id="e6870-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="e6870-133">failedCount</span></span>|<span data-ttu-id="e6870-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e6870-134">Int32</span></span>|<span data-ttu-id="e6870-135">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="e6870-135">Number of failed Users</span></span>|
|<span data-ttu-id="e6870-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e6870-136">lastUpdateDateTime</span></span>|<span data-ttu-id="e6870-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6870-137">DateTimeOffset</span></span>|<span data-ttu-id="e6870-138">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="e6870-138">Last update time</span></span>|
|<span data-ttu-id="e6870-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e6870-139">configurationVersion</span></span>|<span data-ttu-id="e6870-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e6870-140">Int32</span></span>|<span data-ttu-id="e6870-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="e6870-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6870-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e6870-142">Relationships</span></span>
<span data-ttu-id="e6870-143">Keine</span><span class="sxs-lookup"><span data-stu-id="e6870-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6870-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e6870-144">JSON Representation</span></span>
<span data-ttu-id="e6870-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e6870-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}-->
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



