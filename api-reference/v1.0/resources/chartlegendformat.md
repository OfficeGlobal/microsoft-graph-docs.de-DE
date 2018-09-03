# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="b8946-101">ChartLegendFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8946-101">ChartLegendFormat resource type</span></span>

<span data-ttu-id="b8946-102">Kapselt die Formateigenschaften einer Diagrammlegende.</span><span class="sxs-lookup"><span data-stu-id="b8946-102">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="b8946-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="b8946-103">Methods</span></span>
<span data-ttu-id="b8946-104">Keine</span><span class="sxs-lookup"><span data-stu-id="b8946-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="b8946-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8946-105">Properties</span></span>
<span data-ttu-id="b8946-106">Keine</span><span class="sxs-lookup"><span data-stu-id="b8946-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b8946-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8946-107">Relationships</span></span>
| <span data-ttu-id="b8946-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b8946-108">Relationship</span></span> | <span data-ttu-id="b8946-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b8946-109">Type</span></span>   |<span data-ttu-id="b8946-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8946-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8946-111">Füll</span><span class="sxs-lookup"><span data-stu-id="b8946-111">fill</span></span>|[<span data-ttu-id="b8946-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="b8946-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="b8946-p101">Stellt das Füllformat eins Objekts dar, einschließlich Informationen über die Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b8946-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="b8946-115">Schriftart</span><span class="sxs-lookup"><span data-stu-id="b8946-115">font</span></span>|[<span data-ttu-id="b8946-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b8946-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b8946-p102">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. einer Diagrammlegende dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b8946-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b8946-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8946-119">JSON representation</span></span>

<span data-ttu-id="b8946-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8946-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->