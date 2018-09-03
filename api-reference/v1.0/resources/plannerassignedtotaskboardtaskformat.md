# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="77f5e-101">plannerAssignedToTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77f5e-101">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="77f5e-p101">Die **plannerAssignedToTaskBoardTaskFormat** Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board verwendet werden (eine Ansicht, die nach Benutzern organisiert ist, denen Aufgaben zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerAssignedToTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="77f5e-p101">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="77f5e-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="77f5e-104">Methods</span></span>

| <span data-ttu-id="77f5e-105">Methode</span><span class="sxs-lookup"><span data-stu-id="77f5e-105">Method</span></span>           | <span data-ttu-id="77f5e-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="77f5e-106">Return Type</span></span>    |<span data-ttu-id="77f5e-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77f5e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77f5e-108">plannerAssignedToTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="77f5e-108">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat_get.md) | [<span data-ttu-id="77f5e-109">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="77f5e-109">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="77f5e-110">Dient zum Lesen der Eigenschaften und Beziehungen eines **PlannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="77f5e-110">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="77f5e-111">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="77f5e-111">Update</span></span>](../api/plannerassignedtotaskboardtaskformat_update.md) | [<span data-ttu-id="77f5e-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="77f5e-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="77f5e-113">Dient zum Aktualisieren eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="77f5e-113">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77f5e-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77f5e-114">Properties</span></span>
| <span data-ttu-id="77f5e-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77f5e-115">Property</span></span>     | <span data-ttu-id="77f5e-116">Typ</span><span class="sxs-lookup"><span data-stu-id="77f5e-116">Type</span></span>   |<span data-ttu-id="77f5e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77f5e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f5e-118">id</span><span class="sxs-lookup"><span data-stu-id="77f5e-118">id</span></span>|<span data-ttu-id="77f5e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77f5e-119">String</span></span>| <span data-ttu-id="77f5e-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77f5e-120">Read-only.</span></span> <span data-ttu-id="77f5e-121">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77f5e-121">The ID of the resource.</span></span> <span data-ttu-id="77f5e-122">Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="77f5e-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="77f5e-123">[Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="77f5e-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="77f5e-124">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="77f5e-124">orderHintsByAssignee</span></span>|[<span data-ttu-id="77f5e-125">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="77f5e-125">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="77f5e-p103">Wörterbuch von Hinweisen, die verwendet werden, um Aufgaben in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen. Der Schlüssel für jeden Eintrag ist einer der Benutzer, denen die Aufgabe zugewiesen ist, und der Wert ist der Anordnungshinweis. Das Format der einzelnen Werte ist wie [hier](planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="77f5e-p103">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="77f5e-129">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="77f5e-129">unassignedOrderHint</span></span>|<span data-ttu-id="77f5e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77f5e-130">String</span></span>|<span data-ttu-id="77f5e-p104">Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="77f5e-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="77f5e-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77f5e-133">Relationships</span></span>
<span data-ttu-id="77f5e-134">Keine</span><span class="sxs-lookup"><span data-stu-id="77f5e-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="77f5e-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77f5e-135">JSON representation</span></span>
<span data-ttu-id="77f5e-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77f5e-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->