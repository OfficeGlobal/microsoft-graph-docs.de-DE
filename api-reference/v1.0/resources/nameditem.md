# <a name="nameditem-resource-type"></a><span data-ttu-id="9c0a0-101">GetNamedItem Ressourcenart</span><span class="sxs-lookup"><span data-stu-id="9c0a0-101">NamedItem resource type</span></span>

<span data-ttu-id="9c0a0-p101">Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="9c0a0-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="9c0a0-105">Methods</span></span>

| <span data-ttu-id="9c0a0-106">Methode</span><span class="sxs-lookup"><span data-stu-id="9c0a0-106">Method</span></span>           | <span data-ttu-id="9c0a0-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9c0a0-107">Return Type</span></span>    |<span data-ttu-id="9c0a0-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c0a0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c0a0-109">Add</span><span class="sxs-lookup"><span data-stu-id="9c0a0-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="9c0a0-110">NamedItem</span><span class="sxs-lookup"><span data-stu-id="9c0a0-110">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="9c0a0-111">Fügt einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="9c0a0-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="9c0a0-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="9c0a0-113">NamedItem</span><span class="sxs-lookup"><span data-stu-id="9c0a0-113">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="9c0a0-114">Fügt unter Verwendung des Gebietsschemas des Benutzers für die Formel einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="9c0a0-115">NamedItem abrufen</span><span class="sxs-lookup"><span data-stu-id="9c0a0-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="9c0a0-116">NamedItem</span><span class="sxs-lookup"><span data-stu-id="9c0a0-116">NamedItem</span></span>](nameditem.md) |<span data-ttu-id="9c0a0-117">Dient zum Lesen der Eigenschaften und der Beziehungen des namedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="9c0a0-118">Update</span><span class="sxs-lookup"><span data-stu-id="9c0a0-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="9c0a0-119">NamedItem</span><span class="sxs-lookup"><span data-stu-id="9c0a0-119">NamedItem</span></span>](nameditem.md)   |<span data-ttu-id="9c0a0-120">Dient zum Aktualisieren des NamedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="9c0a0-121">Range</span><span class="sxs-lookup"><span data-stu-id="9c0a0-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="9c0a0-122">Range</span><span class="sxs-lookup"><span data-stu-id="9c0a0-122">Range</span></span>](range.md)|<span data-ttu-id="9c0a0-p102">Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="9c0a0-125">List</span><span class="sxs-lookup"><span data-stu-id="9c0a0-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="9c0a0-126">[NamedItem-Sammlung](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="9c0a0-126">[NamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="9c0a0-127">Dient zum Abrufen einer der namedItem-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c0a0-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c0a0-128">Properties</span></span>
| <span data-ttu-id="9c0a0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c0a0-129">Property</span></span>     | <span data-ttu-id="9c0a0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9c0a0-130">Type</span></span>   |<span data-ttu-id="9c0a0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c0a0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c0a0-132">name</span><span class="sxs-lookup"><span data-stu-id="9c0a0-132">name</span></span>|<span data-ttu-id="9c0a0-133">string</span><span class="sxs-lookup"><span data-stu-id="9c0a0-133">string</span></span>|<span data-ttu-id="9c0a0-p103">Der Name des Objekts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="9c0a0-136">comment</span><span class="sxs-lookup"><span data-stu-id="9c0a0-136">comment</span></span>|<span data-ttu-id="9c0a0-137">string</span><span class="sxs-lookup"><span data-stu-id="9c0a0-137">string</span></span>|<span data-ttu-id="9c0a0-138">Stellt den Kommentar dar, der mit diesem Namen verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="9c0a0-139">scope</span><span class="sxs-lookup"><span data-stu-id="9c0a0-139">scope</span></span>|<span data-ttu-id="9c0a0-140">string</span><span class="sxs-lookup"><span data-stu-id="9c0a0-140">string</span></span>|<span data-ttu-id="9c0a0-p104">Gibt an, ob der Name im Bereich der Arbeitsmappe oder im Bereich eines bestimmten Arbeitsblatts liegt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="9c0a0-143">type</span><span class="sxs-lookup"><span data-stu-id="9c0a0-143">type</span></span>|<span data-ttu-id="9c0a0-144">string</span><span class="sxs-lookup"><span data-stu-id="9c0a0-144">string</span></span>|<span data-ttu-id="9c0a0-p105">Gibt an, welche Art von Verweis mit dem Namen verknüpft ist. Mögliche Werte:`String`, `Integer`, `Double`, `Boolean`, `Range`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-p105">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="9c0a0-148">value</span><span class="sxs-lookup"><span data-stu-id="9c0a0-148">value</span></span>|<span data-ttu-id="9c0a0-149">object</span><span class="sxs-lookup"><span data-stu-id="9c0a0-149">object</span></span>|<span data-ttu-id="9c0a0-p106">Stellt die Formel dar, auf die der Name verweist. z. B. =Sheet14!$B$2:$H$12, =4.75 usw. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="9c0a0-153">visible</span><span class="sxs-lookup"><span data-stu-id="9c0a0-153">visible</span></span>|<span data-ttu-id="9c0a0-154">boolean</span><span class="sxs-lookup"><span data-stu-id="9c0a0-154">boolean</span></span>|<span data-ttu-id="9c0a0-155">Gibt an, ob das Objekt sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c0a0-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9c0a0-156">Relationships</span></span>
| <span data-ttu-id="9c0a0-157">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9c0a0-157">Relationship</span></span>     | <span data-ttu-id="9c0a0-158">Typ</span><span class="sxs-lookup"><span data-stu-id="9c0a0-158">Type</span></span>   |<span data-ttu-id="9c0a0-159">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c0a0-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c0a0-160">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="9c0a0-160">worksheet</span></span>|[<span data-ttu-id="9c0a0-161">worksheet</span><span class="sxs-lookup"><span data-stu-id="9c0a0-161">worksheet</span></span>](worksheet.md)|<span data-ttu-id="9c0a0-p107">Gibt das Arbeitsblatt zurück, auf dessen Bereich das benannte Element beschränkt ist. Nur verfügbar, wenn das Element auf das Arbeitsblatt beschränkt ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c0a0-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9c0a0-165">JSON representation</span></span>

<span data-ttu-id="9c0a0-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9c0a0-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.range"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
