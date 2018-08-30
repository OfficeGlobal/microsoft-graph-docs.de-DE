# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="9d048-101">ChartSeriesFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9d048-101">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="9d048-102">Kapselt die Formateigenschaften für den Diagrammdatenreihe.</span><span class="sxs-lookup"><span data-stu-id="9d048-102">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="9d048-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="9d048-103">Methods</span></span>
<span data-ttu-id="9d048-104">Keine</span><span class="sxs-lookup"><span data-stu-id="9d048-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="9d048-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9d048-105">Properties</span></span>
<span data-ttu-id="9d048-106">Keine</span><span class="sxs-lookup"><span data-stu-id="9d048-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9d048-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9d048-107">Relationships</span></span>
| <span data-ttu-id="9d048-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9d048-108">Relationship</span></span> | <span data-ttu-id="9d048-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9d048-109">Type</span></span>   |<span data-ttu-id="9d048-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d048-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d048-111">fill</span><span class="sxs-lookup"><span data-stu-id="9d048-111">fill</span></span>|[<span data-ttu-id="9d048-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="9d048-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="9d048-p101">Stellt die Füllung einer Diagrammdatenreihe dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9d048-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="9d048-115">line</span><span class="sxs-lookup"><span data-stu-id="9d048-115">line</span></span>|[<span data-ttu-id="9d048-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="9d048-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="9d048-p102">Die Zeilenformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9d048-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9d048-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9d048-119">JSON representation</span></span>

<span data-ttu-id="9d048-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9d048-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->