# <a name="icon-resource-type"></a><span data-ttu-id="70e73-101">Icon-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="70e73-101">Icon resource type</span></span>

<span data-ttu-id="70e73-102">Stellt ein Zellensymbol dar.</span><span class="sxs-lookup"><span data-stu-id="70e73-102">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="70e73-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="70e73-103">Methods</span></span>

| <span data-ttu-id="70e73-104">Methode</span><span class="sxs-lookup"><span data-stu-id="70e73-104">Method</span></span>           | <span data-ttu-id="70e73-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="70e73-105">Return Type</span></span>    |<span data-ttu-id="70e73-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70e73-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70e73-107">Symbol abrufen</span><span class="sxs-lookup"><span data-stu-id="70e73-107">Get Icon</span></span>](../api/icon_get.md) | [<span data-ttu-id="70e73-108">Symbol</span><span class="sxs-lookup"><span data-stu-id="70e73-108">Icon</span></span>](icon.md) |<span data-ttu-id="70e73-109">Dient zum Lesen der Eigenschaften und der Beziehungen des Symbol-Objekts.</span><span class="sxs-lookup"><span data-stu-id="70e73-109">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="70e73-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="70e73-110">Update</span></span>](../api/icon_update.md) | [<span data-ttu-id="70e73-111">Symbol</span><span class="sxs-lookup"><span data-stu-id="70e73-111">Icon</span></span>](icon.md)  |<span data-ttu-id="70e73-112">Dient zum Aktualisieren des Symbol-Objekts.</span><span class="sxs-lookup"><span data-stu-id="70e73-112">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="70e73-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70e73-113">Properties</span></span>
| <span data-ttu-id="70e73-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70e73-114">Property</span></span>     | <span data-ttu-id="70e73-115">Typ</span><span class="sxs-lookup"><span data-stu-id="70e73-115">Type</span></span>   |<span data-ttu-id="70e73-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70e73-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70e73-117">Index</span><span class="sxs-lookup"><span data-stu-id="70e73-117">index</span></span>|<span data-ttu-id="70e73-118">int</span><span class="sxs-lookup"><span data-stu-id="70e73-118">int</span></span>|<span data-ttu-id="70e73-119">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="70e73-119">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="70e73-120">Gruppe</span><span class="sxs-lookup"><span data-stu-id="70e73-120">set</span></span>|<span data-ttu-id="70e73-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70e73-121">string</span></span>|<span data-ttu-id="70e73-122">Repräsentiert die Gruppe, zu der das Symbol gehört.</span><span class="sxs-lookup"><span data-stu-id="70e73-122">Represents the set that the icon is part of. Possible values are: , , , , , , , , , , , , , , , , , , , , .</span></span> <span data-ttu-id="70e73-123">Mögliche Werte: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="70e73-123">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70e73-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="70e73-124">Relationships</span></span>
<span data-ttu-id="70e73-125">Keine</span><span class="sxs-lookup"><span data-stu-id="70e73-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="70e73-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70e73-126">JSON representation</span></span>

<span data-ttu-id="70e73-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70e73-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->