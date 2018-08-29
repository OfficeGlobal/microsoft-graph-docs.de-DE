# <a name="planneruser-resource-type"></a><span data-ttu-id="4bf94-101">plannerUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4bf94-101">plannerUser resource type</span></span>

<span data-ttu-id="4bf94-p101">Die **plannerUser**-Ressource bietet einem [Benutzer](user.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4bf94-p101">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="4bf94-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="4bf94-104">Methods</span></span>

| <span data-ttu-id="4bf94-105">Methode</span><span class="sxs-lookup"><span data-stu-id="4bf94-105">Method</span></span>           | <span data-ttu-id="4bf94-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4bf94-106">Return Type</span></span>    |<span data-ttu-id="4bf94-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bf94-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bf94-108">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="4bf94-108">List plans</span></span>](../api/planneruser_list_plans.md) |<span data-ttu-id="4bf94-109">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4bf94-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4bf94-110">Dient zum Abrufen einer **plannerPlan**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="4bf94-110">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="4bf94-111">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="4bf94-111">List tasks</span></span>](../api/planneruser_list_tasks.md) |<span data-ttu-id="4bf94-112">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4bf94-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="4bf94-113">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="4bf94-113">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="4bf94-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4bf94-114">Properties</span></span>
| <span data-ttu-id="4bf94-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4bf94-115">Property</span></span>     | <span data-ttu-id="4bf94-116">Typ</span><span class="sxs-lookup"><span data-stu-id="4bf94-116">Type</span></span>   |<span data-ttu-id="4bf94-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bf94-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bf94-118">id</span><span class="sxs-lookup"><span data-stu-id="4bf94-118">id</span></span>|<span data-ttu-id="4bf94-119">String</span><span class="sxs-lookup"><span data-stu-id="4bf94-119">String</span></span>| <span data-ttu-id="4bf94-p102">Schreibgeschützt. Bezeichner der plannerUser-Ressource.</span><span class="sxs-lookup"><span data-stu-id="4bf94-p102">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bf94-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4bf94-122">Relationships</span></span>
| <span data-ttu-id="4bf94-123">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4bf94-123">Relationship</span></span> | <span data-ttu-id="4bf94-124">Typ</span><span class="sxs-lookup"><span data-stu-id="4bf94-124">Type</span></span>   |<span data-ttu-id="4bf94-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bf94-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bf94-126">plans</span><span class="sxs-lookup"><span data-stu-id="4bf94-126">plans</span></span>|<span data-ttu-id="4bf94-127">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4bf94-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4bf94-p103">Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="4bf94-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="4bf94-131">tasks</span><span class="sxs-lookup"><span data-stu-id="4bf94-131">tasks</span></span>|<span data-ttu-id="4bf94-132">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4bf94-132">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="4bf94-p104">Schreibgeschützt. Lässt Nullwerte zu. Gibt die für den Benutzer freigegebenen [plannerPlans](plannerplan.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="4bf94-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4bf94-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4bf94-136">JSON representation</span></span>
<span data-ttu-id="4bf94-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4bf94-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->