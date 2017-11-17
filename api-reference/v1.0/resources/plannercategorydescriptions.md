<span data-ttu-id="e9843-p101">Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum [planDetails](plannerplandetails.md)-Objekt. Es können bis zu 6 Kategorien definiert werden.</span><span class="sxs-lookup"><span data-stu-id="e9843-p101">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span>

Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum [planDetails](plannerplandetails.md)-Objekt. Es können bis zu 6 Kategorien definiert werden. 


## <span data-ttu-id="e9843-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9843-105">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="e9843-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9843-106">Property</span></span>     | <span data-ttu-id="e9843-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e9843-107">Type</span></span>   |<span data-ttu-id="e9843-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9843-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9843-109">category1</span><span class="sxs-lookup"><span data-stu-id="e9843-109">category1</span></span>|<span data-ttu-id="e9843-110">String</span><span class="sxs-lookup"><span data-stu-id="e9843-110">String</span></span>|<span data-ttu-id="e9843-111">Mit Kategorie 1 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e9843-111">The label associated with Category 1</span></span>|
|<span data-ttu-id="e9843-112">category2</span><span class="sxs-lookup"><span data-stu-id="e9843-112">category2</span></span>|<span data-ttu-id="e9843-113">String</span><span class="sxs-lookup"><span data-stu-id="e9843-113">String</span></span>|<span data-ttu-id="e9843-114">Mit Kategorie 2 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e9843-114">The label associated with Category 2</span></span>|
|<span data-ttu-id="e9843-115">category3</span><span class="sxs-lookup"><span data-stu-id="e9843-115">category3</span></span>|<span data-ttu-id="e9843-116">String</span><span class="sxs-lookup"><span data-stu-id="e9843-116">String</span></span>|<span data-ttu-id="e9843-117">Mit Kategorie 3 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e9843-117">The label associated with Category 3</span></span>|
|<span data-ttu-id="e9843-118">category4</span><span class="sxs-lookup"><span data-stu-id="e9843-118">category4</span></span>|<span data-ttu-id="e9843-119">String</span><span class="sxs-lookup"><span data-stu-id="e9843-119">String</span></span>|<span data-ttu-id="e9843-120">Mit Kategorie 4 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e9843-120">The label associated with Category 4</span></span>|
|<span data-ttu-id="e9843-121">category5</span><span class="sxs-lookup"><span data-stu-id="e9843-121">category5</span></span>|<span data-ttu-id="e9843-122">String</span><span class="sxs-lookup"><span data-stu-id="e9843-122">String</span></span>|<span data-ttu-id="e9843-123">Mit Kategorie 5 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e9843-123">The label associated with Category 5</span></span>|
|<span data-ttu-id="e9843-124">category6</span><span class="sxs-lookup"><span data-stu-id="e9843-124">category6</span></span>|<span data-ttu-id="e9843-125">String</span><span class="sxs-lookup"><span data-stu-id="e9843-125">String</span></span>|<span data-ttu-id="e9843-126">Mit Kategorie 6 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e9843-126">The label associated with Category 6</span></span>|

## <span data-ttu-id="e9843-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9843-127">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="e9843-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9843-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->