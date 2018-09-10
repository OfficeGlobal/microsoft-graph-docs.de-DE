# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="27a6c-101">managedDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27a6c-101">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="27a6c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="27a6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27a6c-103">Zusammenfassungsdaten für verwaltete Geräte</span><span class="sxs-lookup"><span data-stu-id="27a6c-103">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="27a6c-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="27a6c-104">Methods</span></span>
|<span data-ttu-id="27a6c-105">Methode</span><span class="sxs-lookup"><span data-stu-id="27a6c-105">Method</span></span>|<span data-ttu-id="27a6c-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="27a6c-106">Return Type</span></span>|<span data-ttu-id="27a6c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27a6c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27a6c-108">managedDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="27a6c-108">Get managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_get.md)|[<span data-ttu-id="27a6c-109">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="27a6c-109">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="27a6c-110">Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="27a6c-110">Read properties and relationships of the [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="27a6c-111">managedDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="27a6c-111">Update managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_update.md)|[<span data-ttu-id="27a6c-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="27a6c-112">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="27a6c-113">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="27a6c-113">Update the properties of a [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27a6c-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27a6c-114">Properties</span></span>
|<span data-ttu-id="27a6c-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27a6c-115">Property</span></span>|<span data-ttu-id="27a6c-116">Typ</span><span class="sxs-lookup"><span data-stu-id="27a6c-116">Type</span></span>|<span data-ttu-id="27a6c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27a6c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27a6c-118">ID</span><span class="sxs-lookup"><span data-stu-id="27a6c-118">id</span></span>|<span data-ttu-id="27a6c-119">String</span><span class="sxs-lookup"><span data-stu-id="27a6c-119">String</span></span>|<span data-ttu-id="27a6c-120">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="27a6c-120">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="27a6c-121">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27a6c-121">enrolledDeviceCount</span></span>|<span data-ttu-id="27a6c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="27a6c-122">Int32</span></span>|<span data-ttu-id="27a6c-123">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="27a6c-123">Total enrolled device count.</span></span> <span data-ttu-id="27a6c-124">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="27a6c-124">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="27a6c-125">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="27a6c-125">mdmEnrolledCount</span></span>|<span data-ttu-id="27a6c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="27a6c-126">Int32</span></span>|<span data-ttu-id="27a6c-127">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="27a6c-127">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="27a6c-128">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27a6c-128">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="27a6c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="27a6c-129">Int32</span></span>|<span data-ttu-id="27a6c-130">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="27a6c-130">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="27a6c-131">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="27a6c-131">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="27a6c-132">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="27a6c-132">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="27a6c-133">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="27a6c-133">Device operating system summary.</span></span>|
|<span data-ttu-id="27a6c-134">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="27a6c-134">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="27a6c-135">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="27a6c-135">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="27a6c-136">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="27a6c-136">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="27a6c-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="27a6c-137">Relationships</span></span>
<span data-ttu-id="27a6c-138">Keine</span><span class="sxs-lookup"><span data-stu-id="27a6c-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27a6c-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27a6c-139">JSON Representation</span></span>
<span data-ttu-id="27a6c-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27a6c-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```








