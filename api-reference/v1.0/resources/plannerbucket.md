# <a name="plannerbucket-resource-type"></a><span data-ttu-id="36546-101">plannerBucket-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="36546-101">plannerBucket resource type</span></span>

<span data-ttu-id="36546-p101">Die **plannerBucket**-Ressource stellt einen Bucket (bzw. eine „benutzerdefinierte Spalte“) für Aufgaben in einem Plan in Office 365 dar. Sie ist in einem [plannerPlan](plannerPlan.md) enthalten und kann eine Sammlung von [plannerTasks](plannerTask.md) haben.</span><span class="sxs-lookup"><span data-stu-id="36546-p101">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerPlan.md) and can have a collection of [plannerTasks](plannerTask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="36546-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="36546-104">Methods</span></span>

| <span data-ttu-id="36546-105">Methode</span><span class="sxs-lookup"><span data-stu-id="36546-105">Method</span></span>           | <span data-ttu-id="36546-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="36546-106">Return Type</span></span>    |<span data-ttu-id="36546-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36546-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36546-108">plannerBucket abrufen</span><span class="sxs-lookup"><span data-stu-id="36546-108">Get plannerBucket</span></span>](../api/plannerbucket_get.md) | [<span data-ttu-id="36546-109">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="36546-109">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="36546-110">Dient zum Lesen der Eigenschaften und Beziehungen des **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="36546-110">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="36546-111">plannerTasks auflisten</span><span class="sxs-lookup"><span data-stu-id="36546-111">List plannerTasks</span></span>](../api/plannerbucket_list_tasks.md) |<span data-ttu-id="36546-112">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="36546-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="36546-113">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="36546-113">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="36546-114">Erstellen</span><span class="sxs-lookup"><span data-stu-id="36546-114">Create</span></span>](../api/planner_post_buckets.md) | [<span data-ttu-id="36546-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="36546-115">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="36546-116">Dient zum Erstellen eines neuen **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="36546-116">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="36546-117">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="36546-117">Update</span></span>](../api/plannerbucket_update.md) | [<span data-ttu-id="36546-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="36546-118">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="36546-119">Dient zum Aktualisieren eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="36546-119">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="36546-120">Löschen</span><span class="sxs-lookup"><span data-stu-id="36546-120">Delete</span></span>](../api/plannerbucket_delete.md) | <span data-ttu-id="36546-121">Keine</span><span class="sxs-lookup"><span data-stu-id="36546-121">None</span></span> |<span data-ttu-id="36546-122">Dient zum Löschen eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="36546-122">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="36546-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36546-123">Properties</span></span>
| <span data-ttu-id="36546-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36546-124">Property</span></span>     | <span data-ttu-id="36546-125">Typ</span><span class="sxs-lookup"><span data-stu-id="36546-125">Type</span></span>   |<span data-ttu-id="36546-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36546-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36546-127">ID</span><span class="sxs-lookup"><span data-stu-id="36546-127">id</span></span>|<span data-ttu-id="36546-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36546-128">String</span></span>| <span data-ttu-id="36546-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="36546-129">Read-only.</span></span> <span data-ttu-id="36546-130">ID des Buckets.</span><span class="sxs-lookup"><span data-stu-id="36546-130">Name of the bucket.</span></span> <span data-ttu-id="36546-131">Er ist 28 Zeichen lang und beachtet Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="36546-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="36546-132">[Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="36546-132">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="36546-133">Name</span><span class="sxs-lookup"><span data-stu-id="36546-133">name</span></span>|<span data-ttu-id="36546-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36546-134">String</span></span>|<span data-ttu-id="36546-135">Name des Buckets.</span><span class="sxs-lookup"><span data-stu-id="36546-135">Name of the bucket.</span></span>|
|<span data-ttu-id="36546-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="36546-136">orderHint</span></span>|<span data-ttu-id="36546-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36546-137">String</span></span>|<span data-ttu-id="36546-p103">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="36546-p103">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="36546-140">planId</span><span class="sxs-lookup"><span data-stu-id="36546-140">planId</span></span>|<span data-ttu-id="36546-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36546-141">String</span></span>|<span data-ttu-id="36546-142">Plan-ID, zu der der Bucket gehört.</span><span class="sxs-lookup"><span data-stu-id="36546-142">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36546-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="36546-143">Relationships</span></span>
| <span data-ttu-id="36546-144">Beziehung</span><span class="sxs-lookup"><span data-stu-id="36546-144">Relationship</span></span> | <span data-ttu-id="36546-145">Typ</span><span class="sxs-lookup"><span data-stu-id="36546-145">Type</span></span>   |<span data-ttu-id="36546-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36546-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36546-147">Aufgaben</span><span class="sxs-lookup"><span data-stu-id="36546-147">tasks</span></span>|<span data-ttu-id="36546-148">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="36546-148">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="36546-p104">Schreibgeschützt. Lässt Nullwerte zu. Die Sammlung von Aufgaben im Bucket.</span><span class="sxs-lookup"><span data-stu-id="36546-p104">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36546-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="36546-152">JSON representation</span></span>
<span data-ttu-id="36546-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="36546-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->