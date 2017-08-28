# <a name="thumbnail-resource-type"></a><span data-ttu-id="959c9-101">thumbnail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="959c9-101">Thumbnail resource type</span></span>

<span data-ttu-id="959c9-102">Der **thumbnail**-Ressourcentyp stellt eine Miniaturansicht für ein Bild, ein Video, ein Dokument oder ein beliebiges Element dar, das über eine Bitmapdarstellung verfügt.</span><span class="sxs-lookup"><span data-stu-id="959c9-102">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="959c9-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="959c9-103">JSON representation</span></span>

<span data-ttu-id="959c9-104">Es folgt eine JSON-Darstellung der **thumbnail**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="959c9-104">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="959c9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="959c9-105">Properties</span></span>

| <span data-ttu-id="959c9-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="959c9-106">Property</span></span>     | <span data-ttu-id="959c9-107">Typ</span><span class="sxs-lookup"><span data-stu-id="959c9-107">Type</span></span>   | <span data-ttu-id="959c9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="959c9-108">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="959c9-109">height</span><span class="sxs-lookup"><span data-stu-id="959c9-109">height</span></span>       | <span data-ttu-id="959c9-110">Int32</span><span class="sxs-lookup"><span data-stu-id="959c9-110">Int32</span></span>  | <span data-ttu-id="959c9-111">Die Höhe der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="959c9-111">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="959c9-112">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="959c9-112">sourceItemId</span></span> | <span data-ttu-id="959c9-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="959c9-113">String</span></span> | <span data-ttu-id="959c9-p101">Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="959c9-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="959c9-116">url</span><span class="sxs-lookup"><span data-stu-id="959c9-116">url</span></span>          | <span data-ttu-id="959c9-117">String</span><span class="sxs-lookup"><span data-stu-id="959c9-117">String</span></span> | <span data-ttu-id="959c9-118">Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="959c9-118">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="959c9-119">width</span><span class="sxs-lookup"><span data-stu-id="959c9-119">width</span></span>        | <span data-ttu-id="959c9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="959c9-120">Int32</span></span>  | <span data-ttu-id="959c9-121">Die Breite der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="959c9-121">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="959c9-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="959c9-122">Relationships</span></span>

| <span data-ttu-id="959c9-123">Name</span><span class="sxs-lookup"><span data-stu-id="959c9-123">Name</span></span>    | <span data-ttu-id="959c9-124">Typ</span><span class="sxs-lookup"><span data-stu-id="959c9-124">Type</span></span>   | <span data-ttu-id="959c9-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="959c9-125">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="959c9-126">Inhalt</span><span class="sxs-lookup"><span data-stu-id="959c9-126">content</span></span> | <span data-ttu-id="959c9-127">Stream</span><span class="sxs-lookup"><span data-stu-id="959c9-127">Stream</span></span> | <span data-ttu-id="959c9-128">Der Inhaltsdatenstrom für die Miniaturansicht.</span><span class="sxs-lookup"><span data-stu-id="959c9-128">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
