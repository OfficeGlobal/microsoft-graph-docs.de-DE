---
title: plannerUser-Ressourcentyp
description: 'Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen Benutzer. '
ms.openlocfilehash: 592a26daacd1bd6d0a780ca0180d3ec5a57b6eb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062234"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="94308-103">plannerUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="94308-103">plannerUser resource type</span></span>

> <span data-ttu-id="94308-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94308-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94308-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94308-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94308-106">Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen [Benutzer](user.md).</span><span class="sxs-lookup"><span data-stu-id="94308-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="94308-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="94308-107">Methods</span></span>

| <span data-ttu-id="94308-108">Methode</span><span class="sxs-lookup"><span data-stu-id="94308-108">Method</span></span>           | <span data-ttu-id="94308-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="94308-109">Return Type</span></span>    |<span data-ttu-id="94308-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94308-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94308-111">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="94308-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="94308-112">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="94308-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="94308-113">Rufen Sie die [PlannerTasks](plannertask.md) die ihm zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="94308-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="94308-114">Liste favoritePlans</span><span class="sxs-lookup"><span data-stu-id="94308-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="94308-115">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="94308-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="94308-116">Rufen Sie die [PlannerPlans](plannerplan.md) durch den Benutzer als bevorzugten markiert.</span><span class="sxs-lookup"><span data-stu-id="94308-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="94308-117">Liste recentPlans</span><span class="sxs-lookup"><span data-stu-id="94308-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="94308-118">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="94308-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="94308-119">Rufen Sie die [PlannerPlans](plannerplan.md) zuletzt vom Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="94308-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="94308-120">Update</span><span class="sxs-lookup"><span data-stu-id="94308-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="94308-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="94308-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="94308-122">Aktualisieren eines **PlannerUser** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="94308-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="94308-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94308-123">Properties</span></span>
| <span data-ttu-id="94308-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94308-124">Property</span></span>     | <span data-ttu-id="94308-125">Typ</span><span class="sxs-lookup"><span data-stu-id="94308-125">Type</span></span>   |<span data-ttu-id="94308-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94308-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94308-127">id</span><span class="sxs-lookup"><span data-stu-id="94308-127">id</span></span>|<span data-ttu-id="94308-128">String</span><span class="sxs-lookup"><span data-stu-id="94308-128">String</span></span>| <span data-ttu-id="94308-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94308-129">Read-only.</span></span> <span data-ttu-id="94308-130">Bezeichner des der plannerUser</span><span class="sxs-lookup"><span data-stu-id="94308-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="94308-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="94308-131">favoritePlanReferences</span></span>|[<span data-ttu-id="94308-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="94308-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="94308-133">Eine Auflistung mit der Verweise auf die Pläne, die der Benutzer als Favoriten gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="94308-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="94308-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="94308-134">recentPlanReferences</span></span>|[<span data-ttu-id="94308-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="94308-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="94308-136">Eine Auflistung mit Verweisen auf die Pläne, die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="94308-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94308-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94308-137">Relationships</span></span>
| <span data-ttu-id="94308-138">Beziehung</span><span class="sxs-lookup"><span data-stu-id="94308-138">Relationship</span></span> | <span data-ttu-id="94308-139">Typ</span><span class="sxs-lookup"><span data-stu-id="94308-139">Type</span></span>   |<span data-ttu-id="94308-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94308-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94308-141">tasks</span><span class="sxs-lookup"><span data-stu-id="94308-141">tasks</span></span>|<span data-ttu-id="94308-142">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="94308-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="94308-p103">Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="94308-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="94308-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="94308-146">favoritePlans</span></span>|<span data-ttu-id="94308-147">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="94308-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="94308-148">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94308-148">Read-only.</span></span> <span data-ttu-id="94308-149">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="94308-149">Nullable.</span></span> <span data-ttu-id="94308-150">Gibt die [PlannerPlans](plannerplan.md) , die der Benutzer als Favoriten gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="94308-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="94308-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="94308-151">recentPlans</span></span>|<span data-ttu-id="94308-152">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="94308-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="94308-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94308-153">Read-only.</span></span> <span data-ttu-id="94308-154">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="94308-154">Nullable.</span></span> <span data-ttu-id="94308-155">Gibt die [PlannerPlans](plannerplan.md) , die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="94308-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94308-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94308-156">JSON representation</span></span>
<span data-ttu-id="94308-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94308-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
