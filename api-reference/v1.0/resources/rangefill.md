# <a name="rangefill-resource-type"></a><span data-ttu-id="43bd2-101">RangeFill-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="43bd2-101">RangeFill resource type</span></span>

<span data-ttu-id="43bd2-102">Stellt den Hintergrund eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="43bd2-102">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="43bd2-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="43bd2-103">Methods</span></span>

| <span data-ttu-id="43bd2-104">Methode</span><span class="sxs-lookup"><span data-stu-id="43bd2-104">Method</span></span>           | <span data-ttu-id="43bd2-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="43bd2-105">Return Type</span></span>    |<span data-ttu-id="43bd2-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43bd2-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43bd2-107">RangeFill abrufen</span><span class="sxs-lookup"><span data-stu-id="43bd2-107">Get RangeFill</span></span>](../api/rangefill_get.md) | [<span data-ttu-id="43bd2-108">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="43bd2-108">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="43bd2-109">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43bd2-109">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="43bd2-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="43bd2-110">Update</span></span>](../api/rangefill_update.md) | [<span data-ttu-id="43bd2-111">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="43bd2-111">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="43bd2-112">Dient zum Aktualisieren des RangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43bd2-112">Update RangeFill object.</span></span> |
|[<span data-ttu-id="43bd2-113">Löschen</span><span class="sxs-lookup"><span data-stu-id="43bd2-113">Clear</span></span>](../api/rangefill_clear.md)|<span data-ttu-id="43bd2-114">Keine</span><span class="sxs-lookup"><span data-stu-id="43bd2-114">None</span></span>|<span data-ttu-id="43bd2-115">Setzt den Hintergrund des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="43bd2-115">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="43bd2-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="43bd2-116">Properties</span></span>
| <span data-ttu-id="43bd2-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43bd2-117">Property</span></span>     | <span data-ttu-id="43bd2-118">Typ</span><span class="sxs-lookup"><span data-stu-id="43bd2-118">Type</span></span>   |<span data-ttu-id="43bd2-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43bd2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43bd2-120">Farbe</span><span class="sxs-lookup"><span data-stu-id="43bd2-120">color</span></span>|<span data-ttu-id="43bd2-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43bd2-121">string</span></span>|<span data-ttu-id="43bd2-122">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.</span><span class="sxs-lookup"><span data-stu-id="43bd2-122">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="43bd2-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="43bd2-123">Relationships</span></span>
<span data-ttu-id="43bd2-124">Keine</span><span class="sxs-lookup"><span data-stu-id="43bd2-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="43bd2-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="43bd2-125">JSON representation</span></span>

<span data-ttu-id="43bd2-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="43bd2-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->