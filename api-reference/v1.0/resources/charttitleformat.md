# <a name="charttitleformat-resource-type"></a><span data-ttu-id="23099-101">ChartTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23099-101">ChartTitleFormat resource type</span></span>

<span data-ttu-id="23099-102">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="23099-102">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="23099-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="23099-103">Methods</span></span>
<span data-ttu-id="23099-104">Keine</span><span class="sxs-lookup"><span data-stu-id="23099-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="23099-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23099-105">Properties</span></span>
<span data-ttu-id="23099-106">Keine</span><span class="sxs-lookup"><span data-stu-id="23099-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="23099-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23099-107">Relationships</span></span>
| <span data-ttu-id="23099-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="23099-108">Relationship</span></span> | <span data-ttu-id="23099-109">Typ</span><span class="sxs-lookup"><span data-stu-id="23099-109">Type</span></span>   |<span data-ttu-id="23099-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23099-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23099-111">fill</span><span class="sxs-lookup"><span data-stu-id="23099-111">fill</span></span>|[<span data-ttu-id="23099-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="23099-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="23099-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="23099-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="23099-115">Schriftart</span><span class="sxs-lookup"><span data-stu-id="23099-115">font</span></span>|[<span data-ttu-id="23099-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="23099-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="23099-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="23099-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="23099-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23099-119">JSON representation</span></span>

<span data-ttu-id="23099-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23099-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
