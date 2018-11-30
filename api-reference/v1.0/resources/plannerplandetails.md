---
title: plannerPlanDetails-Ressourcentyp
description: Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes plan-Objekt hat ein Detailobjekt.
ms.openlocfilehash: eac0082c72e46101d8d02367f8c13aef5e921d17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016588"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="9dcbe-104">plannerPlanDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9dcbe-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="9dcbe-p102">Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="9dcbe-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="9dcbe-107">Methods</span></span>

| <span data-ttu-id="9dcbe-108">Methode</span><span class="sxs-lookup"><span data-stu-id="9dcbe-108">Method</span></span>           | <span data-ttu-id="9dcbe-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9dcbe-109">Return Type</span></span>    |<span data-ttu-id="9dcbe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dcbe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9dcbe-111">plannerPlanDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="9dcbe-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="9dcbe-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="9dcbe-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="9dcbe-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlanDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="9dcbe-114">Update</span><span class="sxs-lookup"><span data-stu-id="9dcbe-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="9dcbe-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="9dcbe-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="9dcbe-116">Dient zum Aktualisieren des **plannerPlanDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9dcbe-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9dcbe-117">Properties</span></span>
| <span data-ttu-id="9dcbe-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9dcbe-118">Property</span></span>     | <span data-ttu-id="9dcbe-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9dcbe-119">Type</span></span>   |<span data-ttu-id="9dcbe-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dcbe-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dcbe-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="9dcbe-121">categoryDescriptions</span></span>|[<span data-ttu-id="9dcbe-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="9dcbe-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="9dcbe-123">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="9dcbe-124">id</span><span class="sxs-lookup"><span data-stu-id="9dcbe-124">id</span></span>|<span data-ttu-id="9dcbe-125">String</span><span class="sxs-lookup"><span data-stu-id="9dcbe-125">String</span></span>| <span data-ttu-id="9dcbe-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-126">Read-only.</span></span> <span data-ttu-id="9dcbe-127">ID des die Details des Plans.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-127">ID of the plan details.</span></span> <span data-ttu-id="9dcbe-128">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9dcbe-129">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9dcbe-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="9dcbe-130">sharedWith</span></span>|[<span data-ttu-id="9dcbe-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="9dcbe-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="9dcbe-p104">Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9dcbe-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9dcbe-135">Relationships</span></span>
<span data-ttu-id="9dcbe-136">Keine</span><span class="sxs-lookup"><span data-stu-id="9dcbe-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9dcbe-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9dcbe-137">JSON representation</span></span>
<span data-ttu-id="9dcbe-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9dcbe-138">Here is a JSON representation of the resource.</span></span>

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