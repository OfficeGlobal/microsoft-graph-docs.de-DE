# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="e2ba4-101">managedDeviceMobileAppConfigurationUserSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2ba4-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="e2ba4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2ba4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2ba4-103">Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Benutzerstatus von MDM-Konfigurationen mobiler Apps.</span><span class="sxs-lookup"><span data-stu-id="e2ba4-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="e2ba4-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="e2ba4-104">Methods</span></span>
|<span data-ttu-id="e2ba4-105">Methode</span><span class="sxs-lookup"><span data-stu-id="e2ba4-105">Method</span></span>|<span data-ttu-id="e2ba4-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e2ba4-106">Return Type</span></span>|<span data-ttu-id="e2ba4-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2ba4-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2ba4-108">managedDeviceMobileAppConfigurationUserSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="e2ba4-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="e2ba4-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="e2ba4-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="e2ba4-110">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e2ba4-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="e2ba4-111">managedDeviceMobileAppConfigurationUserSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e2ba4-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="e2ba4-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="e2ba4-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="e2ba4-113">Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e2ba4-113">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2ba4-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2ba4-114">Properties</span></span>
|<span data-ttu-id="e2ba4-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2ba4-115">Property</span></span>|<span data-ttu-id="e2ba4-116">Typ</span><span class="sxs-lookup"><span data-stu-id="e2ba4-116">Type</span></span>|<span data-ttu-id="e2ba4-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2ba4-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ba4-118">id</span><span class="sxs-lookup"><span data-stu-id="e2ba4-118">id</span></span>|<span data-ttu-id="e2ba4-119">String</span><span class="sxs-lookup"><span data-stu-id="e2ba4-119">String</span></span>|<span data-ttu-id="e2ba4-120">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="e2ba4-120">Key of the setting.</span></span>|
|<span data-ttu-id="e2ba4-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e2ba4-121">pendingCount</span></span>|<span data-ttu-id="e2ba4-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ba4-122">Int32</span></span>|<span data-ttu-id="e2ba4-123">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="e2ba4-123">Number of pending Users</span></span>|
|<span data-ttu-id="e2ba4-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e2ba4-124">notApplicableCount</span></span>|<span data-ttu-id="e2ba4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ba4-125">Int32</span></span>|<span data-ttu-id="e2ba4-126">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="e2ba4-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="e2ba4-127">successCount</span><span class="sxs-lookup"><span data-stu-id="e2ba4-127">successCount</span></span>|<span data-ttu-id="e2ba4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ba4-128">Int32</span></span>|<span data-ttu-id="e2ba4-129">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="e2ba4-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="e2ba4-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="e2ba4-130">errorCount</span></span>|<span data-ttu-id="e2ba4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ba4-131">Int32</span></span>|<span data-ttu-id="e2ba4-132">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="e2ba4-132">Number of error Users</span></span>|
|<span data-ttu-id="e2ba4-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="e2ba4-133">failedCount</span></span>|<span data-ttu-id="e2ba4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ba4-134">Int32</span></span>|<span data-ttu-id="e2ba4-135">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="e2ba4-135">Number of failed Users</span></span>|
|<span data-ttu-id="e2ba4-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ba4-136">lastUpdateDateTime</span></span>|<span data-ttu-id="e2ba4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2ba4-137">DateTimeOffset</span></span>|<span data-ttu-id="e2ba4-138">Zeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="e2ba4-138">Last update time</span></span>|
|<span data-ttu-id="e2ba4-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e2ba4-139">configurationVersion</span></span>|<span data-ttu-id="e2ba4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ba4-140">Int32</span></span>|<span data-ttu-id="e2ba4-141">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="e2ba4-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ba4-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2ba4-142">Relationships</span></span>
<span data-ttu-id="e2ba4-143">Keine</span><span class="sxs-lookup"><span data-stu-id="e2ba4-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2ba4-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2ba4-144">JSON Representation</span></span>
<span data-ttu-id="e2ba4-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2ba4-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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



