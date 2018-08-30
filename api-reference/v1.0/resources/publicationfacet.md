# <a name="publicationfacet-resource-type"></a><span data-ttu-id="29b0d-101">PublicationFacet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="29b0d-101">PublicationFacet resource type</span></span>

<span data-ttu-id="29b0d-102">Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer [DriveItemVersion](driveitemversion.md)- oder [DriveItem](driveitem.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="29b0d-102">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29b0d-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="29b0d-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="29b0d-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="29b0d-104">Properties</span></span>

|   <span data-ttu-id="29b0d-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29b0d-105">Property</span></span>    |  <span data-ttu-id="29b0d-106">Typ</span><span class="sxs-lookup"><span data-stu-id="29b0d-106">Type</span></span>  | <span data-ttu-id="29b0d-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29b0d-107">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="29b0d-108">**level**</span><span class="sxs-lookup"><span data-stu-id="29b0d-108">**level**</span></span>     | <span data-ttu-id="29b0d-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29b0d-109">String</span></span> | <span data-ttu-id="29b0d-110">Der Status der Veröffentlichung für dieses Dokument.</span><span class="sxs-lookup"><span data-stu-id="29b0d-110">The state of publication for this document.</span></span> <span data-ttu-id="29b0d-111">Möglich ist `published` oder `checkout`.</span><span class="sxs-lookup"><span data-stu-id="29b0d-111">Either `published` or `checkout`.</span></span> <span data-ttu-id="29b0d-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="29b0d-112">Read-only.</span></span>  |
| <span data-ttu-id="29b0d-113">**versionId**</span><span class="sxs-lookup"><span data-stu-id="29b0d-113">**versionId**</span></span> | <span data-ttu-id="29b0d-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29b0d-114">String</span></span> | <span data-ttu-id="29b0d-115">Der eindeutige Bezeichner für die Version, die für den aktuellen Anrufer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="29b0d-115">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="29b0d-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="29b0d-116">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
