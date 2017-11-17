# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="ebce9-101">plannerPlanDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ebce9-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="ebce9-p101">Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="ebce9-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="ebce9-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="ebce9-104">Methods</span></span>

| <span data-ttu-id="ebce9-105">Methode</span><span class="sxs-lookup"><span data-stu-id="ebce9-105">Method</span></span>           | <span data-ttu-id="ebce9-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ebce9-106">Return Type</span></span>    |<span data-ttu-id="ebce9-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebce9-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebce9-108">plannerPlanDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="ebce9-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="ebce9-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="ebce9-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="ebce9-110">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlanDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebce9-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="ebce9-111">Update</span><span class="sxs-lookup"><span data-stu-id="ebce9-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="ebce9-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="ebce9-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="ebce9-113">Dient zum Aktualisieren des **plannerPlanDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebce9-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ebce9-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ebce9-114">Properties</span></span>
| <span data-ttu-id="ebce9-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebce9-115">Property</span></span>     | <span data-ttu-id="ebce9-116">Typ</span><span class="sxs-lookup"><span data-stu-id="ebce9-116">Type</span></span>   |<span data-ttu-id="ebce9-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebce9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebce9-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="ebce9-118">categoryDescriptions</span></span>|[<span data-ttu-id="ebce9-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="ebce9-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="ebce9-120">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="ebce9-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="ebce9-121">id</span><span class="sxs-lookup"><span data-stu-id="ebce9-121">id</span></span>|<span data-ttu-id="ebce9-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebce9-122">String</span></span>| <span data-ttu-id="ebce9-p102">Schreibgeschützt. ID der Plandetails. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](planner_identifiers_disclaimer.md) durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="ebce9-p102">Read-only. ID of the plan details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ebce9-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="ebce9-127">sharedWith</span></span>|[<span data-ttu-id="ebce9-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="ebce9-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="ebce9-p103">Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="ebce9-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ebce9-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ebce9-132">Relationships</span></span>
<span data-ttu-id="ebce9-133">Keine</span><span class="sxs-lookup"><span data-stu-id="ebce9-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ebce9-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ebce9-134">JSON representation</span></span>
<span data-ttu-id="ebce9-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ebce9-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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