# <a name="tablesort-resource-type"></a><span data-ttu-id="490a6-101">TableSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="490a6-101">TableSort resource type</span></span>

<span data-ttu-id="490a6-102">Verwaltet Sortiervorgänge für Table-Objekte.</span><span class="sxs-lookup"><span data-stu-id="490a6-102">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="490a6-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="490a6-103">Methods</span></span>

| <span data-ttu-id="490a6-104">Methode</span><span class="sxs-lookup"><span data-stu-id="490a6-104">Method</span></span>           | <span data-ttu-id="490a6-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="490a6-105">Return Type</span></span>    |<span data-ttu-id="490a6-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="490a6-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="490a6-107">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="490a6-107">Get TableSort</span></span>](../api/tablesort_get.md) | [<span data-ttu-id="490a6-108">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="490a6-108">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="490a6-109">Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.</span><span class="sxs-lookup"><span data-stu-id="490a6-109">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="490a6-110">Anwenden</span><span class="sxs-lookup"><span data-stu-id="490a6-110">Apply</span></span>](../api/tablesort_apply.md)|<span data-ttu-id="490a6-111">Keine</span><span class="sxs-lookup"><span data-stu-id="490a6-111">None</span></span>|<span data-ttu-id="490a6-112">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="490a6-112">Perform a sort operation.</span></span>|
|[<span data-ttu-id="490a6-113">Löschen</span><span class="sxs-lookup"><span data-stu-id="490a6-113">Clear</span></span>](../api/tablesort_clear.md)|<span data-ttu-id="490a6-114">Keine</span><span class="sxs-lookup"><span data-stu-id="490a6-114">None</span></span>|<span data-ttu-id="490a6-p101">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="490a6-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="490a6-117">Reapply</span><span class="sxs-lookup"><span data-stu-id="490a6-117">Reapply</span></span>](../api/tablesort_reapply.md)|<span data-ttu-id="490a6-118">Keine</span><span class="sxs-lookup"><span data-stu-id="490a6-118">None</span></span>|<span data-ttu-id="490a6-119">Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="490a6-119">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="490a6-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="490a6-120">Properties</span></span>
| <span data-ttu-id="490a6-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="490a6-121">Property</span></span>     | <span data-ttu-id="490a6-122">Typ</span><span class="sxs-lookup"><span data-stu-id="490a6-122">Type</span></span>   |<span data-ttu-id="490a6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="490a6-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="490a6-124">fields</span><span class="sxs-lookup"><span data-stu-id="490a6-124">fields</span></span>|<span data-ttu-id="490a6-125">[WorkbookSortField](sortfield.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="490a6-125">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="490a6-p102">Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="490a6-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="490a6-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="490a6-128">matchCase</span></span>|<span data-ttu-id="490a6-129">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="490a6-129">boolean</span></span>|<span data-ttu-id="490a6-p103">Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="490a6-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="490a6-132">method</span><span class="sxs-lookup"><span data-stu-id="490a6-132">method</span></span>|<span data-ttu-id="490a6-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="490a6-133">string</span></span>|<span data-ttu-id="490a6-134">Stellt die Sortiermethode für chinesische Zeichen dar, die zuletzt verwendet wurde, um die Tabelle zu sortieren.</span><span class="sxs-lookup"><span data-stu-id="490a6-134">Represents Chinese character ordering method last used to sort the table. Possible values are: , . Read-only.</span></span> <span data-ttu-id="490a6-135">Die möglichen Werte sind: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="490a6-135">The possible values are:</span></span> <span data-ttu-id="490a6-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="490a6-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="490a6-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="490a6-137">JSON representation</span></span>

<span data-ttu-id="490a6-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="490a6-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->