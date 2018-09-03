# <a name="filter-resource-type"></a><span data-ttu-id="4e353-101">Filter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4e353-101">Filter resource type</span></span>

<span data-ttu-id="4e353-102">Verwaltet das Filtern der Spalte einer Tabelle.</span><span class="sxs-lookup"><span data-stu-id="4e353-102">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="4e353-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="4e353-103">Methods</span></span>

| <span data-ttu-id="4e353-104">Methode</span><span class="sxs-lookup"><span data-stu-id="4e353-104">Method</span></span>           | <span data-ttu-id="4e353-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4e353-105">Return Type</span></span>    |<span data-ttu-id="4e353-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e353-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e353-107">Anwenden</span><span class="sxs-lookup"><span data-stu-id="4e353-107">Apply</span></span>](../api/filter_apply.md)|<span data-ttu-id="4e353-108">Keine</span><span class="sxs-lookup"><span data-stu-id="4e353-108">None</span></span>|<span data-ttu-id="4e353-109">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="4e353-109">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="4e353-110">Löschen</span><span class="sxs-lookup"><span data-stu-id="4e353-110">Clear</span></span>](../api/filter_clear.md)|<span data-ttu-id="4e353-111">Keine</span><span class="sxs-lookup"><span data-stu-id="4e353-111">None</span></span>|<span data-ttu-id="4e353-112">Deaktiviert den Filter für die angegebene Spalte.</span><span class="sxs-lookup"><span data-stu-id="4e353-112">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e353-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e353-113">Properties</span></span>

| <span data-ttu-id="4e353-114">Name</span><span class="sxs-lookup"><span data-stu-id="4e353-114">Name</span></span> | <span data-ttu-id="4e353-115">Typ</span><span class="sxs-lookup"><span data-stu-id="4e353-115">Type</span></span>   |<span data-ttu-id="4e353-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e353-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e353-117">Kriterien</span><span class="sxs-lookup"><span data-stu-id="4e353-117">criteria</span></span>|[<span data-ttu-id="4e353-118">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="4e353-118">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="4e353-p101">Der aktuell angewendete Filter in der angegebenen Spalte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e353-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e353-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e353-121">JSON representation</span></span>

<span data-ttu-id="4e353-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e353-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->