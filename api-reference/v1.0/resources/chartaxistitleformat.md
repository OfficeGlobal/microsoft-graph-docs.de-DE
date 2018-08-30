# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="272b9-101">ChartAxisTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="272b9-101">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="272b9-102">Stellt die Formatierung des Diagrammachsentitels dar.</span><span class="sxs-lookup"><span data-stu-id="272b9-102">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="272b9-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="272b9-103">Methods</span></span>
<span data-ttu-id="272b9-104">Keine</span><span class="sxs-lookup"><span data-stu-id="272b9-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="272b9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="272b9-105">Properties</span></span>
<span data-ttu-id="272b9-106">Keine</span><span class="sxs-lookup"><span data-stu-id="272b9-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="272b9-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="272b9-107">Relationships</span></span>
| <span data-ttu-id="272b9-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="272b9-108">Relationship</span></span> | <span data-ttu-id="272b9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="272b9-109">Type</span></span>   |<span data-ttu-id="272b9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="272b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="272b9-111">font</span><span class="sxs-lookup"><span data-stu-id="272b9-111">font</span></span>|[<span data-ttu-id="272b9-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="272b9-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="272b9-p101">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. eines Diagrammachsentitel-Objekts dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="272b9-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="272b9-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="272b9-115">JSON representation</span></span>

<span data-ttu-id="272b9-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="272b9-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->