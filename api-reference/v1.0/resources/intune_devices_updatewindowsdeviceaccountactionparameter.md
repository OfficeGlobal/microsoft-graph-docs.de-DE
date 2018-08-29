# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="e760b-101">updateWindowsDeviceAccountActionParameter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e760b-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="e760b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e760b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e760b-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e760b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e760b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e760b-104">Properties</span></span>
|<span data-ttu-id="e760b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e760b-105">Property</span></span>|<span data-ttu-id="e760b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="e760b-106">Type</span></span>|<span data-ttu-id="e760b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e760b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e760b-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="e760b-108">deviceAccount</span></span>|[<span data-ttu-id="e760b-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="e760b-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="e760b-110">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e760b-110">Not yet documented</span></span>|
|<span data-ttu-id="e760b-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="e760b-111">passwordRotationEnabled</span></span>|<span data-ttu-id="e760b-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e760b-112">Boolean</span></span>|<span data-ttu-id="e760b-113">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e760b-113">Not yet documented</span></span>|
|<span data-ttu-id="e760b-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="e760b-114">calendarSyncEnabled</span></span>|<span data-ttu-id="e760b-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e760b-115">Boolean</span></span>|<span data-ttu-id="e760b-116">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e760b-116">Not yet documented</span></span>|
|<span data-ttu-id="e760b-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="e760b-117">deviceAccountEmail</span></span>|<span data-ttu-id="e760b-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e760b-118">String</span></span>|<span data-ttu-id="e760b-119">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e760b-119">Not yet documented</span></span>|
|<span data-ttu-id="e760b-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="e760b-120">exchangeServer</span></span>|<span data-ttu-id="e760b-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e760b-121">String</span></span>|<span data-ttu-id="e760b-122">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e760b-122">Not yet documented</span></span>|
|<span data-ttu-id="e760b-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="e760b-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="e760b-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e760b-124">String</span></span>|<span data-ttu-id="e760b-125">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e760b-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="e760b-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e760b-126">Relationships</span></span>
<span data-ttu-id="e760b-127">Keine</span><span class="sxs-lookup"><span data-stu-id="e760b-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e760b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e760b-128">JSON Representation</span></span>
<span data-ttu-id="e760b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e760b-129">Here is a JSON representation of the resource.</span></span>
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



