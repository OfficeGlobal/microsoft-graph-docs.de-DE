# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="c5615-101">plannerTaskDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c5615-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="c5615-p101">Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="c5615-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="c5615-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="c5615-104">Methods</span></span>

| <span data-ttu-id="c5615-105">Methode</span><span class="sxs-lookup"><span data-stu-id="c5615-105">Method</span></span>           | <span data-ttu-id="c5615-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c5615-106">Return Type</span></span>    |<span data-ttu-id="c5615-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5615-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5615-108">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="c5615-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="c5615-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="c5615-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="c5615-110">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5615-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="c5615-111">Update</span><span class="sxs-lookup"><span data-stu-id="c5615-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="c5615-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="c5615-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="c5615-113">Dient zum Aktualisieren des **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5615-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c5615-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c5615-114">Properties</span></span>
| <span data-ttu-id="c5615-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5615-115">Property</span></span>     | <span data-ttu-id="c5615-116">Typ</span><span class="sxs-lookup"><span data-stu-id="c5615-116">Type</span></span>   |<span data-ttu-id="c5615-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5615-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5615-118">checklist</span><span class="sxs-lookup"><span data-stu-id="c5615-118">checklist</span></span>|[<span data-ttu-id="c5615-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="c5615-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="c5615-120">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="c5615-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="c5615-121">description</span><span class="sxs-lookup"><span data-stu-id="c5615-121">description</span></span>|<span data-ttu-id="c5615-122">String</span><span class="sxs-lookup"><span data-stu-id="c5615-122">String</span></span>|<span data-ttu-id="c5615-123">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="c5615-123">Description of the task</span></span>|
|<span data-ttu-id="c5615-124">id</span><span class="sxs-lookup"><span data-stu-id="c5615-124">id</span></span>|<span data-ttu-id="c5615-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5615-125">String</span></span>| <span data-ttu-id="c5615-p102">Schreibgeschützt. ID der Aufgabendetails. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](planner_identifiers_disclaimer.md) durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="c5615-p102">Read-only. ID of the task details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c5615-130">previewType</span><span class="sxs-lookup"><span data-stu-id="c5615-130">previewType</span></span>|<span data-ttu-id="c5615-131">string</span><span class="sxs-lookup"><span data-stu-id="c5615-131">string</span></span>|<span data-ttu-id="c5615-p103">Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c5615-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="c5615-135">references</span><span class="sxs-lookup"><span data-stu-id="c5615-135">references</span></span>|[<span data-ttu-id="c5615-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="c5615-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="c5615-137">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="c5615-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5615-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c5615-138">Relationships</span></span>
<span data-ttu-id="c5615-139">Keine</span><span class="sxs-lookup"><span data-stu-id="c5615-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c5615-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c5615-140">JSON representation</span></span>
<span data-ttu-id="c5615-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c5615-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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