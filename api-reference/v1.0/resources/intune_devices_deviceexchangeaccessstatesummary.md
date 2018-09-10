# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="9153b-101">deviceExchangeAccessStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9153b-101">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="9153b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9153b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9153b-103">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="9153b-103">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="9153b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9153b-104">Properties</span></span>
|<span data-ttu-id="9153b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9153b-105">Property</span></span>|<span data-ttu-id="9153b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="9153b-106">Type</span></span>|<span data-ttu-id="9153b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9153b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9153b-108">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9153b-108">allowedDeviceCount</span></span>|<span data-ttu-id="9153b-109">Int32</span><span class="sxs-lookup"><span data-stu-id="9153b-109">Int32</span></span>|<span data-ttu-id="9153b-110">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.</span><span class="sxs-lookup"><span data-stu-id="9153b-110">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="9153b-111">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9153b-111">blockedDeviceCount</span></span>|<span data-ttu-id="9153b-112">Int32</span><span class="sxs-lookup"><span data-stu-id="9153b-112">Int32</span></span>|<span data-ttu-id="9153b-113">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.</span><span class="sxs-lookup"><span data-stu-id="9153b-113">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="9153b-114">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9153b-114">quarantinedDeviceCount</span></span>|<span data-ttu-id="9153b-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9153b-115">Int32</span></span>|<span data-ttu-id="9153b-116">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="9153b-116">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="9153b-117">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9153b-117">unknownDeviceCount</span></span>|<span data-ttu-id="9153b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="9153b-118">Int32</span></span>|<span data-ttu-id="9153b-119">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="9153b-119">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="9153b-120">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9153b-120">unavailableDeviceCount</span></span>|<span data-ttu-id="9153b-121">Int32</span><span class="sxs-lookup"><span data-stu-id="9153b-121">Int32</span></span>|<span data-ttu-id="9153b-122">Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="9153b-122">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9153b-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9153b-123">Relationships</span></span>
<span data-ttu-id="9153b-124">Keine</span><span class="sxs-lookup"><span data-stu-id="9153b-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9153b-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9153b-125">JSON Representation</span></span>
<span data-ttu-id="9153b-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9153b-126">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```








