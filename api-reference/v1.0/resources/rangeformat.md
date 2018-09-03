# <a name="rangeformat-resource-type"></a><span data-ttu-id="aa6ac-101">RangeFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aa6ac-101">RangeFormat resource type</span></span>

<span data-ttu-id="aa6ac-102">Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-102">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="aa6ac-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="aa6ac-103">Methods</span></span>

| <span data-ttu-id="aa6ac-104">Methode</span><span class="sxs-lookup"><span data-stu-id="aa6ac-104">Method</span></span>           | <span data-ttu-id="aa6ac-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aa6ac-105">Return Type</span></span>    |<span data-ttu-id="aa6ac-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa6ac-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa6ac-107">RangeFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="aa6ac-107">Get RangeFormat</span></span>](../api/rangeformat_get.md) | [<span data-ttu-id="aa6ac-108">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="aa6ac-108">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="aa6ac-109">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-109">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="aa6ac-110">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="aa6ac-110">Create RangeBorder</span></span>](../api/rangeformat_post_borders.md) |[<span data-ttu-id="aa6ac-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="aa6ac-111">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="aa6ac-112">Dient zum Erstellen eines neues RangeBorder durch Veröffentlichen in der Rahmensammlung.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-112">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="aa6ac-113">Rahmen auflisten</span><span class="sxs-lookup"><span data-stu-id="aa6ac-113">List borders</span></span>](../api/rangeformat_list_borders.md) |<span data-ttu-id="aa6ac-114">[WorkbookRangeBorder](rangeborder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa6ac-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="aa6ac-115">Dient zum Abrufen einer RangeBorder-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-115">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="aa6ac-116">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aa6ac-116">Update</span></span>](../api/rangeformat_update.md) | [<span data-ttu-id="aa6ac-117">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="aa6ac-117">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="aa6ac-118">Dient zum Aktualisieren des RangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-118">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="aa6ac-119">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="aa6ac-119">Autofitcolumns</span></span>](../api/rangeformat_autofitcolumns.md)|<span data-ttu-id="aa6ac-120">Keine</span><span class="sxs-lookup"><span data-stu-id="aa6ac-120">None</span></span>|<span data-ttu-id="aa6ac-121">Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-121">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="aa6ac-122">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="aa6ac-122">Autofitrows</span></span>](../api/rangeformat_autofitrows.md)|<span data-ttu-id="aa6ac-123">Keine</span><span class="sxs-lookup"><span data-stu-id="aa6ac-123">None</span></span>|<span data-ttu-id="aa6ac-124">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-124">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa6ac-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa6ac-125">Properties</span></span>
| <span data-ttu-id="aa6ac-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa6ac-126">Property</span></span>     | <span data-ttu-id="aa6ac-127">Typ</span><span class="sxs-lookup"><span data-stu-id="aa6ac-127">Type</span></span>   |<span data-ttu-id="aa6ac-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa6ac-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa6ac-129">columnWidth</span><span class="sxs-lookup"><span data-stu-id="aa6ac-129">columnWidth</span></span>|<span data-ttu-id="aa6ac-130">double</span><span class="sxs-lookup"><span data-stu-id="aa6ac-130">double</span></span>|<span data-ttu-id="aa6ac-p101">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="aa6ac-133">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="aa6ac-133">horizontalAlignment</span></span>|<span data-ttu-id="aa6ac-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa6ac-134">string</span></span>|<span data-ttu-id="aa6ac-135">Stellt die horizontale Ausrichtung für das angegebene Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-135">Returns or sets the horizontal alignment for the specified object.</span></span> <span data-ttu-id="aa6ac-136">Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-136">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="aa6ac-137">rowHeight</span><span class="sxs-lookup"><span data-stu-id="aa6ac-137">rowHeight</span></span>|<span data-ttu-id="aa6ac-138">double</span><span class="sxs-lookup"><span data-stu-id="aa6ac-138">double</span></span>|<span data-ttu-id="aa6ac-p103">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="aa6ac-141">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="aa6ac-141">verticalAlignment</span></span>|<span data-ttu-id="aa6ac-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa6ac-142">string</span></span>|<span data-ttu-id="aa6ac-143">Stellt die vertikale Ausrichtung für das angegebene Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-143">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="aa6ac-144">Mögliche Werte sind: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-144">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="aa6ac-145">wrapText</span><span class="sxs-lookup"><span data-stu-id="aa6ac-145">wrapText</span></span>|<span data-ttu-id="aa6ac-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="aa6ac-146">boolean</span></span>|<span data-ttu-id="aa6ac-p105">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="aa6ac-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa6ac-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aa6ac-149">Relationships</span></span>
| <span data-ttu-id="aa6ac-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="aa6ac-150">Relationship</span></span> | <span data-ttu-id="aa6ac-151">Typ</span><span class="sxs-lookup"><span data-stu-id="aa6ac-151">Type</span></span>   |<span data-ttu-id="aa6ac-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa6ac-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa6ac-153">Borders</span><span class="sxs-lookup"><span data-stu-id="aa6ac-153">borders</span></span>|<span data-ttu-id="aa6ac-154">[WorkbookRangeBorder](rangeborder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa6ac-154">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="aa6ac-155">Auflistung von Border-Objekten, die für den gesamten ausgewählten Bereich gelten, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-155">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="aa6ac-156">fill</span><span class="sxs-lookup"><span data-stu-id="aa6ac-156">fill</span></span>|[<span data-ttu-id="aa6ac-157">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="aa6ac-157">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="aa6ac-p106">Gibt das Fill-Objekt an, das für den gesamten Bereich definiert ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="aa6ac-160">Schriftart</span><span class="sxs-lookup"><span data-stu-id="aa6ac-160">font</span></span>|[<span data-ttu-id="aa6ac-161">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="aa6ac-161">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="aa6ac-162">Gibt das Font-Objekt zurück, das für den gesamten ausgewählten Bereich definiert ist, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-162">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="aa6ac-163">protection</span><span class="sxs-lookup"><span data-stu-id="aa6ac-163">protection</span></span>|[<span data-ttu-id="aa6ac-164">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="aa6ac-164">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="aa6ac-p107">Gibt das Formatschutz-Objekt für einen Bereich zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa6ac-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa6ac-167">JSON representation</span></span>

<span data-ttu-id="aa6ac-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa6ac-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->