# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="6bc97-101">deviceAppManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6bc97-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="6bc97-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6bc97-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bc97-103">Singleton-Entität, die als Container für alle Geräte-App-Verwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="6bc97-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="6bc97-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="6bc97-104">Methods</span></span>
|<span data-ttu-id="6bc97-105">Methode</span><span class="sxs-lookup"><span data-stu-id="6bc97-105">Method</span></span>|<span data-ttu-id="6bc97-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6bc97-106">Return Type</span></span>|<span data-ttu-id="6bc97-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bc97-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bc97-108">deviceAppManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="6bc97-108">Get deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_get.md)|[<span data-ttu-id="6bc97-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6bc97-109">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="6bc97-110">Lesen von Eigenschaften und Beziehungen des [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6bc97-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="6bc97-111">deviceAppManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6bc97-111">Update deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_update.md)|[<span data-ttu-id="6bc97-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6bc97-112">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="6bc97-113">Aktualisieren der Eigenschaften eines [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6bc97-113">Update the properties of a [calendar](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bc97-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6bc97-114">Properties</span></span>
|<span data-ttu-id="6bc97-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6bc97-115">Property</span></span>|<span data-ttu-id="6bc97-116">Typ</span><span class="sxs-lookup"><span data-stu-id="6bc97-116">Type</span></span>|<span data-ttu-id="6bc97-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bc97-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc97-118">id</span><span class="sxs-lookup"><span data-stu-id="6bc97-118">id</span></span>|<span data-ttu-id="6bc97-119">String</span><span class="sxs-lookup"><span data-stu-id="6bc97-119">String</span></span>|<span data-ttu-id="6bc97-120">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="6bc97-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bc97-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6bc97-121">Relationships</span></span>
|<span data-ttu-id="6bc97-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6bc97-122">Relationship</span></span>|<span data-ttu-id="6bc97-123">Typ</span><span class="sxs-lookup"><span data-stu-id="6bc97-123">Type</span></span>|<span data-ttu-id="6bc97-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bc97-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc97-125">mobileApps</span><span class="sxs-lookup"><span data-stu-id="6bc97-125">mobileApps</span></span>|<span data-ttu-id="6bc97-126">[mobileApp](../resources/intune_apps_mobileapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6bc97-126">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="6bc97-127">Die mobilen Apps.</span><span class="sxs-lookup"><span data-stu-id="6bc97-127">The mobile apps.</span></span>|
|<span data-ttu-id="6bc97-128">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="6bc97-128">mobileAppCategories</span></span>|<span data-ttu-id="6bc97-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6bc97-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="6bc97-130">Die Kategorien der mobilen Apps.</span><span class="sxs-lookup"><span data-stu-id="6bc97-130">The mobile app categories.</span></span>|
|<span data-ttu-id="6bc97-131">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="6bc97-131">mobileAppConfigurations</span></span>|<span data-ttu-id="6bc97-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6bc97-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="6bc97-133">Die Konfigurationen der mobilen Apps für verwaltete Geräte.</span><span class="sxs-lookup"><span data-stu-id="6bc97-133">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bc97-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6bc97-134">JSON Representation</span></span>
<span data-ttu-id="6bc97-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6bc97-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



