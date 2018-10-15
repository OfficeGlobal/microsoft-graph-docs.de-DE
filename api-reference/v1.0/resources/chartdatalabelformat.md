# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="9dc4e-101">ChartDataLabelFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9dc4e-101">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="9dc4e-102">Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.</span><span class="sxs-lookup"><span data-stu-id="9dc4e-102">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="9dc4e-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="9dc4e-103">Methods</span></span>
<span data-ttu-id="9dc4e-104">Keine</span><span class="sxs-lookup"><span data-stu-id="9dc4e-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="9dc4e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9dc4e-105">Properties</span></span>
<span data-ttu-id="9dc4e-106">Keine</span><span class="sxs-lookup"><span data-stu-id="9dc4e-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9dc4e-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9dc4e-107">Relationships</span></span>
| <span data-ttu-id="9dc4e-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9dc4e-108">Relationship</span></span> | <span data-ttu-id="9dc4e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9dc4e-109">Type</span></span>   |<span data-ttu-id="9dc4e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dc4e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dc4e-111">fill</span><span class="sxs-lookup"><span data-stu-id="9dc4e-111">fill</span></span>|[<span data-ttu-id="9dc4e-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="9dc4e-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="9dc4e-p101">Stellt die Füllung der aktuellen Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9dc4e-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="9dc4e-115">Schriftart</span><span class="sxs-lookup"><span data-stu-id="9dc4e-115">font</span></span>|[<span data-ttu-id="9dc4e-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="9dc4e-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="9dc4e-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für eine Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9dc4e-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9dc4e-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9dc4e-119">JSON representation</span></span>

<span data-ttu-id="9dc4e-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9dc4e-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->