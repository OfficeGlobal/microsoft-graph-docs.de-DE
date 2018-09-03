# <a name="rangeborder-resource-type"></a><span data-ttu-id="8fcf7-101">RangeBorder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8fcf7-101">RangeBorder resource type</span></span>

<span data-ttu-id="8fcf7-102">Stellt den Rahmen eines Objekts dar.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-102">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="8fcf7-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="8fcf7-103">Methods</span></span>

| <span data-ttu-id="8fcf7-104">Methode</span><span class="sxs-lookup"><span data-stu-id="8fcf7-104">Method</span></span>           | <span data-ttu-id="8fcf7-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8fcf7-105">Return Type</span></span>    |<span data-ttu-id="8fcf7-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fcf7-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8fcf7-107">RangeBorder abrufen</span><span class="sxs-lookup"><span data-stu-id="8fcf7-107">Get RangeBorder</span></span>](../api/rangeborder_get.md) | [<span data-ttu-id="8fcf7-108">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="8fcf7-108">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="8fcf7-109">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeBorder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-109">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="8fcf7-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8fcf7-110">Update</span></span>](../api/rangeborder_update.md) | [<span data-ttu-id="8fcf7-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="8fcf7-111">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="8fcf7-112">Dient zum Aktualisieren des RangeBorder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-112">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="8fcf7-113">Liste</span><span class="sxs-lookup"><span data-stu-id="8fcf7-113">List</span></span>](../api/rangeborder_list.md) | <span data-ttu-id="8fcf7-114">[WorkbookRangeBorder](rangeborder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8fcf7-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="8fcf7-115">Dient zum Abrufen der RangeBorder-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-115">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="8fcf7-116">Itemat</span><span class="sxs-lookup"><span data-stu-id="8fcf7-116">Itemat</span></span>](../api/rangebordercollection_itemat.md)|[<span data-ttu-id="8fcf7-117">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="8fcf7-117">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="8fcf7-118">Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-118">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="8fcf7-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8fcf7-119">Properties</span></span>
| <span data-ttu-id="8fcf7-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fcf7-120">Property</span></span>     | <span data-ttu-id="8fcf7-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8fcf7-121">Type</span></span>   |<span data-ttu-id="8fcf7-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fcf7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fcf7-123">color</span><span class="sxs-lookup"><span data-stu-id="8fcf7-123">color</span></span>|<span data-ttu-id="8fcf7-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fcf7-124">string</span></span>|<span data-ttu-id="8fcf7-125">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="8fcf7-126">id</span><span class="sxs-lookup"><span data-stu-id="8fcf7-126">id</span></span>|<span data-ttu-id="8fcf7-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fcf7-127">string</span></span>|<span data-ttu-id="8fcf7-128">Stellt den Bezeichner des Rahmens dar.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-128">Represents border identifier. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="8fcf7-129">Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-129">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="8fcf7-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-130">Read-only.</span></span>|
|<span data-ttu-id="8fcf7-131">sideIndex</span><span class="sxs-lookup"><span data-stu-id="8fcf7-131">sideIndex</span></span>|<span data-ttu-id="8fcf7-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fcf7-132">string</span></span>|<span data-ttu-id="8fcf7-133">Konstanter Wert, der die bestimmte Seite des Rahmens angibt.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-133">Constant value that indicates the specific side of the border. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="8fcf7-134">Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-134">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="8fcf7-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-135">Read-only.</span></span>|
|<span data-ttu-id="8fcf7-136">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="8fcf7-136">style</span></span>|<span data-ttu-id="8fcf7-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fcf7-137">string</span></span>|<span data-ttu-id="8fcf7-138">Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-138">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="8fcf7-139">Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-139">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="8fcf7-140">weight</span><span class="sxs-lookup"><span data-stu-id="8fcf7-140">weight</span></span>|<span data-ttu-id="8fcf7-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fcf7-141">string</span></span>|<span data-ttu-id="8fcf7-142">Gibt die Stärke des Rahmens um einen Bereich an.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="8fcf7-143">Die möglichen Werte sind: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-143">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fcf7-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8fcf7-144">Relationships</span></span>
<span data-ttu-id="8fcf7-145">Keine</span><span class="sxs-lookup"><span data-stu-id="8fcf7-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8fcf7-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8fcf7-146">JSON representation</span></span>

<span data-ttu-id="8fcf7-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8fcf7-147">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->