# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="96f7d-101">managedDeviceMobileAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="96f7d-101">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="96f7d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96f7d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96f7d-103">Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.</span><span class="sxs-lookup"><span data-stu-id="96f7d-103">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="96f7d-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="96f7d-104">Methods</span></span>
|<span data-ttu-id="96f7d-105">Methode</span><span class="sxs-lookup"><span data-stu-id="96f7d-105">Method</span></span>|<span data-ttu-id="96f7d-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="96f7d-106">Return Type</span></span>|<span data-ttu-id="96f7d-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96f7d-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96f7d-108">managedDeviceMobileAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="96f7d-108">List managedDeviceMobileAppConfigurations</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|<span data-ttu-id="96f7d-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="96f7d-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="96f7d-110">Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="96f7d-110">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="96f7d-111">managedDeviceMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="96f7d-111">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[<span data-ttu-id="96f7d-112">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="96f7d-112">managedDeviceMobileAppConfiguration</span></span>](../resources/intune_apps_manageddevicemobileappconfiguration.md)|<span data-ttu-id="96f7d-113">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="96f7d-113">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96f7d-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96f7d-114">Properties</span></span>
|<span data-ttu-id="96f7d-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96f7d-115">Property</span></span>|<span data-ttu-id="96f7d-116">Typ</span><span class="sxs-lookup"><span data-stu-id="96f7d-116">Type</span></span>|<span data-ttu-id="96f7d-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96f7d-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96f7d-118">ID</span><span class="sxs-lookup"><span data-stu-id="96f7d-118">id</span></span>|<span data-ttu-id="96f7d-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96f7d-119">String</span></span>|<span data-ttu-id="96f7d-120">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="96f7d-120">Key of the entity.</span></span>|
|<span data-ttu-id="96f7d-121">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="96f7d-121">targetedMobileApps</span></span>|<span data-ttu-id="96f7d-122">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="96f7d-122">String collection</span></span>|<span data-ttu-id="96f7d-123">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="96f7d-123">the associated app.</span></span>|
|<span data-ttu-id="96f7d-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96f7d-124">createdDateTime</span></span>|<span data-ttu-id="96f7d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96f7d-125">DateTimeOffset</span></span>|<span data-ttu-id="96f7d-126">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="96f7d-126">DateTime the object was created.</span></span>|
|<span data-ttu-id="96f7d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96f7d-127">description</span></span>|<span data-ttu-id="96f7d-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96f7d-128">String</span></span>|<span data-ttu-id="96f7d-129">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="96f7d-129">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="96f7d-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96f7d-130">lastModifiedDateTime</span></span>|<span data-ttu-id="96f7d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96f7d-131">DateTimeOffset</span></span>|<span data-ttu-id="96f7d-132">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="96f7d-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="96f7d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="96f7d-133">displayName</span></span>|<span data-ttu-id="96f7d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96f7d-134">String</span></span>|<span data-ttu-id="96f7d-135">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="96f7d-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="96f7d-136">Version</span><span class="sxs-lookup"><span data-stu-id="96f7d-136">version</span></span>|<span data-ttu-id="96f7d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="96f7d-137">Int32</span></span>|<span data-ttu-id="96f7d-138">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="96f7d-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96f7d-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="96f7d-139">Relationships</span></span>
|<span data-ttu-id="96f7d-140">Beziehung</span><span class="sxs-lookup"><span data-stu-id="96f7d-140">Relationship</span></span>|<span data-ttu-id="96f7d-141">Typ</span><span class="sxs-lookup"><span data-stu-id="96f7d-141">Type</span></span>|<span data-ttu-id="96f7d-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96f7d-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96f7d-143">Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="96f7d-143">assignments</span></span>|<span data-ttu-id="96f7d-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="96f7d-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="96f7d-145">Die Liste der Gruppenzuweisungen für die App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="96f7d-145">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="96f7d-146">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="96f7d-146">deviceStatuses</span></span>|<span data-ttu-id="96f7d-147">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="96f7d-147">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="96f7d-148">Liste von ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="96f7d-148">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="96f7d-149">userStatuses</span><span class="sxs-lookup"><span data-stu-id="96f7d-149">userStatuses</span></span>|<span data-ttu-id="96f7d-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="96f7d-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="96f7d-151">Liste von ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="96f7d-151">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="96f7d-152">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="96f7d-152">deviceStatusSummary</span></span>|[<span data-ttu-id="96f7d-153">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="96f7d-153">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="96f7d-154">Zusammenfassung der App-Konfiguration-Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="96f7d-154">App configuration device status summary.</span></span>|
|<span data-ttu-id="96f7d-155">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="96f7d-155">userStatusSummary</span></span>|[<span data-ttu-id="96f7d-156">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="96f7d-156">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="96f7d-157">Zusammenfassung der App-Konfiguration-Benutzerstatus.</span><span class="sxs-lookup"><span data-stu-id="96f7d-157">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96f7d-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96f7d-158">JSON Representation</span></span>
<span data-ttu-id="96f7d-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96f7d-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```








