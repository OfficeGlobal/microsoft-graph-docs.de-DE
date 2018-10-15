# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="163e5-101">ChartAxisTitle-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="163e5-101">ChartAxisTitle resource type</span></span>

<span data-ttu-id="163e5-102">Stellt den Titel einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="163e5-102">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="163e5-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="163e5-103">Methods</span></span>

| <span data-ttu-id="163e5-104">Methode</span><span class="sxs-lookup"><span data-stu-id="163e5-104">Method</span></span>           | <span data-ttu-id="163e5-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="163e5-105">Return Type</span></span>    |<span data-ttu-id="163e5-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="163e5-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="163e5-107">ChartAxisTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="163e5-107">Get ChartAxisTitle</span></span>](../api/chartaxistitle_get.md) | [<span data-ttu-id="163e5-108">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="163e5-108">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="163e5-109">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="163e5-109">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="163e5-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="163e5-110">Update</span></span>](../api/chartaxistitle_update.md) | [<span data-ttu-id="163e5-111">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="163e5-111">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="163e5-112">Dient zum Aktualisieren de chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="163e5-112">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="163e5-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="163e5-113">Properties</span></span>
| <span data-ttu-id="163e5-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="163e5-114">Property</span></span>     | <span data-ttu-id="163e5-115">Typ</span><span class="sxs-lookup"><span data-stu-id="163e5-115">Type</span></span>   |<span data-ttu-id="163e5-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="163e5-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="163e5-117">Text</span><span class="sxs-lookup"><span data-stu-id="163e5-117">text</span></span>|<span data-ttu-id="163e5-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="163e5-118">string</span></span>|<span data-ttu-id="163e5-119">Stellt den Achsentitel dar.</span><span class="sxs-lookup"><span data-stu-id="163e5-119">Represents the axis title.</span></span>|
|<span data-ttu-id="163e5-120">sichtbar</span><span class="sxs-lookup"><span data-stu-id="163e5-120">visible</span></span>|<span data-ttu-id="163e5-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="163e5-121">boolean</span></span>|<span data-ttu-id="163e5-122">Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.</span><span class="sxs-lookup"><span data-stu-id="163e5-122">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="163e5-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="163e5-123">Relationships</span></span>
| <span data-ttu-id="163e5-124">Beziehung</span><span class="sxs-lookup"><span data-stu-id="163e5-124">Relationship</span></span> | <span data-ttu-id="163e5-125">Typ</span><span class="sxs-lookup"><span data-stu-id="163e5-125">Type</span></span>   |<span data-ttu-id="163e5-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="163e5-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="163e5-127">Format</span><span class="sxs-lookup"><span data-stu-id="163e5-127">format</span></span>|[<span data-ttu-id="163e5-128">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="163e5-128">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="163e5-p101">Stellt die Formatierung des Diagrammachsentitels dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="163e5-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="163e5-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="163e5-131">JSON representation</span></span>

<span data-ttu-id="163e5-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="163e5-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->