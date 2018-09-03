# <a name="chartpoint-resource-type"></a><span data-ttu-id="7fd10-101">ChartPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7fd10-101">ChartPoint resource type</span></span>

<span data-ttu-id="7fd10-102">Stellt einen Punkt einer Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="7fd10-102">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7fd10-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="7fd10-103">Methods</span></span>

| <span data-ttu-id="7fd10-104">Methode</span><span class="sxs-lookup"><span data-stu-id="7fd10-104">Method</span></span>           | <span data-ttu-id="7fd10-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7fd10-105">Return Type</span></span>    |<span data-ttu-id="7fd10-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7fd10-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7fd10-107">ChartPoint abrufen</span><span class="sxs-lookup"><span data-stu-id="7fd10-107">Get ChartPoint</span></span>](../api/chartpoint_get.md) | [<span data-ttu-id="7fd10-108">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="7fd10-108">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="7fd10-109">Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7fd10-109">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="7fd10-110">Liste</span><span class="sxs-lookup"><span data-stu-id="7fd10-110">List</span></span>](../api/chartpoint_list.md) | <span data-ttu-id="7fd10-111">[WorkbookChartPoint](chartpoint.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7fd10-111">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="7fd10-112">Dient zum Abrufen der chartPoint-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="7fd10-112">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="7fd10-113">ItemAt</span><span class="sxs-lookup"><span data-stu-id="7fd10-113">Itemat</span></span>](../api/chartpointscollection_itemat.md)|[<span data-ttu-id="7fd10-114">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="7fd10-114">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="7fd10-115">Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="7fd10-115">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="7fd10-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7fd10-116">Properties</span></span>
| <span data-ttu-id="7fd10-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7fd10-117">Property</span></span>     | <span data-ttu-id="7fd10-118">Typ</span><span class="sxs-lookup"><span data-stu-id="7fd10-118">Type</span></span>   |<span data-ttu-id="7fd10-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7fd10-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fd10-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7fd10-120">value</span></span>|<span data-ttu-id="7fd10-121">Json</span><span class="sxs-lookup"><span data-stu-id="7fd10-121">Json</span></span>|<span data-ttu-id="7fd10-p101">Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7fd10-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="7fd10-124">id</span><span class="sxs-lookup"><span data-stu-id="7fd10-124">id</span></span>|<span data-ttu-id="7fd10-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7fd10-125">string</span></span>|<span data-ttu-id="7fd10-126">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="7fd10-126">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fd10-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7fd10-127">Relationships</span></span>
| <span data-ttu-id="7fd10-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7fd10-128">Relationship</span></span> | <span data-ttu-id="7fd10-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7fd10-129">Type</span></span>   |<span data-ttu-id="7fd10-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7fd10-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fd10-131">Format</span><span class="sxs-lookup"><span data-stu-id="7fd10-131">format</span></span>|[<span data-ttu-id="7fd10-132">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="7fd10-132">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="7fd10-p102">Kapselt die Formateigenschaften eines Diagrammpunkts ein. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7fd10-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fd10-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7fd10-135">JSON representation</span></span>

<span data-ttu-id="7fd10-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7fd10-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->