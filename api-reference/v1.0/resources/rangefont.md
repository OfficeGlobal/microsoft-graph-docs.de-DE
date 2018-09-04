# <a name="rangefont-resource-type"></a><span data-ttu-id="93302-101">RangeFont-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93302-101">RangeFont resource type</span></span>

<span data-ttu-id="93302-102">Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="93302-102">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="93302-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="93302-103">Methods</span></span>

| <span data-ttu-id="93302-104">Methode</span><span class="sxs-lookup"><span data-stu-id="93302-104">Method</span></span>           | <span data-ttu-id="93302-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="93302-105">Return Type</span></span>    |<span data-ttu-id="93302-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93302-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93302-107">RangeFont abrufen</span><span class="sxs-lookup"><span data-stu-id="93302-107">Get RangeFont</span></span>](../api/rangefont_get.md) | [<span data-ttu-id="93302-108">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="93302-108">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="93302-109">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="93302-109">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="93302-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="93302-110">Update</span></span>](../api/rangefont_update.md) | [<span data-ttu-id="93302-111">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="93302-111">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="93302-112">Dient zum Aktualisieren des RangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="93302-112">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="93302-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93302-113">Properties</span></span>
| <span data-ttu-id="93302-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93302-114">Property</span></span>     | <span data-ttu-id="93302-115">Typ</span><span class="sxs-lookup"><span data-stu-id="93302-115">Type</span></span>   |<span data-ttu-id="93302-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93302-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93302-117">fett</span><span class="sxs-lookup"><span data-stu-id="93302-117">bold</span></span>|<span data-ttu-id="93302-118">boolesch</span><span class="sxs-lookup"><span data-stu-id="93302-118">boolean</span></span>|<span data-ttu-id="93302-119">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="93302-119">Represents the bold status of font.</span></span>|
|<span data-ttu-id="93302-120">Farbe</span><span class="sxs-lookup"><span data-stu-id="93302-120">color</span></span>|<span data-ttu-id="93302-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93302-121">string</span></span>|<span data-ttu-id="93302-p101">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="93302-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="93302-125">kursiv</span><span class="sxs-lookup"><span data-stu-id="93302-125">italic</span></span>|<span data-ttu-id="93302-126">boolesch</span><span class="sxs-lookup"><span data-stu-id="93302-126">boolean</span></span>|<span data-ttu-id="93302-127">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="93302-127">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="93302-128">Name</span><span class="sxs-lookup"><span data-stu-id="93302-128">name</span></span>|<span data-ttu-id="93302-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93302-129">string</span></span>|<span data-ttu-id="93302-130">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="93302-130">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="93302-131">Größe</span><span class="sxs-lookup"><span data-stu-id="93302-131">size</span></span>|<span data-ttu-id="93302-132">doppelt</span><span class="sxs-lookup"><span data-stu-id="93302-132">double</span></span>|<span data-ttu-id="93302-133">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="93302-133">Font size.</span></span>|
|<span data-ttu-id="93302-134">unterstrichen</span><span class="sxs-lookup"><span data-stu-id="93302-134">underline</span></span>|<span data-ttu-id="93302-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93302-135">string</span></span>|<span data-ttu-id="93302-136">Art der Unterstreichung für die Schriftart.</span><span class="sxs-lookup"><span data-stu-id="93302-136">Type of underline applied to the font. Possible values are: , .</span></span> <span data-ttu-id="93302-137">Mögliche Werte sind: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="93302-137">The possible values are `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`, , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="93302-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="93302-138">Relationships</span></span>
<span data-ttu-id="93302-139">Keine</span><span class="sxs-lookup"><span data-stu-id="93302-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="93302-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93302-140">JSON representation</span></span>

<span data-ttu-id="93302-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93302-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->