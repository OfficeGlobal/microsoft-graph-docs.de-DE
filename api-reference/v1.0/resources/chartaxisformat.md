# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="40445-101">ChartAxisFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="40445-101">ChartAxisFormat resource type</span></span>

<span data-ttu-id="40445-102">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="40445-102">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="40445-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="40445-103">Methods</span></span>
<span data-ttu-id="40445-104">Keine</span><span class="sxs-lookup"><span data-stu-id="40445-104">None</span></span>
## <a name="properties"></a><span data-ttu-id="40445-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40445-105">Properties</span></span>
<span data-ttu-id="40445-106">Keine</span><span class="sxs-lookup"><span data-stu-id="40445-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="40445-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="40445-107">Relationships</span></span>
| <span data-ttu-id="40445-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="40445-108">Relationship</span></span> | <span data-ttu-id="40445-109">Typ</span><span class="sxs-lookup"><span data-stu-id="40445-109">Type</span></span>   |<span data-ttu-id="40445-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40445-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40445-111">Schriftart</span><span class="sxs-lookup"><span data-stu-id="40445-111">font</span></span>|[<span data-ttu-id="40445-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="40445-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="40445-p101">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammachsenelement dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40445-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="40445-115">Linie</span><span class="sxs-lookup"><span data-stu-id="40445-115">line</span></span>|[<span data-ttu-id="40445-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="40445-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="40445-p102">Stellt die Formatierung der Diagrammlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40445-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="40445-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40445-119">JSON representation</span></span>

<span data-ttu-id="40445-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="40445-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->