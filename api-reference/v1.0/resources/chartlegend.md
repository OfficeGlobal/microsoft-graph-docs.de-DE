# <a name="chartlegend-resource-type"></a><span data-ttu-id="506ed-101">ChartLegend-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="506ed-101">ChartLegend resource type</span></span>

<span data-ttu-id="506ed-102">Stellt die Legende in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="506ed-102">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="506ed-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="506ed-103">Methods</span></span>

| <span data-ttu-id="506ed-104">Methode</span><span class="sxs-lookup"><span data-stu-id="506ed-104">Method</span></span>           | <span data-ttu-id="506ed-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="506ed-105">Return Type</span></span>    |<span data-ttu-id="506ed-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="506ed-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="506ed-107">ChartLegend abrufen</span><span class="sxs-lookup"><span data-stu-id="506ed-107">Get ChartLegend</span></span>](../api/chartlegend_get.md) | [<span data-ttu-id="506ed-108">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="506ed-108">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="506ed-109">Dient zum Lesen der Eigenschaften und der Beziehungen des chartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="506ed-109">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="506ed-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="506ed-110">Update</span></span>](../api/chartlegend_update.md) | [<span data-ttu-id="506ed-111">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="506ed-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="506ed-112">Dient zum Aktualisieren des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="506ed-112">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="506ed-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="506ed-113">Properties</span></span>
| <span data-ttu-id="506ed-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="506ed-114">Property</span></span>     | <span data-ttu-id="506ed-115">Typ</span><span class="sxs-lookup"><span data-stu-id="506ed-115">Type</span></span>   |<span data-ttu-id="506ed-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="506ed-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="506ed-117">Overlay</span><span class="sxs-lookup"><span data-stu-id="506ed-117">overlay</span></span>|<span data-ttu-id="506ed-118">boolean</span><span class="sxs-lookup"><span data-stu-id="506ed-118">boolean</span></span>|<span data-ttu-id="506ed-119">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="506ed-119">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="506ed-120">Position</span><span class="sxs-lookup"><span data-stu-id="506ed-120">position</span></span>|<span data-ttu-id="506ed-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="506ed-121">string</span></span>|<span data-ttu-id="506ed-122">Gibt die Position der Legende im Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="506ed-122">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="506ed-123">Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="506ed-123">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="506ed-124">visible</span><span class="sxs-lookup"><span data-stu-id="506ed-124">visible</span></span>|<span data-ttu-id="506ed-125">boolean</span><span class="sxs-lookup"><span data-stu-id="506ed-125">boolean</span></span>|<span data-ttu-id="506ed-126">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="506ed-126">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="506ed-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="506ed-127">Relationships</span></span>
| <span data-ttu-id="506ed-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="506ed-128">Relationship</span></span> | <span data-ttu-id="506ed-129">Typ</span><span class="sxs-lookup"><span data-stu-id="506ed-129">Type</span></span>   |<span data-ttu-id="506ed-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="506ed-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="506ed-131">Format</span><span class="sxs-lookup"><span data-stu-id="506ed-131">format</span></span>|[<span data-ttu-id="506ed-132">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="506ed-132">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="506ed-p102">Stellt die Formatierung für eine Diagrammlegende dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="506ed-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="506ed-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="506ed-135">JSON representation</span></span>

<span data-ttu-id="506ed-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="506ed-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->