# <a name="website-resource-type"></a><span data-ttu-id="676ab-101">website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="676ab-101">website resource type</span></span>

<span data-ttu-id="676ab-102">Stellt eine Website dar.</span><span class="sxs-lookup"><span data-stu-id="676ab-102">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="676ab-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="676ab-103">Properties</span></span>
| <span data-ttu-id="676ab-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="676ab-104">Property</span></span>     | <span data-ttu-id="676ab-105">Typ</span><span class="sxs-lookup"><span data-stu-id="676ab-105">Type</span></span>   |<span data-ttu-id="676ab-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="676ab-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="676ab-107">type</span><span class="sxs-lookup"><span data-stu-id="676ab-107">type</span></span>|<span data-ttu-id="676ab-108">websiteType</span><span class="sxs-lookup"><span data-stu-id="676ab-108">WebsiteType</span></span>| <span data-ttu-id="676ab-109">Die möglichen Werte sind: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="676ab-109">The possible values are `other`, `home`, `work`, `blog`, `profile`, , , , , , , or .</span></span>|
|<span data-ttu-id="676ab-110">address</span><span class="sxs-lookup"><span data-stu-id="676ab-110">address</span></span>|<span data-ttu-id="676ab-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="676ab-111">string</span></span>|<span data-ttu-id="676ab-112">Die URL der Website.</span><span class="sxs-lookup"><span data-stu-id="676ab-112">The URL of the website.</span></span>|
|<span data-ttu-id="676ab-113">displayName</span><span class="sxs-lookup"><span data-stu-id="676ab-113">displayName</span></span>|<span data-ttu-id="676ab-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="676ab-114">string</span></span>|<span data-ttu-id="676ab-115">Der Anzeigename der Website.</span><span class="sxs-lookup"><span data-stu-id="676ab-115">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="676ab-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="676ab-116">JSON representation</span></span>

<span data-ttu-id="676ab-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="676ab-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
