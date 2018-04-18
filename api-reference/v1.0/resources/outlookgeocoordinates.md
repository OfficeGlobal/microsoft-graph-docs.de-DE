# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="7885b-101">outlookGeoCoordinates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7885b-101">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="7885b-102">Die geografischen Koordinaten, die Erhebung und deren Genauigkeitsgrad für einen physischen Ort.</span><span class="sxs-lookup"><span data-stu-id="7885b-102">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7885b-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7885b-103">JSON representation</span></span>

<span data-ttu-id="7885b-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7885b-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="7885b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7885b-105">Properties</span></span>
| <span data-ttu-id="7885b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7885b-106">Property</span></span>     | <span data-ttu-id="7885b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7885b-107">Type</span></span>   |<span data-ttu-id="7885b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7885b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7885b-109">accuracy</span><span class="sxs-lookup"><span data-stu-id="7885b-109">accuracy</span></span>|<span data-ttu-id="7885b-110">double</span><span class="sxs-lookup"><span data-stu-id="7885b-110">double</span></span>|<span data-ttu-id="7885b-111">Die Genauigkeit des Breiten- und Längengrads.</span><span class="sxs-lookup"><span data-stu-id="7885b-111">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="7885b-112">Die Genauigkeit kann beispielsweise in Metern gemessen werden, der Breiten- und Längengrad sind beispielsweise auf 50 Meter genau.</span><span class="sxs-lookup"><span data-stu-id="7885b-112">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="7885b-113">altitude</span><span class="sxs-lookup"><span data-stu-id="7885b-113">altitude</span></span>|<span data-ttu-id="7885b-114">double</span><span class="sxs-lookup"><span data-stu-id="7885b-114">double</span></span>|<span data-ttu-id="7885b-115">Die Höhe des Orts.</span><span class="sxs-lookup"><span data-stu-id="7885b-115">The altitude of the location.</span></span>|
|<span data-ttu-id="7885b-116">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="7885b-116">altitudeAccuracy</span></span>|<span data-ttu-id="7885b-117">double</span><span class="sxs-lookup"><span data-stu-id="7885b-117">double</span></span>|<span data-ttu-id="7885b-118">Die Genauigkeit der Höhe.</span><span class="sxs-lookup"><span data-stu-id="7885b-118">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="7885b-119">latitude</span><span class="sxs-lookup"><span data-stu-id="7885b-119">latitude</span></span>|<span data-ttu-id="7885b-120">double</span><span class="sxs-lookup"><span data-stu-id="7885b-120">double</span></span>|<span data-ttu-id="7885b-121">Der Breitengrad des Orts.</span><span class="sxs-lookup"><span data-stu-id="7885b-121">The latitude of the location.</span></span>|
|<span data-ttu-id="7885b-122">longitude</span><span class="sxs-lookup"><span data-stu-id="7885b-122">longitude</span></span>|<span data-ttu-id="7885b-123">double</span><span class="sxs-lookup"><span data-stu-id="7885b-123">double</span></span>|<span data-ttu-id="7885b-124">Der Längengrad des Orts.</span><span class="sxs-lookup"><span data-stu-id="7885b-124">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->