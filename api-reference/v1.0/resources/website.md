# <a name="website-resource-type"></a><span data-ttu-id="bf352-101">website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bf352-101">website resource type</span></span>

<span data-ttu-id="bf352-102">Stellt eine Website dar.</span><span class="sxs-lookup"><span data-stu-id="bf352-102">Represents a SharePoint Foundation website.</span></span>


## <a name="properties"></a><span data-ttu-id="bf352-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bf352-103">Properties</span></span>
| <span data-ttu-id="bf352-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf352-104">Property</span></span>     | <span data-ttu-id="bf352-105">Typ</span><span class="sxs-lookup"><span data-stu-id="bf352-105">Type</span></span>   |<span data-ttu-id="bf352-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf352-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf352-107">type</span><span class="sxs-lookup"><span data-stu-id="bf352-107">type</span></span>|<span data-ttu-id="bf352-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bf352-108">String</span></span>| <span data-ttu-id="bf352-109">Mögliche Werte: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="bf352-109">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="bf352-110">address</span><span class="sxs-lookup"><span data-stu-id="bf352-110">address</span></span>|<span data-ttu-id="bf352-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bf352-111">string</span></span>|<span data-ttu-id="bf352-112">Die URL der Website.</span><span class="sxs-lookup"><span data-stu-id="bf352-112">The URL of the current website.</span></span>|
|<span data-ttu-id="bf352-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bf352-113">displayName</span></span>|<span data-ttu-id="bf352-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bf352-114">string</span></span>|<span data-ttu-id="bf352-115">Der Anzeigename der Website.</span><span class="sxs-lookup"><span data-stu-id="bf352-115">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf352-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bf352-116">JSON representation</span></span>

<span data-ttu-id="bf352-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bf352-117">Here is a JSON representation of the resource</span></span>

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
