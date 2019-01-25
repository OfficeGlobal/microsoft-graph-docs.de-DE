---
title: plannerPlanDetails-Ressourcentyp
description: Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes plan-Objekt hat ein Detailobjekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529880"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="96081-104">plannerPlanDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="96081-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96081-p102">Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="96081-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="96081-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="96081-107">Methods</span></span>

| <span data-ttu-id="96081-108">Methode</span><span class="sxs-lookup"><span data-stu-id="96081-108">Method</span></span>           | <span data-ttu-id="96081-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="96081-109">Return Type</span></span>    |<span data-ttu-id="96081-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96081-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96081-111">plannerPlanDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="96081-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="96081-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="96081-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="96081-113">Lesen Sie die Eigenschaften und die Beziehungen eines **PlannerPlanDetails** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="96081-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="96081-114">Update</span><span class="sxs-lookup"><span data-stu-id="96081-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="96081-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="96081-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="96081-116">Aktualisieren eines **PlannerPlanDetails** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="96081-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="96081-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96081-117">Properties</span></span>
| <span data-ttu-id="96081-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96081-118">Property</span></span>     | <span data-ttu-id="96081-119">Typ</span><span class="sxs-lookup"><span data-stu-id="96081-119">Type</span></span>   |<span data-ttu-id="96081-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96081-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96081-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="96081-121">categoryDescriptions</span></span>|[<span data-ttu-id="96081-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="96081-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="96081-123">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="96081-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="96081-124">id</span><span class="sxs-lookup"><span data-stu-id="96081-124">id</span></span>|<span data-ttu-id="96081-125">String</span><span class="sxs-lookup"><span data-stu-id="96081-125">String</span></span>| <span data-ttu-id="96081-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="96081-126">Read-only.</span></span> <span data-ttu-id="96081-127">Die ID des die Details des Plans.</span><span class="sxs-lookup"><span data-stu-id="96081-127">The ID of the plan details.</span></span> <span data-ttu-id="96081-128">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="96081-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="96081-129">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="96081-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="96081-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="96081-130">sharedWith</span></span>|[<span data-ttu-id="96081-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="96081-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="96081-132">Der Satz von Benutzer-IDs, die mit diesem Plan freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="96081-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="96081-133">Wenn Sie Office 365 Gruppen verwenden, verwenden Sie die API-Gruppen zum Verwalten der Gruppenmitgliedschaft zum Planen [der Gruppe](group.md) freigeben.</span><span class="sxs-lookup"><span data-stu-id="96081-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="96081-134">Sie können auch vorhandene Mitglieder der Gruppe zu dieser Auflistung hinzufügen, obwohl es nicht erforderlich ist, damit sie Zugriff auf den Besitz der Gruppe Plan.</span><span class="sxs-lookup"><span data-stu-id="96081-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="96081-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="96081-135">contextDetails</span></span>|[<span data-ttu-id="96081-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="96081-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="96081-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="96081-137">Read-only.</span></span> <span data-ttu-id="96081-138">Eine Auflistung von zusätzlichen Informationen im Zusammenhang mit [PlannerPlanContext](plannerplancontext.md) -Einträge, die für den Container [PlannerPlan](plannerplan.md) definiert sind.</span><span class="sxs-lookup"><span data-stu-id="96081-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96081-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="96081-139">Relationships</span></span>
<span data-ttu-id="96081-140">Keine.</span><span class="sxs-lookup"><span data-stu-id="96081-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="96081-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96081-141">JSON representation</span></span>
<span data-ttu-id="96081-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96081-142">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplandetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
