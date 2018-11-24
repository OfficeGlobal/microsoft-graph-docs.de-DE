# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="b8b36-101">updateWindowsDeviceAccountActionParameter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8b36-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="b8b36-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8b36-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8b36-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8b36-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b8b36-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8b36-104">Properties</span></span>
|<span data-ttu-id="b8b36-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8b36-105">Property</span></span>|<span data-ttu-id="b8b36-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b8b36-106">Type</span></span>|<span data-ttu-id="b8b36-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8b36-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b36-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="b8b36-108">deviceAccount</span></span>|[<span data-ttu-id="b8b36-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="b8b36-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="b8b36-110">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8b36-110">Not yet documented</span></span>|
|<span data-ttu-id="b8b36-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="b8b36-111">passwordRotationEnabled</span></span>|<span data-ttu-id="b8b36-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8b36-112">Boolean</span></span>|<span data-ttu-id="b8b36-113">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8b36-113">Not yet documented</span></span>|
|<span data-ttu-id="b8b36-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="b8b36-114">calendarSyncEnabled</span></span>|<span data-ttu-id="b8b36-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8b36-115">Boolean</span></span>|<span data-ttu-id="b8b36-116">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8b36-116">Not yet documented</span></span>|
|<span data-ttu-id="b8b36-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b8b36-117">deviceAccountEmail</span></span>|<span data-ttu-id="b8b36-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8b36-118">String</span></span>|<span data-ttu-id="b8b36-119">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8b36-119">Not yet documented</span></span>|
|<span data-ttu-id="b8b36-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="b8b36-120">exchangeServer</span></span>|<span data-ttu-id="b8b36-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8b36-121">String</span></span>|<span data-ttu-id="b8b36-122">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8b36-122">Not yet documented</span></span>|
|<span data-ttu-id="b8b36-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="b8b36-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="b8b36-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8b36-124">String</span></span>|<span data-ttu-id="b8b36-125">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8b36-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8b36-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8b36-126">Relationships</span></span>
<span data-ttu-id="b8b36-127">Keine</span><span class="sxs-lookup"><span data-stu-id="b8b36-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8b36-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8b36-128">JSON Representation</span></span>
<span data-ttu-id="b8b36-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8b36-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
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



