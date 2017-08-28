# <a name="location-resource-type"></a><span data-ttu-id="222a2-101">Location-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="222a2-101">Location resource type</span></span>

<span data-ttu-id="222a2-102">Stellt Standortinformationen eines Ereignisses dar.</span><span class="sxs-lookup"><span data-stu-id="222a2-102">Represents location information of an event.</span></span>


## <a name="properties"></a><span data-ttu-id="222a2-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="222a2-103">Properties</span></span>
| <span data-ttu-id="222a2-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="222a2-104">Property</span></span>  | <span data-ttu-id="222a2-105">Typ</span><span class="sxs-lookup"><span data-stu-id="222a2-105">Type</span></span>   | <span data-ttu-id="222a2-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="222a2-106">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="222a2-107">address</span><span class="sxs-lookup"><span data-stu-id="222a2-107">address</span></span> | [<span data-ttu-id="222a2-108">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="222a2-108">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="222a2-109">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="222a2-109">The street address of the location.</span></span> |
| <span data-ttu-id="222a2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="222a2-110">displayName</span></span>  | <span data-ttu-id="222a2-111">String</span><span class="sxs-lookup"><span data-stu-id="222a2-111">String</span></span> | <span data-ttu-id="222a2-112">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="222a2-112">The name associated with the location.</span></span>                       |
| <span data-ttu-id="222a2-113">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="222a2-113">locationEmailAddress</span></span> | <span data-ttu-id="222a2-114">String</span><span class="sxs-lookup"><span data-stu-id="222a2-114">String</span></span> | <span data-ttu-id="222a2-115">Optionale E-Mail-Adresse des Orts</span><span class="sxs-lookup"><span data-stu-id="222a2-115">Optional email address of the location.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="222a2-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="222a2-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```

## <a name="remarks"></a><span data-ttu-id="222a2-117">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="222a2-117">Remarks</span></span>

<span data-ttu-id="222a2-118">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="222a2-118">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->