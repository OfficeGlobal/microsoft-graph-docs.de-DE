---
title: plannerPlanDetails-Ressourcentyp
description: Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes plan-Objekt hat ein Detailobjekt.
ms.openlocfilehash: 1cce5727666bca705da67fccd1a3edf370c68127
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064756"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="07f66-104">plannerPlanDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07f66-104">plannerPlanDetails resource type</span></span>

> <span data-ttu-id="07f66-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07f66-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07f66-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07f66-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07f66-p103">Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="07f66-p103">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="07f66-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="07f66-109">Methods</span></span>

| <span data-ttu-id="07f66-110">Methode</span><span class="sxs-lookup"><span data-stu-id="07f66-110">Method</span></span>           | <span data-ttu-id="07f66-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="07f66-111">Return Type</span></span>    |<span data-ttu-id="07f66-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07f66-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07f66-113">plannerPlanDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="07f66-113">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="07f66-114">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="07f66-114">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="07f66-115">Lesen Sie die Eigenschaften und die Beziehungen eines **PlannerPlanDetails** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="07f66-115">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="07f66-116">Update</span><span class="sxs-lookup"><span data-stu-id="07f66-116">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="07f66-117">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="07f66-117">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="07f66-118">Aktualisieren eines **PlannerPlanDetails** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="07f66-118">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="07f66-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07f66-119">Properties</span></span>
| <span data-ttu-id="07f66-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07f66-120">Property</span></span>     | <span data-ttu-id="07f66-121">Typ</span><span class="sxs-lookup"><span data-stu-id="07f66-121">Type</span></span>   |<span data-ttu-id="07f66-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07f66-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07f66-123">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="07f66-123">categoryDescriptions</span></span>|[<span data-ttu-id="07f66-124">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="07f66-124">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="07f66-125">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="07f66-125">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="07f66-126">id</span><span class="sxs-lookup"><span data-stu-id="07f66-126">id</span></span>|<span data-ttu-id="07f66-127">String</span><span class="sxs-lookup"><span data-stu-id="07f66-127">String</span></span>| <span data-ttu-id="07f66-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="07f66-128">Read-only.</span></span> <span data-ttu-id="07f66-129">Die ID des die Details des Plans.</span><span class="sxs-lookup"><span data-stu-id="07f66-129">The ID of the plan details.</span></span> <span data-ttu-id="07f66-130">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="07f66-130">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="07f66-131">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="07f66-131">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="07f66-132">sharedWith</span><span class="sxs-lookup"><span data-stu-id="07f66-132">sharedWith</span></span>|[<span data-ttu-id="07f66-133">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="07f66-133">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="07f66-134">Der Satz von Benutzer-IDs, die mit diesem Plan freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="07f66-134">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="07f66-135">Wenn Sie Office 365 Gruppen verwenden, verwenden Sie die API-Gruppen zum Verwalten der Gruppenmitgliedschaft zum Planen [der Gruppe](group.md) freigeben.</span><span class="sxs-lookup"><span data-stu-id="07f66-135">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="07f66-136">Sie können auch vorhandene Mitglieder der Gruppe zu dieser Auflistung hinzufügen, obwohl es nicht erforderlich ist, damit sie Zugriff auf den Besitz der Gruppe Plan.</span><span class="sxs-lookup"><span data-stu-id="07f66-136">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="07f66-137">contextDetails</span><span class="sxs-lookup"><span data-stu-id="07f66-137">contextDetails</span></span>|[<span data-ttu-id="07f66-138">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="07f66-138">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="07f66-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="07f66-139">Read-only.</span></span> <span data-ttu-id="07f66-140">Eine Auflistung von zusätzlichen Informationen im Zusammenhang mit [PlannerPlanContext](plannerplancontext.md) -Einträge, die für den Container [PlannerPlan](plannerplan.md) definiert sind.</span><span class="sxs-lookup"><span data-stu-id="07f66-140">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="07f66-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07f66-141">Relationships</span></span>
<span data-ttu-id="07f66-142">Keine.</span><span class="sxs-lookup"><span data-stu-id="07f66-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="07f66-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07f66-143">JSON representation</span></span>
<span data-ttu-id="07f66-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07f66-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
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
