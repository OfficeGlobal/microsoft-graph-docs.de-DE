# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="e1891-101">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e1891-101">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="e1891-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1891-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1891-103">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="e1891-103">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="e1891-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1891-104">Properties</span></span>
|<span data-ttu-id="e1891-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1891-105">Property</span></span>|<span data-ttu-id="e1891-106">Typ</span><span class="sxs-lookup"><span data-stu-id="e1891-106">Type</span></span>|<span data-ttu-id="e1891-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1891-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1891-108">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1891-108">lastCollectedDateTime</span></span>|<span data-ttu-id="e1891-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1891-109">DateTimeOffset</span></span>|<span data-ttu-id="e1891-110">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="e1891-110">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="e1891-111">longitude</span><span class="sxs-lookup"><span data-stu-id="e1891-111">longitude</span></span>|<span data-ttu-id="e1891-112">Double</span><span class="sxs-lookup"><span data-stu-id="e1891-112">Double</span></span>|<span data-ttu-id="e1891-113">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="e1891-113">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="e1891-114">latitude</span><span class="sxs-lookup"><span data-stu-id="e1891-114">latitude</span></span>|<span data-ttu-id="e1891-115">Double</span><span class="sxs-lookup"><span data-stu-id="e1891-115">Double</span></span>|<span data-ttu-id="e1891-116">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="e1891-116">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="e1891-117">altitude</span><span class="sxs-lookup"><span data-stu-id="e1891-117">altitude</span></span>|<span data-ttu-id="e1891-118">Double</span><span class="sxs-lookup"><span data-stu-id="e1891-118">Double</span></span>|<span data-ttu-id="e1891-119">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="e1891-119">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="e1891-120">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="e1891-120">horizontalAccuracy</span></span>|<span data-ttu-id="e1891-121">Double</span><span class="sxs-lookup"><span data-stu-id="e1891-121">Double</span></span>|<span data-ttu-id="e1891-122">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="e1891-122">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="e1891-123">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="e1891-123">verticalAccuracy</span></span>|<span data-ttu-id="e1891-124">Double</span><span class="sxs-lookup"><span data-stu-id="e1891-124">Double</span></span>|<span data-ttu-id="e1891-125">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="e1891-125">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="e1891-126">heading</span><span class="sxs-lookup"><span data-stu-id="e1891-126">heading</span></span>|<span data-ttu-id="e1891-127">Double</span><span class="sxs-lookup"><span data-stu-id="e1891-127">Double</span></span>|<span data-ttu-id="e1891-128">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="e1891-128">Heading in degrees from true north</span></span>|
|<span data-ttu-id="e1891-129">speed</span><span class="sxs-lookup"><span data-stu-id="e1891-129">speed</span></span>|<span data-ttu-id="e1891-130">Double</span><span class="sxs-lookup"><span data-stu-id="e1891-130">Double</span></span>|<span data-ttu-id="e1891-131">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="e1891-131">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1891-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e1891-132">Relationships</span></span>
<span data-ttu-id="e1891-133">Keine</span><span class="sxs-lookup"><span data-stu-id="e1891-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1891-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1891-134">JSON Representation</span></span>
<span data-ttu-id="e1891-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1891-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



