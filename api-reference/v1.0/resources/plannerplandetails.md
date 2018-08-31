# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="e330b-101">plannerPlanDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e330b-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="e330b-p101">Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="e330b-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="e330b-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="e330b-104">Methods</span></span>

| <span data-ttu-id="e330b-105">Methode</span><span class="sxs-lookup"><span data-stu-id="e330b-105">Method</span></span>           | <span data-ttu-id="e330b-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e330b-106">Return Type</span></span>    |<span data-ttu-id="e330b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e330b-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e330b-108">plannerPlanDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="e330b-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="e330b-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e330b-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="e330b-110">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlanDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e330b-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="e330b-111">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e330b-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="e330b-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e330b-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="e330b-113">Dient zum Aktualisieren des **plannerPlanDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e330b-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e330b-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e330b-114">Properties</span></span>
| <span data-ttu-id="e330b-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e330b-115">Property</span></span>     | <span data-ttu-id="e330b-116">Typ</span><span class="sxs-lookup"><span data-stu-id="e330b-116">Type</span></span>   |<span data-ttu-id="e330b-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e330b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e330b-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="e330b-118">categoryDescriptions</span></span>|[<span data-ttu-id="e330b-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="e330b-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="e330b-120">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="e330b-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="e330b-121">ID</span><span class="sxs-lookup"><span data-stu-id="e330b-121">id</span></span>|<span data-ttu-id="e330b-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e330b-122">String</span></span>| <span data-ttu-id="e330b-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e330b-123">Read-only.</span></span> <span data-ttu-id="e330b-124">ID der Plan-Details.</span><span class="sxs-lookup"><span data-stu-id="e330b-124">ID of the plan details.</span></span> <span data-ttu-id="e330b-125">Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="e330b-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e330b-126">[Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="e330b-126">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e330b-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="e330b-127">sharedWith</span></span>|[<span data-ttu-id="e330b-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="e330b-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="e330b-p103">Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="e330b-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e330b-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e330b-132">Relationships</span></span>
<span data-ttu-id="e330b-133">Keine</span><span class="sxs-lookup"><span data-stu-id="e330b-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e330b-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e330b-134">JSON representation</span></span>
<span data-ttu-id="e330b-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e330b-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->