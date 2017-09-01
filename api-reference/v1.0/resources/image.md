# <a name="image-resource-type"></a><span data-ttu-id="182d7-101">Image-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="182d7-101">Image resource type</span></span>

<span data-ttu-id="182d7-p101">Die **Image**-Ressourc gruppiert bildbezogene Eigenschaften in einer einzelnen Struktur. Wenn ein [**DriveItem**](driveitem.md) ein **image**-Facet ungleich Null aufweist, stellt das Element eine Bitmapdatei dar.</span><span class="sxs-lookup"><span data-stu-id="182d7-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="182d7-104">**Hinweis:** Wenn der Dienst die Breite und Höhe des Bilds nicht bestimmen kann, ist die **Image**-Ressource möglicherweise leer.</span><span class="sxs-lookup"><span data-stu-id="182d7-104">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="182d7-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="182d7-105">JSON representation</span></span>

<span data-ttu-id="182d7-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="182d7-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.image"
}-->

```json
{
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a><span data-ttu-id="182d7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="182d7-107">Properties</span></span>

| <span data-ttu-id="182d7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="182d7-108">Property</span></span>   | <span data-ttu-id="182d7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="182d7-109">Type</span></span>  | <span data-ttu-id="182d7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="182d7-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="182d7-111">**height**</span><span class="sxs-lookup"><span data-stu-id="182d7-111">**height**</span></span> | <span data-ttu-id="182d7-112">Int32</span><span class="sxs-lookup"><span data-stu-id="182d7-112">Int32</span></span> | <span data-ttu-id="182d7-p102">Optional. Die Höhe des Bilds in Pixel. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="182d7-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="182d7-116">**width**</span><span class="sxs-lookup"><span data-stu-id="182d7-116">**width**</span></span>  | <span data-ttu-id="182d7-117">Int32</span><span class="sxs-lookup"><span data-stu-id="182d7-117">Int32</span></span> | <span data-ttu-id="182d7-p103">Optional. Die Breite des Bilds in Pixel. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="182d7-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="182d7-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="182d7-121">Remarks</span></span>

<span data-ttu-id="182d7-p104">In OneDrive for Business wird diese Ressource für Elemente zurückgegeben, von denen basierend auf der Dateierweiterung davon ausgegangen wird, dass es sich um Bilder handelt. Diese Ressource gibt keine Eigenschaften in OneDrive for Business zurück.</span><span class="sxs-lookup"><span data-stu-id="182d7-p104">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension. This resource returns no properties in OneDrive for Business.</span></span>

<span data-ttu-id="182d7-124">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="182d7-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "image resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
