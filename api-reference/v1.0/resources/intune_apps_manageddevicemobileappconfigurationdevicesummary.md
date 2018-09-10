# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="be558-101">managedDeviceMobileAppConfigurationDeviceSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="be558-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="be558-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be558-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be558-103">Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Gerätestatus von MDM-Konfigurationen mobiler Apps.</span><span class="sxs-lookup"><span data-stu-id="be558-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="be558-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="be558-104">Methods</span></span>
|<span data-ttu-id="be558-105">Methode</span><span class="sxs-lookup"><span data-stu-id="be558-105">Method</span></span>|<span data-ttu-id="be558-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="be558-106">Return Type</span></span>|<span data-ttu-id="be558-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be558-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be558-108">managedDeviceMobileAppConfigurationDeviceSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="be558-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="be558-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="be558-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="be558-110">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="be558-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="be558-111">managedDeviceMobileAppConfigurationDeviceSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="be558-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="be558-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="be558-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="be558-113">Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="be558-113">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be558-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="be558-114">Properties</span></span>
|<span data-ttu-id="be558-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be558-115">Property</span></span>|<span data-ttu-id="be558-116">Typ</span><span class="sxs-lookup"><span data-stu-id="be558-116">Type</span></span>|<span data-ttu-id="be558-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be558-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be558-118">ID</span><span class="sxs-lookup"><span data-stu-id="be558-118">id</span></span>|<span data-ttu-id="be558-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be558-119">String</span></span>|<span data-ttu-id="be558-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="be558-120">Key of the entity.</span></span>|
|<span data-ttu-id="be558-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="be558-121">pendingCount</span></span>|<span data-ttu-id="be558-122">Int32</span><span class="sxs-lookup"><span data-stu-id="be558-122">Int32</span></span>|<span data-ttu-id="be558-123">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="be558-123">Number of pending devices</span></span>|
|<span data-ttu-id="be558-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="be558-124">notApplicableCount</span></span>|<span data-ttu-id="be558-125">Int32</span><span class="sxs-lookup"><span data-stu-id="be558-125">Int32</span></span>|<span data-ttu-id="be558-126">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="be558-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="be558-127">successCount</span><span class="sxs-lookup"><span data-stu-id="be558-127">successCount</span></span>|<span data-ttu-id="be558-128">Int32</span><span class="sxs-lookup"><span data-stu-id="be558-128">Int32</span></span>|<span data-ttu-id="be558-129">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="be558-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="be558-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="be558-130">errorCount</span></span>|<span data-ttu-id="be558-131">Int32</span><span class="sxs-lookup"><span data-stu-id="be558-131">Int32</span></span>|<span data-ttu-id="be558-132">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="be558-132">Number of error devices</span></span>|
|<span data-ttu-id="be558-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="be558-133">failedCount</span></span>|<span data-ttu-id="be558-134">Int32</span><span class="sxs-lookup"><span data-stu-id="be558-134">Int32</span></span>|<span data-ttu-id="be558-135">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="be558-135">Number of failed devices</span></span>|
|<span data-ttu-id="be558-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="be558-136">lastUpdateDateTime</span></span>|<span data-ttu-id="be558-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be558-137">DateTimeOffset</span></span>|<span data-ttu-id="be558-138">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="be558-138">Last update time</span></span>|
|<span data-ttu-id="be558-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="be558-139">configurationVersion</span></span>|<span data-ttu-id="be558-140">Int32</span><span class="sxs-lookup"><span data-stu-id="be558-140">Int32</span></span>|<span data-ttu-id="be558-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="be558-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="be558-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="be558-142">Relationships</span></span>
<span data-ttu-id="be558-143">Keine</span><span class="sxs-lookup"><span data-stu-id="be558-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be558-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="be558-144">JSON Representation</span></span>
<span data-ttu-id="be558-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="be558-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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








