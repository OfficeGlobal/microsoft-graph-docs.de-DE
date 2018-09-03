# <a name="chartgridlines-resource-type"></a><span data-ttu-id="620f0-101">ChartGridlines-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="620f0-101">ChartGridlines resource type</span></span>

<span data-ttu-id="620f0-102">Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="620f0-102">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="620f0-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="620f0-103">Methods</span></span>

| <span data-ttu-id="620f0-104">Methode</span><span class="sxs-lookup"><span data-stu-id="620f0-104">Method</span></span>           | <span data-ttu-id="620f0-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="620f0-105">Return Type</span></span>    |<span data-ttu-id="620f0-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="620f0-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="620f0-107">ChartGridlines abrufen</span><span class="sxs-lookup"><span data-stu-id="620f0-107">Get ChartGridlines</span></span>](../api/chartgridlines_get.md) | [<span data-ttu-id="620f0-108">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="620f0-108">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="620f0-109">Dient zum Lesen der Eigenschaften und der Beziehungen des chartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="620f0-109">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="620f0-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="620f0-110">Update</span></span>](../api/chartgridlines_update.md) | [<span data-ttu-id="620f0-111">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="620f0-111">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="620f0-112">Dient zum Aktualisieren des ChartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="620f0-112">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="620f0-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="620f0-113">Properties</span></span>
| <span data-ttu-id="620f0-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="620f0-114">Property</span></span>     | <span data-ttu-id="620f0-115">Typ</span><span class="sxs-lookup"><span data-stu-id="620f0-115">Type</span></span>   |<span data-ttu-id="620f0-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="620f0-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="620f0-117">sichtbar</span><span class="sxs-lookup"><span data-stu-id="620f0-117">visible</span></span>|<span data-ttu-id="620f0-118">boolesch</span><span class="sxs-lookup"><span data-stu-id="620f0-118">boolean</span></span>|<span data-ttu-id="620f0-119">Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="620f0-119">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="620f0-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="620f0-120">Relationships</span></span>
| <span data-ttu-id="620f0-121">Beziehung</span><span class="sxs-lookup"><span data-stu-id="620f0-121">Relationship</span></span> | <span data-ttu-id="620f0-122">Typ</span><span class="sxs-lookup"><span data-stu-id="620f0-122">Type</span></span>   |<span data-ttu-id="620f0-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="620f0-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="620f0-124">Format</span><span class="sxs-lookup"><span data-stu-id="620f0-124">format</span></span>|[<span data-ttu-id="620f0-125">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="620f0-125">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="620f0-p101">Stellt die Formatierung der Diagrammgitternetzlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="620f0-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="620f0-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="620f0-128">JSON representation</span></span>

<span data-ttu-id="620f0-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="620f0-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->