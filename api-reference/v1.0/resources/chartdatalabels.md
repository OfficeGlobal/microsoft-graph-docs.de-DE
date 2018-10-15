# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="b1a2a-101">ChartDataLabels-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b1a2a-101">ChartDataLabels resource type</span></span>

<span data-ttu-id="b1a2a-102">Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-102">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="b1a2a-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="b1a2a-103">Methods</span></span>

| <span data-ttu-id="b1a2a-104">Methode</span><span class="sxs-lookup"><span data-stu-id="b1a2a-104">Method</span></span>           | <span data-ttu-id="b1a2a-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b1a2a-105">Return Type</span></span>    |<span data-ttu-id="b1a2a-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1a2a-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1a2a-107">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="b1a2a-107">Get ChartDataLabels</span></span>](../api/chartdatalabels_get.md) | [<span data-ttu-id="b1a2a-108">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="b1a2a-108">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="b1a2a-109">Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-109">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="b1a2a-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b1a2a-110">Update</span></span>](../api/chartdatalabels_update.md) | [<span data-ttu-id="b1a2a-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="b1a2a-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="b1a2a-112">Dient zum Aktualisieren des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-112">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b1a2a-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b1a2a-113">Properties</span></span>
| <span data-ttu-id="b1a2a-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1a2a-114">Property</span></span>     | <span data-ttu-id="b1a2a-115">Typ</span><span class="sxs-lookup"><span data-stu-id="b1a2a-115">Type</span></span>   |<span data-ttu-id="b1a2a-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1a2a-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1a2a-117">position</span><span class="sxs-lookup"><span data-stu-id="b1a2a-117">position</span></span>|<span data-ttu-id="b1a2a-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1a2a-118">string</span></span>|<span data-ttu-id="b1a2a-119">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-119">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="b1a2a-120">Die möglichen Werte sind: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-120">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="b1a2a-121">Separator</span><span class="sxs-lookup"><span data-stu-id="b1a2a-121">separator</span></span>|<span data-ttu-id="b1a2a-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1a2a-122">string</span></span>|<span data-ttu-id="b1a2a-123">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-123">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="b1a2a-124">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="b1a2a-124">showBubbleSize</span></span>|<span data-ttu-id="b1a2a-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b1a2a-125">boolean</span></span>|<span data-ttu-id="b1a2a-126">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-126">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="b1a2a-127">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="b1a2a-127">showCategoryName</span></span>|<span data-ttu-id="b1a2a-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b1a2a-128">boolean</span></span>|<span data-ttu-id="b1a2a-129">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-129">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="b1a2a-130">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="b1a2a-130">showLegendKey</span></span>|<span data-ttu-id="b1a2a-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b1a2a-131">boolean</span></span>|<span data-ttu-id="b1a2a-132">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-132">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="b1a2a-133">showPercentage</span><span class="sxs-lookup"><span data-stu-id="b1a2a-133">showPercentage</span></span>|<span data-ttu-id="b1a2a-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b1a2a-134">boolean</span></span>|<span data-ttu-id="b1a2a-135">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-135">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="b1a2a-136">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="b1a2a-136">showSeriesName</span></span>|<span data-ttu-id="b1a2a-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b1a2a-137">boolean</span></span>|<span data-ttu-id="b1a2a-138">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-138">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="b1a2a-139">showValue</span><span class="sxs-lookup"><span data-stu-id="b1a2a-139">showValue</span></span>|<span data-ttu-id="b1a2a-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b1a2a-140">boolean</span></span>|<span data-ttu-id="b1a2a-141">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-141">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1a2a-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b1a2a-142">Relationships</span></span>
| <span data-ttu-id="b1a2a-143">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b1a2a-143">Relationship</span></span> | <span data-ttu-id="b1a2a-144">Typ</span><span class="sxs-lookup"><span data-stu-id="b1a2a-144">Type</span></span>   |<span data-ttu-id="b1a2a-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1a2a-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1a2a-146">Format</span><span class="sxs-lookup"><span data-stu-id="b1a2a-146">format</span></span>|[<span data-ttu-id="b1a2a-147">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="b1a2a-147">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="b1a2a-p102">Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1a2a-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b1a2a-150">JSON representation</span></span>

<span data-ttu-id="b1a2a-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b1a2a-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->