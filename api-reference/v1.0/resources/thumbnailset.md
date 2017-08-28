# <a name="thumbnailset-resource-type"></a><span data-ttu-id="4e010-101">ThumbnailSet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4e010-101">ThumbnailSet resource type</span></span>

<span data-ttu-id="4e010-p101">Die **ThumbnailSet**-Ressource ist eine verschlüsselter Sammlung von [thumbnail](thumbnail.md)-Ressourcen. Sie wird zum Darstellen eines Satzes von Miniaturansichten verwendet, die mit einem DriveItem verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="4e010-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e010-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e010-104">JSON representation</span></span>

<span data-ttu-id="4e010-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e010-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": {"@odata.type": "microsoft.graph.thumbnail"},
  "medium": {"@odata.type": "microsoft.graph.thumbnail"},
  "small": {"@odata.type": "microsoft.graph.thumbnail"},
  "source": {"@odata.type": "microsoft.graph.thumbnail"}
}
```

## <a name="properties"></a><span data-ttu-id="4e010-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e010-106">Properties</span></span>

| <span data-ttu-id="4e010-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e010-107">Property</span></span> | <span data-ttu-id="4e010-108">Typ</span><span class="sxs-lookup"><span data-stu-id="4e010-108">Type</span></span>                      | <span data-ttu-id="4e010-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e010-109">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="4e010-110">id</span><span class="sxs-lookup"><span data-stu-id="4e010-110">id</span></span>       | <span data-ttu-id="4e010-111">String</span><span class="sxs-lookup"><span data-stu-id="4e010-111">String</span></span>                    | <span data-ttu-id="4e010-p102">Die ID innerhalb des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e010-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="4e010-114">large</span><span class="sxs-lookup"><span data-stu-id="4e010-114">large</span></span>    | [<span data-ttu-id="4e010-115">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="4e010-115">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4e010-116">Eine skalierte Miniaturansicht von 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="4e010-116">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="4e010-117">medium</span><span class="sxs-lookup"><span data-stu-id="4e010-117">medium</span></span>   | [<span data-ttu-id="4e010-118">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="4e010-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4e010-119">Eine skalierte Miniaturansicht von 176x176.</span><span class="sxs-lookup"><span data-stu-id="4e010-119">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="4e010-120">small</span><span class="sxs-lookup"><span data-stu-id="4e010-120">small</span></span>    | [<span data-ttu-id="4e010-121">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="4e010-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4e010-122">Eine zugeschnittene Miniaturansicht von 48x48.</span><span class="sxs-lookup"><span data-stu-id="4e010-122">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="4e010-123">source</span><span class="sxs-lookup"><span data-stu-id="4e010-123">source</span></span>   | [<span data-ttu-id="4e010-124">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="4e010-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4e010-125">Eine benutzerdefiniertes Miniaturbild oder das ursprüngliche Bild, das zum Erstellen anderer Miniaturansichten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4e010-125">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnailSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
