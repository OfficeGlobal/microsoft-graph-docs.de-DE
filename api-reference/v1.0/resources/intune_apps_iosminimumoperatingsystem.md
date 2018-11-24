# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="77a6c-101">iosMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77a6c-101">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="77a6c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="77a6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77a6c-103">Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="77a6c-103">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="77a6c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77a6c-104">Properties</span></span>
|<span data-ttu-id="77a6c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77a6c-105">Property</span></span>|<span data-ttu-id="77a6c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="77a6c-106">Type</span></span>|<span data-ttu-id="77a6c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77a6c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77a6c-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="77a6c-108">v8_0</span></span>|<span data-ttu-id="77a6c-109">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77a6c-109">Boolean</span></span>|<span data-ttu-id="77a6c-110">Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="77a6c-110">Version 8.0 or later.</span></span>|
|<span data-ttu-id="77a6c-111">v9_0</span><span class="sxs-lookup"><span data-stu-id="77a6c-111">v9_0</span></span>|<span data-ttu-id="77a6c-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77a6c-112">Boolean</span></span>|<span data-ttu-id="77a6c-113">Version 9.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="77a6c-113">Version 9.0 or later.</span></span>|
|<span data-ttu-id="77a6c-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="77a6c-114">v10_0</span></span>|<span data-ttu-id="77a6c-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77a6c-115">Boolean</span></span>|<span data-ttu-id="77a6c-116">Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="77a6c-116">Version 10.0 or later.</span></span>|
|<span data-ttu-id="77a6c-117">v11_0</span><span class="sxs-lookup"><span data-stu-id="77a6c-117">v11_0</span></span>|<span data-ttu-id="77a6c-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77a6c-118">Boolean</span></span>|<span data-ttu-id="77a6c-119">Version 11.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="77a6c-119">Version 11.0 or later.</span></span>|
|<span data-ttu-id="77a6c-120">v12_0</span><span class="sxs-lookup"><span data-stu-id="77a6c-120">v12_0</span></span>|<span data-ttu-id="77a6c-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77a6c-121">Boolean</span></span>|<span data-ttu-id="77a6c-122">Version 12.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="77a6c-122">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77a6c-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77a6c-123">Relationships</span></span>
<span data-ttu-id="77a6c-124">Keine</span><span class="sxs-lookup"><span data-stu-id="77a6c-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="77a6c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77a6c-125">JSON Representation</span></span>
<span data-ttu-id="77a6c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77a6c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



