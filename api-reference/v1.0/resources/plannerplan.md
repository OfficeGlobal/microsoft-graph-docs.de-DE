# <a name="plannerplan-resource-type"></a><span data-ttu-id="6efb3-101">plannerPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6efb3-101">plannerPlan resource type</span></span>

<span data-ttu-id="6efb3-p101">Die **plannerPlan**-Ressource stellt einen Plan in Office 365 dar. Ein Plan kann im Besitz einer [Gruppe](group.md) sein und enthält eine Sammlung von [plannerTasks](plannerTask.md). Er kann auch über eine Sammlung von [plannerBuckets](plannerBucket.md) verfügen. Jedes Planobjekt verfügt über [details](plannerPlanDetails.md)-Objekt, das weitere Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Plänen und Aufgaben finden Sie unter [Planner](planner_overview.md).</span><span class="sxs-lookup"><span data-stu-id="6efb3-p101">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannerTask.md). It can also have a collection of [plannerBuckets](plannerBucket.md). Each plan object has a [details](plannerPlanDetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6efb3-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="6efb3-107">Methods</span></span>

| <span data-ttu-id="6efb3-108">Methode</span><span class="sxs-lookup"><span data-stu-id="6efb3-108">Method</span></span>           | <span data-ttu-id="6efb3-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6efb3-109">Return Type</span></span>    |<span data-ttu-id="6efb3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6efb3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6efb3-111">plannerPlan abrufen</span><span class="sxs-lookup"><span data-stu-id="6efb3-111">Get plannerPlan</span></span>](../api/plannerplan_get.md) | [<span data-ttu-id="6efb3-112">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6efb3-112">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="6efb3-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6efb3-113">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="6efb3-114">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="6efb3-114">List buckets</span></span>](../api/plannerplan_list_buckets.md) |<span data-ttu-id="6efb3-115">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6efb3-115">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="6efb3-116">Dient zum Abrufen einer **plannerBucket**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="6efb3-116">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="6efb3-117">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="6efb3-117">List tasks</span></span>](../api/plannerplan_list_tasks.md) |<span data-ttu-id="6efb3-118">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6efb3-118">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="6efb3-119">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="6efb3-119">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="6efb3-120">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6efb3-120">Update</span></span>](../api/plannerplan_update.md) | [<span data-ttu-id="6efb3-121">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6efb3-121">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="6efb3-122">Dient zum Aktualisieren eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6efb3-122">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6efb3-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6efb3-123">Properties</span></span>
| <span data-ttu-id="6efb3-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6efb3-124">Property</span></span>     | <span data-ttu-id="6efb3-125">Typ</span><span class="sxs-lookup"><span data-stu-id="6efb3-125">Type</span></span>   |<span data-ttu-id="6efb3-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6efb3-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6efb3-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6efb3-127">createdDateTime</span></span>|<span data-ttu-id="6efb3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efb3-128">DateTimeOffset</span></span>|<span data-ttu-id="6efb3-p102">Schreibgeschützt. Datum und Uhrzeit der Erstellung des Plans. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6efb3-p102">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6efb3-133">id</span><span class="sxs-lookup"><span data-stu-id="6efb3-133">id</span></span>|<span data-ttu-id="6efb3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6efb3-134">String</span></span>| <span data-ttu-id="6efb3-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6efb3-135">Read-only.</span></span> <span data-ttu-id="6efb3-136">ID des Plans.</span><span class="sxs-lookup"><span data-stu-id="6efb3-136">Title of the plan.</span></span> <span data-ttu-id="6efb3-137">Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="6efb3-137">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6efb3-138">Die [Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="6efb3-138">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6efb3-139">owner</span><span class="sxs-lookup"><span data-stu-id="6efb3-139">owner</span></span>|<span data-ttu-id="6efb3-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6efb3-140">String</span></span>|<span data-ttu-id="6efb3-p104">ID der [Gruppe](group.md), die den Plan besitzt. Dieses Feld kann erst festgelegt werden, wenn eine gültige Gruppe vorhanden ist. Nachdem dieses festgelegt wurde, kann es nur noch vom Besitzer aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="6efb3-p104">ID of the [Group](group.md) that owns the plan. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="6efb3-144">title</span><span class="sxs-lookup"><span data-stu-id="6efb3-144">title</span></span>|<span data-ttu-id="6efb3-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6efb3-145">String</span></span>|<span data-ttu-id="6efb3-p105">Erforderlich.  Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="6efb3-p105">Required. Title of the plan.</span></span>|
|<span data-ttu-id="6efb3-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="6efb3-148">createdBy</span></span>|[<span data-ttu-id="6efb3-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="6efb3-149">identitySet</span></span>](identityset.md)|<span data-ttu-id="6efb3-p106">Schreibgeschützt. Der Benutzer, der den Plan erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="6efb3-p106">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6efb3-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6efb3-152">Relationships</span></span>
| <span data-ttu-id="6efb3-153">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6efb3-153">Relationship</span></span> | <span data-ttu-id="6efb3-154">Typ</span><span class="sxs-lookup"><span data-stu-id="6efb3-154">Type</span></span>   |<span data-ttu-id="6efb3-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6efb3-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6efb3-156">buckets</span><span class="sxs-lookup"><span data-stu-id="6efb3-156">buckets</span></span>|<span data-ttu-id="6efb3-157">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6efb3-157">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="6efb3-p107">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Buckets im Plan.</span><span class="sxs-lookup"><span data-stu-id="6efb3-p107">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="6efb3-161">Details</span><span class="sxs-lookup"><span data-stu-id="6efb3-161">details</span></span>|[<span data-ttu-id="6efb3-162">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="6efb3-162">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="6efb3-p108">Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über den Plan.</span><span class="sxs-lookup"><span data-stu-id="6efb3-p108">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="6efb3-166">tasks</span><span class="sxs-lookup"><span data-stu-id="6efb3-166">tasks</span></span>|<span data-ttu-id="6efb3-167">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6efb3-167">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="6efb3-p109">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Aufgaben im Plan.</span><span class="sxs-lookup"><span data-stu-id="6efb3-p109">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6efb3-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6efb3-171">JSON representation</span></span>

<span data-ttu-id="6efb3-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6efb3-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->