# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="88d96-101">plannerBucketTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88d96-101">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="88d96-p101">Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="88d96-p101">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="88d96-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="88d96-104">Methods</span></span>

| <span data-ttu-id="88d96-105">Methode</span><span class="sxs-lookup"><span data-stu-id="88d96-105">Method</span></span>           | <span data-ttu-id="88d96-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="88d96-106">Return Type</span></span>    |<span data-ttu-id="88d96-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88d96-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88d96-108">plannerBucketTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="88d96-108">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat_get.md) | [<span data-ttu-id="88d96-109">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="88d96-109">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="88d96-110">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="88d96-110">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="88d96-111">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="88d96-111">Update</span></span>](../api/plannerbuckettaskboardtaskformat_update.md) | [<span data-ttu-id="88d96-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="88d96-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="88d96-113">Dient zum Aktualisieren des **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="88d96-113">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="88d96-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88d96-114">Properties</span></span>
| <span data-ttu-id="88d96-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88d96-115">Property</span></span>     | <span data-ttu-id="88d96-116">Typ</span><span class="sxs-lookup"><span data-stu-id="88d96-116">Type</span></span>   |<span data-ttu-id="88d96-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88d96-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88d96-118">ID</span><span class="sxs-lookup"><span data-stu-id="88d96-118">id</span></span>|<span data-ttu-id="88d96-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88d96-119">String</span></span>| <span data-ttu-id="88d96-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="88d96-120">Read-only.</span></span> <span data-ttu-id="88d96-121">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88d96-121">The ID of the resource.</span></span> <span data-ttu-id="88d96-122">Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="88d96-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="88d96-123">Die [Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="88d96-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="88d96-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="88d96-124">orderHint</span></span>|<span data-ttu-id="88d96-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88d96-125">String</span></span>|<span data-ttu-id="88d96-p103">Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="88d96-p103">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="88d96-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="88d96-128">Relationships</span></span>
<span data-ttu-id="88d96-129">Keine</span><span class="sxs-lookup"><span data-stu-id="88d96-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="88d96-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88d96-130">JSON representation</span></span>
<span data-ttu-id="88d96-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88d96-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->