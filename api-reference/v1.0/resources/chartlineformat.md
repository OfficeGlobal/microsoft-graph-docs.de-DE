# <a name="chartlineformat-resource-type"></a><span data-ttu-id="deb0e-101">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="deb0e-101">ChartLineFormat resource type</span></span>

<span data-ttu-id="deb0e-102">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="deb0e-102">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="deb0e-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="deb0e-103">Methods</span></span>

| <span data-ttu-id="deb0e-104">Methode</span><span class="sxs-lookup"><span data-stu-id="deb0e-104">Method</span></span>           | <span data-ttu-id="deb0e-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="deb0e-105">Return Type</span></span>    |<span data-ttu-id="deb0e-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="deb0e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="deb0e-107">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="deb0e-107">Get ChartLineFormat</span></span>](../api/chartlineformat_get.md) | [<span data-ttu-id="deb0e-108">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="deb0e-108">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="deb0e-109">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="deb0e-109">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="deb0e-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="deb0e-110">Update</span></span>](../api/chartlineformat_update.md) | [<span data-ttu-id="deb0e-111">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="deb0e-111">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="deb0e-112">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="deb0e-112">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="deb0e-113">Löschen</span><span class="sxs-lookup"><span data-stu-id="deb0e-113">Clear</span></span>](../api/chartlineformat_clear.md)|<span data-ttu-id="deb0e-114">Keine</span><span class="sxs-lookup"><span data-stu-id="deb0e-114">None</span></span>|<span data-ttu-id="deb0e-115">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="deb0e-115">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="deb0e-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="deb0e-116">Properties</span></span>
| <span data-ttu-id="deb0e-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="deb0e-117">Property</span></span>     | <span data-ttu-id="deb0e-118">Typ</span><span class="sxs-lookup"><span data-stu-id="deb0e-118">Type</span></span>   |<span data-ttu-id="deb0e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="deb0e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deb0e-120">Farbe</span><span class="sxs-lookup"><span data-stu-id="deb0e-120">color</span></span>|<span data-ttu-id="deb0e-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="deb0e-121">string</span></span>|<span data-ttu-id="deb0e-122">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="deb0e-122">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="deb0e-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="deb0e-123">Relationships</span></span>
<span data-ttu-id="deb0e-124">Keine</span><span class="sxs-lookup"><span data-stu-id="deb0e-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="deb0e-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="deb0e-125">JSON representation</span></span>

<span data-ttu-id="deb0e-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="deb0e-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->