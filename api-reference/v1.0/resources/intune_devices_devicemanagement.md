# <a name="devicemanagement-resource-type"></a><span data-ttu-id="10ddd-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="10ddd-101">deviceManagement resource type</span></span>

> <span data-ttu-id="10ddd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10ddd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10ddd-103">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="10ddd-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="10ddd-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="10ddd-104">Methods</span></span>
|<span data-ttu-id="10ddd-105">Methode</span><span class="sxs-lookup"><span data-stu-id="10ddd-105">Method</span></span>|<span data-ttu-id="10ddd-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="10ddd-106">Return Type</span></span>|<span data-ttu-id="10ddd-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10ddd-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10ddd-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="10ddd-108">Get deviceManagement</span></span>](../api/intune_devices_devicemanagement_get.md)|[<span data-ttu-id="10ddd-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="10ddd-109">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="10ddd-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_devices_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="10ddd-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="10ddd-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="10ddd-111">Update deviceManagement</span></span>](../api/intune_devices_devicemanagement_update.md)|[<span data-ttu-id="10ddd-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="10ddd-112">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="10ddd-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_devices_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="10ddd-113">Update the properties of a [calendar](../resources/intune_devices_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10ddd-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10ddd-114">Properties</span></span>
|<span data-ttu-id="10ddd-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10ddd-115">Property</span></span>|<span data-ttu-id="10ddd-116">Typ</span><span class="sxs-lookup"><span data-stu-id="10ddd-116">Type</span></span>|<span data-ttu-id="10ddd-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10ddd-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10ddd-118">id</span><span class="sxs-lookup"><span data-stu-id="10ddd-118">id</span></span>|<span data-ttu-id="10ddd-119">String</span><span class="sxs-lookup"><span data-stu-id="10ddd-119">String</span></span>|<span data-ttu-id="10ddd-120">Eindeutiger Bezeichner für das Gerät</span><span class="sxs-lookup"><span data-stu-id="10ddd-120">Unique Identifier for the device</span></span>|
|<span data-ttu-id="10ddd-121">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="10ddd-121">subscriptionState</span></span>|<span data-ttu-id="10ddd-122">String</span><span class="sxs-lookup"><span data-stu-id="10ddd-122">String</span></span>|<span data-ttu-id="10ddd-123">Abonnementstatus für Verwaltung mobiler Geräte des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="10ddd-123">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="10ddd-124">Mögliche Werte: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="10ddd-124">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10ddd-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="10ddd-125">Relationships</span></span>
|<span data-ttu-id="10ddd-126">Beziehung</span><span class="sxs-lookup"><span data-stu-id="10ddd-126">Relationship</span></span>|<span data-ttu-id="10ddd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="10ddd-127">Type</span></span>|<span data-ttu-id="10ddd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10ddd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10ddd-129">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="10ddd-129">applePushNotificationCertificate</span></span>|[<span data-ttu-id="10ddd-130">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="10ddd-130">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="10ddd-131">Apple Push Notification-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="10ddd-131">Apple push notification certificate.</span></span>|
|<span data-ttu-id="10ddd-132">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="10ddd-132">managedDeviceOverview</span></span>|[<span data-ttu-id="10ddd-133">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="10ddd-133">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="10ddd-134">Geräteübersicht</span><span class="sxs-lookup"><span data-stu-id="10ddd-134">Device overview</span></span>|
|<span data-ttu-id="10ddd-135">detectedApps</span><span class="sxs-lookup"><span data-stu-id="10ddd-135">detectedApps</span></span>|<span data-ttu-id="10ddd-136">[detectedApp](../resources/intune_devices_detectedapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="10ddd-136">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="10ddd-137">Die Liste der erkannten Apps, die einem Gerät zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="10ddd-137">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="10ddd-138">managedDevices</span><span class="sxs-lookup"><span data-stu-id="10ddd-138">managedDevices</span></span>|<span data-ttu-id="10ddd-139">[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="10ddd-139">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="10ddd-140">Die Liste der verwalteten Geräte</span><span class="sxs-lookup"><span data-stu-id="10ddd-140">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10ddd-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10ddd-141">JSON Representation</span></span>
<span data-ttu-id="10ddd-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10ddd-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



