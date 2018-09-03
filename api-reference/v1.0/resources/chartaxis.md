# <a name="chartaxis-resource-type"></a><span data-ttu-id="aa8e2-101">ChartAxis-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aa8e2-101">ChartAxis resource type</span></span>

<span data-ttu-id="aa8e2-102">Stellt eine einzelne Achse in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-102">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="aa8e2-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="aa8e2-103">Methods</span></span>

| <span data-ttu-id="aa8e2-104">Methode</span><span class="sxs-lookup"><span data-stu-id="aa8e2-104">Method</span></span>           | <span data-ttu-id="aa8e2-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aa8e2-105">Return Type</span></span>    |<span data-ttu-id="aa8e2-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa8e2-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa8e2-107">ChartAxis abrufen</span><span class="sxs-lookup"><span data-stu-id="aa8e2-107">Get ChartAxis</span></span>](../api/chartaxis_get.md) | [<span data-ttu-id="aa8e2-108">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="aa8e2-108">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="aa8e2-109">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-109">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="aa8e2-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aa8e2-110">Update</span></span>](../api/chartaxis_update.md) | [<span data-ttu-id="aa8e2-111">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="aa8e2-111">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="aa8e2-112">Dient zum Aktualisieren des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-112">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa8e2-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa8e2-113">Properties</span></span>
| <span data-ttu-id="aa8e2-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa8e2-114">Property</span></span>     | <span data-ttu-id="aa8e2-115">Typ</span><span class="sxs-lookup"><span data-stu-id="aa8e2-115">Type</span></span>   |<span data-ttu-id="aa8e2-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa8e2-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa8e2-117">ID</span><span class="sxs-lookup"><span data-stu-id="aa8e2-117">id</span></span>       |<span data-ttu-id="aa8e2-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa8e2-118">string</span></span>   | <span data-ttu-id="aa8e2-119">Eindeutige Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-119">Unique Identifier</span></span> <span data-ttu-id="aa8e2-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-120">Read-only.</span></span>|
|<span data-ttu-id="aa8e2-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="aa8e2-121">majorUnit</span></span>|<span data-ttu-id="aa8e2-122">Json</span><span class="sxs-lookup"><span data-stu-id="aa8e2-122">Json</span></span>|<span data-ttu-id="aa8e2-p102">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="aa8e2-126">Maximum</span><span class="sxs-lookup"><span data-stu-id="aa8e2-126">maximum</span></span>|<span data-ttu-id="aa8e2-127">Json</span><span class="sxs-lookup"><span data-stu-id="aa8e2-127">Json</span></span>|<span data-ttu-id="aa8e2-p103">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="aa8e2-131">Minimum</span><span class="sxs-lookup"><span data-stu-id="aa8e2-131">minimum</span></span>|<span data-ttu-id="aa8e2-132">Json</span><span class="sxs-lookup"><span data-stu-id="aa8e2-132">Json</span></span>|<span data-ttu-id="aa8e2-p104">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="aa8e2-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="aa8e2-136">minorUnit</span></span>|<span data-ttu-id="aa8e2-137">Json</span><span class="sxs-lookup"><span data-stu-id="aa8e2-137">Json</span></span>|<span data-ttu-id="aa8e2-p105">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa8e2-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aa8e2-141">Relationships</span></span>
| <span data-ttu-id="aa8e2-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="aa8e2-142">Relationship</span></span> | <span data-ttu-id="aa8e2-143">Typ</span><span class="sxs-lookup"><span data-stu-id="aa8e2-143">Type</span></span>   |<span data-ttu-id="aa8e2-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa8e2-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa8e2-145">Format</span><span class="sxs-lookup"><span data-stu-id="aa8e2-145">format</span></span>|[<span data-ttu-id="aa8e2-146">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="aa8e2-146">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="aa8e2-p106">Stellt die Formatierung für ein Diagrammobjekt dar, einschließlich Linien- und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="aa8e2-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="aa8e2-149">majorGridlines</span></span>|[<span data-ttu-id="aa8e2-150">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="aa8e2-150">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="aa8e2-p107">Gibt ein Gitternetzlinien-Objekt zurück, das die Hauptgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="aa8e2-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="aa8e2-153">minorGridlines</span></span>|[<span data-ttu-id="aa8e2-154">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="aa8e2-154">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="aa8e2-p108">Gibt ein Gitternetzlinien-Objekt zurück, das die Hilfsgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="aa8e2-157">Titel</span><span class="sxs-lookup"><span data-stu-id="aa8e2-157">title</span></span>|[<span data-ttu-id="aa8e2-158">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="aa8e2-158">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="aa8e2-p109">Stellt den Achsentitel dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa8e2-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa8e2-161">JSON representation</span></span>

<span data-ttu-id="aa8e2-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa8e2-162">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->