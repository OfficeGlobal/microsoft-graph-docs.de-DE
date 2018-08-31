# <a name="sortfield-resource-type"></a><span data-ttu-id="8973b-101">SortField-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8973b-101">SortField resource type</span></span>

<span data-ttu-id="8973b-102">Stellt eine Bedingung in einem Sortiervorgang dar.</span><span class="sxs-lookup"><span data-stu-id="8973b-102">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="8973b-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8973b-103">Properties</span></span>
| <span data-ttu-id="8973b-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8973b-104">Property</span></span>     | <span data-ttu-id="8973b-105">Typ</span><span class="sxs-lookup"><span data-stu-id="8973b-105">Type</span></span>   |<span data-ttu-id="8973b-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8973b-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8973b-107">aufsteigend</span><span class="sxs-lookup"><span data-stu-id="8973b-107">ascending</span></span>|<span data-ttu-id="8973b-108">boolesch</span><span class="sxs-lookup"><span data-stu-id="8973b-108">boolean</span></span>|<span data-ttu-id="8973b-109">Stellt dar, ob die Sortierung in aufsteigender Reihenfolge ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="8973b-109">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="8973b-110">Farbe</span><span class="sxs-lookup"><span data-stu-id="8973b-110">color</span></span>|<span data-ttu-id="8973b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8973b-111">string</span></span>|<span data-ttu-id="8973b-112">Stellt die Farbe dar, die das Ziel der Bedingung ist, wenn die Sortierung für die Schrift- oder Zellenfarbe gilt.</span><span class="sxs-lookup"><span data-stu-id="8973b-112">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="8973b-113">dataOption</span><span class="sxs-lookup"><span data-stu-id="8973b-113">dataOption</span></span>|<span data-ttu-id="8973b-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8973b-114">string</span></span>|<span data-ttu-id="8973b-115">Stellt weitere Sortieroptionen für dieses Feld dar.</span><span class="sxs-lookup"><span data-stu-id="8973b-115">Represents additional sorting options for this field. Possible values are: , .</span></span> <span data-ttu-id="8973b-116">Mögliche Werte sind: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="8973b-116">The possible values are:</span></span>|
|<span data-ttu-id="8973b-117">Schlüssel</span><span class="sxs-lookup"><span data-stu-id="8973b-117">key</span></span>|<span data-ttu-id="8973b-118">int</span><span class="sxs-lookup"><span data-stu-id="8973b-118">int</span></span>|<span data-ttu-id="8973b-p102">Stellt die Spalte (oder Zeile, je nach Sortierausrichtung) dar, für die die Bedingung gilt. Wird als Offset von der ersten Spalte (oder Zeile) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="8973b-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="8973b-121">sortOn</span><span class="sxs-lookup"><span data-stu-id="8973b-121">sortOn</span></span>|<span data-ttu-id="8973b-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8973b-122">string</span></span>|<span data-ttu-id="8973b-123">Stellt den Typ der Sortierung dieser Bedingung dar.</span><span class="sxs-lookup"><span data-stu-id="8973b-123">Represents the type of sorting of this condition. Possible values are: , , , .</span></span> <span data-ttu-id="8973b-124">Mögliche Werte sind: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="8973b-124">The possible values are `Value`, `CellColor`, `FontColor`, `Icon`, , , , , , , , or .</span></span>|
|<span data-ttu-id="8973b-125">Symbol</span><span class="sxs-lookup"><span data-stu-id="8973b-125">icon</span></span>|[<span data-ttu-id="8973b-126">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="8973b-126">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="8973b-127">Stellt das Symbol dar, welches das Ziel der Bedingung ist, wenn die Sortierung für das Symbol der Zelle gilt.</span><span class="sxs-lookup"><span data-stu-id="8973b-127">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8973b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8973b-128">JSON representation</span></span>

<span data-ttu-id="8973b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8973b-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->