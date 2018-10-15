# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="3305a-101">plannerTaskDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3305a-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="3305a-p101">Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="3305a-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="3305a-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="3305a-104">Methods</span></span>

| <span data-ttu-id="3305a-105">Methode</span><span class="sxs-lookup"><span data-stu-id="3305a-105">Method</span></span>           | <span data-ttu-id="3305a-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3305a-106">Return Type</span></span>    |<span data-ttu-id="3305a-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3305a-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3305a-108">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="3305a-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="3305a-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="3305a-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="3305a-110">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3305a-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="3305a-111">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3305a-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="3305a-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="3305a-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="3305a-113">Dient zum Aktualisieren des **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3305a-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3305a-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3305a-114">Properties</span></span>
| <span data-ttu-id="3305a-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3305a-115">Property</span></span>     | <span data-ttu-id="3305a-116">Typ</span><span class="sxs-lookup"><span data-stu-id="3305a-116">Type</span></span>   |<span data-ttu-id="3305a-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3305a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3305a-118">Checkliste</span><span class="sxs-lookup"><span data-stu-id="3305a-118">checklist</span></span>|[<span data-ttu-id="3305a-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="3305a-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="3305a-120">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="3305a-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="3305a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3305a-121">description</span></span>|<span data-ttu-id="3305a-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3305a-122">String</span></span>|<span data-ttu-id="3305a-123">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="3305a-123">Description of the task</span></span>|
|<span data-ttu-id="3305a-124">ID</span><span class="sxs-lookup"><span data-stu-id="3305a-124">id</span></span>|<span data-ttu-id="3305a-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3305a-125">String</span></span>| <span data-ttu-id="3305a-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3305a-126">Read-only.</span></span> <span data-ttu-id="3305a-127">ID der Aufgabendetails.</span><span class="sxs-lookup"><span data-stu-id="3305a-127">ID of the task details.</span></span> <span data-ttu-id="3305a-128">Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="3305a-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="3305a-129">Die [Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="3305a-129">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="3305a-130">previewType</span><span class="sxs-lookup"><span data-stu-id="3305a-130">previewType</span></span>|<span data-ttu-id="3305a-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3305a-131">string</span></span>|<span data-ttu-id="3305a-132">Hierdurch wird der Typ der Vorschau festgelegt, der für die Aufgabe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3305a-132">This sets the type of preview that shows up on the task. Possible values are: , , , , .</span></span> <span data-ttu-id="3305a-133">Mögliche Werte sind: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="3305a-133">The possible values are `automatic`, `noPreview`, `checklist`, `description`, `reference`, , , , , , , or .</span></span> <span data-ttu-id="3305a-134">Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, die die Aufgabe anzeigt.</span><span class="sxs-lookup"><span data-stu-id="3305a-134">This sets the type of preview that shows up on the task. Possible values are: , , , , . When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="3305a-135">Verweise</span><span class="sxs-lookup"><span data-stu-id="3305a-135">references</span></span>|[<span data-ttu-id="3305a-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="3305a-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="3305a-137">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="3305a-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3305a-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3305a-138">Relationships</span></span>
<span data-ttu-id="3305a-139">Keine</span><span class="sxs-lookup"><span data-stu-id="3305a-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3305a-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3305a-140">JSON representation</span></span>
<span data-ttu-id="3305a-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3305a-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
