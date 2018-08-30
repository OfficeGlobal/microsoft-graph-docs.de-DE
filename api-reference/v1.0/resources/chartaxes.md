# <a name="chartaxes-resource-type"></a><span data-ttu-id="d19dc-101">ChartAxes-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d19dc-101">ChartAxes resource type</span></span>

<span data-ttu-id="d19dc-102">Die Achsen des Diagramms.</span><span class="sxs-lookup"><span data-stu-id="d19dc-102">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="d19dc-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="d19dc-103">Methods</span></span>
<span data-ttu-id="d19dc-104">Keine</span><span class="sxs-lookup"><span data-stu-id="d19dc-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="d19dc-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d19dc-105">Properties</span></span>
<span data-ttu-id="d19dc-106">Keine</span><span class="sxs-lookup"><span data-stu-id="d19dc-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d19dc-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d19dc-107">Relationships</span></span>
| <span data-ttu-id="d19dc-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d19dc-108">Relationship</span></span> | <span data-ttu-id="d19dc-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d19dc-109">Type</span></span>   |<span data-ttu-id="d19dc-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d19dc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d19dc-111">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="d19dc-111">categoryAxis</span></span>|[<span data-ttu-id="d19dc-112">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="d19dc-112">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="d19dc-p101">Stellt die Rubrikenachse in einem Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d19dc-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="d19dc-115">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="d19dc-115">seriesAxis</span></span>|[<span data-ttu-id="d19dc-116">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="d19dc-116">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="d19dc-p102">Stellt die Reihenachse eines dreidimensionalen Diagramms dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d19dc-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="d19dc-119">valueAxis</span><span class="sxs-lookup"><span data-stu-id="d19dc-119">valueAxis</span></span>|[<span data-ttu-id="d19dc-120">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="d19dc-120">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="d19dc-p103">Stellt die Größenachse in einer Achse dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d19dc-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d19dc-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d19dc-123">JSON representation</span></span>

<span data-ttu-id="d19dc-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d19dc-124">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->