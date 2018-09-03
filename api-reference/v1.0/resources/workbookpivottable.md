# <a name="pivottable-resource-type"></a><span data-ttu-id="fdba0-101">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="fdba0-101">pivotTable resource type</span></span>

<span data-ttu-id="fdba0-102">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="fdba0-102">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="fdba0-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="fdba0-103">Methods</span></span>

| <span data-ttu-id="fdba0-104">Methode</span><span class="sxs-lookup"><span data-stu-id="fdba0-104">Method</span></span>           | <span data-ttu-id="fdba0-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fdba0-105">Return Type</span></span>    |<span data-ttu-id="fdba0-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdba0-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdba0-107">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="fdba0-107">Get workbookPivotTable</span></span>](../api/workbookpivottable_get.md) | [<span data-ttu-id="fdba0-108">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="fdba0-108">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="fdba0-109">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdba0-109">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="fdba0-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fdba0-110">Refresh</span></span>](../api/workbookpivottable_refresh.md)|<span data-ttu-id="fdba0-111">Keine</span><span class="sxs-lookup"><span data-stu-id="fdba0-111">None</span></span>|<span data-ttu-id="fdba0-112">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="fdba0-112">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="fdba0-113">Refreshall</span><span class="sxs-lookup"><span data-stu-id="fdba0-113">Refreshall</span></span>](../api/workbookpivottable_refreshall.md)|<span data-ttu-id="fdba0-114">Keine</span><span class="sxs-lookup"><span data-stu-id="fdba0-114">None</span></span>|<span data-ttu-id="fdba0-p101">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="fdba0-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdba0-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdba0-117">Properties</span></span>
| <span data-ttu-id="fdba0-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdba0-118">Property</span></span>     | <span data-ttu-id="fdba0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fdba0-119">Type</span></span>   |<span data-ttu-id="fdba0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdba0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdba0-121">id</span><span class="sxs-lookup"><span data-stu-id="fdba0-121">id</span></span>|<span data-ttu-id="fdba0-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fdba0-122">String</span></span>| <span data-ttu-id="fdba0-p102">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fdba0-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="fdba0-125">Name</span><span class="sxs-lookup"><span data-stu-id="fdba0-125">name</span></span>|<span data-ttu-id="fdba0-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fdba0-126">String</span></span>|<span data-ttu-id="fdba0-127">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="fdba0-127">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="fdba0-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdba0-128">Relationships</span></span>
| <span data-ttu-id="fdba0-129">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fdba0-129">Relationship</span></span> | <span data-ttu-id="fdba0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fdba0-130">Type</span></span>   |<span data-ttu-id="fdba0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdba0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdba0-132">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="fdba0-132">worksheet</span></span>|[<span data-ttu-id="fdba0-133">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="fdba0-133">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="fdba0-p103">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fdba0-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="fdba0-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdba0-136">JSON representation</span></span>
<span data-ttu-id="fdba0-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdba0-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
