# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="1d735-101">updateWindowsDeviceAccountActionParameter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1d735-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="1d735-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d735-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d735-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1d735-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1d735-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d735-104">Properties</span></span>
|<span data-ttu-id="1d735-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d735-105">Property</span></span>|<span data-ttu-id="1d735-106">Typ</span><span class="sxs-lookup"><span data-stu-id="1d735-106">Type</span></span>|<span data-ttu-id="1d735-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d735-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d735-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="1d735-108">deviceAccount</span></span>|[<span data-ttu-id="1d735-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="1d735-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="1d735-110">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d735-110">Not yet documented</span></span>|
|<span data-ttu-id="1d735-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="1d735-111">passwordRotationEnabled</span></span>|<span data-ttu-id="1d735-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1d735-112">Boolean</span></span>|<span data-ttu-id="1d735-113">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d735-113">Not yet documented</span></span>|
|<span data-ttu-id="1d735-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="1d735-114">calendarSyncEnabled</span></span>|<span data-ttu-id="1d735-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1d735-115">Boolean</span></span>|<span data-ttu-id="1d735-116">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d735-116">Not yet documented</span></span>|
|<span data-ttu-id="1d735-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="1d735-117">deviceAccountEmail</span></span>|<span data-ttu-id="1d735-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1d735-118">String</span></span>|<span data-ttu-id="1d735-119">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d735-119">Not yet documented</span></span>|
|<span data-ttu-id="1d735-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="1d735-120">exchangeServer</span></span>|<span data-ttu-id="1d735-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1d735-121">String</span></span>|<span data-ttu-id="1d735-122">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d735-122">Not yet documented</span></span>|
|<span data-ttu-id="1d735-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="1d735-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="1d735-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1d735-124">String</span></span>|<span data-ttu-id="1d735-125">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d735-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d735-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1d735-126">Relationships</span></span>
<span data-ttu-id="1d735-127">Keine</span><span class="sxs-lookup"><span data-stu-id="1d735-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d735-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d735-128">JSON Representation</span></span>
<span data-ttu-id="1d735-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d735-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```








