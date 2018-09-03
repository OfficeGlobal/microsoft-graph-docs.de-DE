# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="011ac-101">plannerProgressTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="011ac-101">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="011ac-p101">Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder [Aufgabe](plannertask.md) ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="011ac-p101">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="011ac-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="011ac-104">Methods</span></span>

| <span data-ttu-id="011ac-105">Methode</span><span class="sxs-lookup"><span data-stu-id="011ac-105">Method</span></span>           | <span data-ttu-id="011ac-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="011ac-106">Return Type</span></span>    |<span data-ttu-id="011ac-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="011ac-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="011ac-108">plannerProgressTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="011ac-108">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat_get.md) | [<span data-ttu-id="011ac-109">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="011ac-109">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="011ac-110">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="011ac-110">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="011ac-111">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="011ac-111">Update</span></span>](../api/plannerprogresstaskboardtaskformat_update.md) | [<span data-ttu-id="011ac-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="011ac-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="011ac-113">Dient zum Aktualisieren des **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="011ac-113">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="011ac-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="011ac-114">Properties</span></span>
| <span data-ttu-id="011ac-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="011ac-115">Property</span></span>     | <span data-ttu-id="011ac-116">Typ</span><span class="sxs-lookup"><span data-stu-id="011ac-116">Type</span></span>   |<span data-ttu-id="011ac-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="011ac-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="011ac-118">id</span><span class="sxs-lookup"><span data-stu-id="011ac-118">id</span></span>|<span data-ttu-id="011ac-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="011ac-119">String</span></span>| <span data-ttu-id="011ac-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="011ac-120">Read-only.</span></span> <span data-ttu-id="011ac-121">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="011ac-121">The ID of the resource.</span></span> <span data-ttu-id="011ac-122">Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="011ac-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="011ac-123">[Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="011ac-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="011ac-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="011ac-124">orderHint</span></span>|<span data-ttu-id="011ac-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="011ac-125">String</span></span>|<span data-ttu-id="011ac-p103">Hinweiswert, der verwendet wird, um die Aufgaben in der Ansicht „Fortschritt“ des Task Board anzuordnen. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="011ac-p103">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="011ac-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="011ac-128">Relationships</span></span>
<span data-ttu-id="011ac-129">Keine</span><span class="sxs-lookup"><span data-stu-id="011ac-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="011ac-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="011ac-130">JSON representation</span></span>
<span data-ttu-id="011ac-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="011ac-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->