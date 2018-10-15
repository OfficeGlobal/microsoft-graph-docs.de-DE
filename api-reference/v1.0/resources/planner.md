# <a name="planner-resource-type"></a><span data-ttu-id="b8286-101">planner-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8286-101">planner resource type</span></span>

<span data-ttu-id="b8286-p101">Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="b8286-p101">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="b8286-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b8286-105">Methods</span></span>

| <span data-ttu-id="b8286-106">Methode</span><span class="sxs-lookup"><span data-stu-id="b8286-106">Method</span></span>           | <span data-ttu-id="b8286-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b8286-107">Return Type</span></span>    |<span data-ttu-id="b8286-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8286-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8286-109">plannerBucket erstellen</span><span class="sxs-lookup"><span data-stu-id="b8286-109">Create plannerBucket</span></span>](../api/planner_post_buckets.md) |[<span data-ttu-id="b8286-110">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b8286-110">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="b8286-111">Dient zum Erstellen eines neuen **plannerBucket** durch Veröffentlichung in der buckets-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="b8286-111">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="b8286-112">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="b8286-112">Create plannerPlan</span></span>](../api/planner_post_plans.md) |[<span data-ttu-id="b8286-113">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b8286-113">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="b8286-114">Dient zum Erstellen eines neuen **plannerPlan** durch Veröffentlichung in der plans-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="b8286-114">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="b8286-115">plannerTask erstellen</span><span class="sxs-lookup"><span data-stu-id="b8286-115">Create plannerTask</span></span>](../api/planner_post_tasks.md) |[<span data-ttu-id="b8286-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="b8286-116">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="b8286-117">Dient zum Erstellen einer neuen **plannerTask** durch Veröffentlichung in der tasks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="b8286-117">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8286-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8286-118">Relationships</span></span>
| <span data-ttu-id="b8286-119">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b8286-119">Relationship</span></span> | <span data-ttu-id="b8286-120">Typ</span><span class="sxs-lookup"><span data-stu-id="b8286-120">Type</span></span>   |<span data-ttu-id="b8286-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8286-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8286-122">Buckets</span><span class="sxs-lookup"><span data-stu-id="b8286-122">buckets</span></span>|<span data-ttu-id="b8286-123">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b8286-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b8286-p102">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen einfaches zurück.</span><span class="sxs-lookup"><span data-stu-id="b8286-p102">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="b8286-127">plans</span><span class="sxs-lookup"><span data-stu-id="b8286-127">plans</span></span>|<span data-ttu-id="b8286-128">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b8286-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b8286-p103">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Pläne zurück.</span><span class="sxs-lookup"><span data-stu-id="b8286-p103">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="b8286-132">Aufgaben</span><span class="sxs-lookup"><span data-stu-id="b8286-132">tasks</span></span>|<span data-ttu-id="b8286-133">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b8286-133">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b8286-p104">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Aufgaben zurück.</span><span class="sxs-lookup"><span data-stu-id="b8286-p104">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8286-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8286-137">JSON representation</span></span>
<span data-ttu-id="b8286-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8286-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="b8286-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8286-139">Example</span></span>

<span data-ttu-id="b8286-140">Die **Planner** -Ressource ist im Stamm des Diagramms verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b8286-140">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->