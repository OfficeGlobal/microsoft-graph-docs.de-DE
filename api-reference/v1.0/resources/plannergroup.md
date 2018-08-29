# <a name="plannergroup-resource-type"></a><span data-ttu-id="766b4-101">plannerGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="766b4-101">plannerGroup resource type</span></span>

<span data-ttu-id="766b4-p101">Die **plannerGroup**-Ressource bietet einer [Gruppe](group.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="766b4-p101">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="766b4-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="766b4-104">Methods</span></span>

| <span data-ttu-id="766b4-105">Methode</span><span class="sxs-lookup"><span data-stu-id="766b4-105">Method</span></span>           | <span data-ttu-id="766b4-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="766b4-106">Return Type</span></span>    |<span data-ttu-id="766b4-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766b4-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="766b4-108">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="766b4-108">List plans</span></span>](../api/plannergroup_list_plans.md) |<span data-ttu-id="766b4-109">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="766b4-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="766b4-110">Dient zum Abrufen einer **plannerPlan**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="766b4-110">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="766b4-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="766b4-111">Properties</span></span>
| <span data-ttu-id="766b4-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="766b4-112">Property</span></span>     | <span data-ttu-id="766b4-113">Typ</span><span class="sxs-lookup"><span data-stu-id="766b4-113">Type</span></span>   |<span data-ttu-id="766b4-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766b4-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="766b4-115">id</span><span class="sxs-lookup"><span data-stu-id="766b4-115">id</span></span>|<span data-ttu-id="766b4-116">String</span><span class="sxs-lookup"><span data-stu-id="766b4-116">String</span></span>| <span data-ttu-id="766b4-p102">Schreibgeschützt. Bezeichner der **plannerGroup**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="766b4-p102">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="766b4-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="766b4-119">Relationships</span></span>
| <span data-ttu-id="766b4-120">Beziehung</span><span class="sxs-lookup"><span data-stu-id="766b4-120">Relationship</span></span> | <span data-ttu-id="766b4-121">Typ</span><span class="sxs-lookup"><span data-stu-id="766b4-121">Type</span></span>   |<span data-ttu-id="766b4-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766b4-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="766b4-123">plans</span><span class="sxs-lookup"><span data-stu-id="766b4-123">plans</span></span>|<span data-ttu-id="766b4-124">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="766b4-124">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="766b4-p103">Schreibgeschützt. Lässt Nullwerte zu. Gibt die [plannerPlans](plannerplan.md) im Besitz der Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="766b4-p103">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="766b4-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="766b4-128">JSON representation</span></span>
<span data-ttu-id="766b4-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="766b4-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->