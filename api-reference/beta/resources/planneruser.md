---
title: plannerUser-Ressourcentyp
description: 'Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen Benutzer. '
localization_priority: Normal
ms.openlocfilehash: 709b259c88d8fe0f02defaa57e77727a7b967cfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820804"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="fff28-103">plannerUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fff28-103">plannerUser resource type</span></span>

> <span data-ttu-id="fff28-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fff28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fff28-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fff28-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fff28-106">Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen [Benutzer](user.md).</span><span class="sxs-lookup"><span data-stu-id="fff28-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="fff28-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="fff28-107">Methods</span></span>

| <span data-ttu-id="fff28-108">Methode</span><span class="sxs-lookup"><span data-stu-id="fff28-108">Method</span></span>           | <span data-ttu-id="fff28-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fff28-109">Return Type</span></span>    |<span data-ttu-id="fff28-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fff28-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fff28-111">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="fff28-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="fff28-112">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fff28-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fff28-113">Rufen Sie die [PlannerTasks](plannertask.md) die ihm zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="fff28-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="fff28-114">Liste favoritePlans</span><span class="sxs-lookup"><span data-stu-id="fff28-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="fff28-115">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fff28-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="fff28-116">Rufen Sie die [PlannerPlans](plannerplan.md) durch den Benutzer als bevorzugten markiert.</span><span class="sxs-lookup"><span data-stu-id="fff28-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="fff28-117">Liste recentPlans</span><span class="sxs-lookup"><span data-stu-id="fff28-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="fff28-118">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fff28-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="fff28-119">Rufen Sie die [PlannerPlans](plannerplan.md) zuletzt vom Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="fff28-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="fff28-120">Update</span><span class="sxs-lookup"><span data-stu-id="fff28-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="fff28-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="fff28-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="fff28-122">Aktualisieren eines **PlannerUser** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fff28-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="fff28-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fff28-123">Properties</span></span>
| <span data-ttu-id="fff28-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fff28-124">Property</span></span>     | <span data-ttu-id="fff28-125">Typ</span><span class="sxs-lookup"><span data-stu-id="fff28-125">Type</span></span>   |<span data-ttu-id="fff28-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fff28-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fff28-127">id</span><span class="sxs-lookup"><span data-stu-id="fff28-127">id</span></span>|<span data-ttu-id="fff28-128">String</span><span class="sxs-lookup"><span data-stu-id="fff28-128">String</span></span>| <span data-ttu-id="fff28-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fff28-129">Read-only.</span></span> <span data-ttu-id="fff28-130">Bezeichner des der plannerUser</span><span class="sxs-lookup"><span data-stu-id="fff28-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="fff28-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="fff28-131">favoritePlanReferences</span></span>|[<span data-ttu-id="fff28-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="fff28-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="fff28-133">Eine Auflistung mit der Verweise auf die Pläne, die der Benutzer als Favoriten gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="fff28-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="fff28-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="fff28-134">recentPlanReferences</span></span>|[<span data-ttu-id="fff28-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="fff28-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="fff28-136">Eine Auflistung mit Verweisen auf die Pläne, die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fff28-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fff28-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fff28-137">Relationships</span></span>
| <span data-ttu-id="fff28-138">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fff28-138">Relationship</span></span> | <span data-ttu-id="fff28-139">Typ</span><span class="sxs-lookup"><span data-stu-id="fff28-139">Type</span></span>   |<span data-ttu-id="fff28-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fff28-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fff28-141">tasks</span><span class="sxs-lookup"><span data-stu-id="fff28-141">tasks</span></span>|<span data-ttu-id="fff28-142">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fff28-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fff28-p103">Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="fff28-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="fff28-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="fff28-146">favoritePlans</span></span>|<span data-ttu-id="fff28-147">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fff28-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="fff28-148">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fff28-148">Read-only.</span></span> <span data-ttu-id="fff28-149">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="fff28-149">Nullable.</span></span> <span data-ttu-id="fff28-150">Gibt die [PlannerPlans](plannerplan.md) , die der Benutzer als Favoriten gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="fff28-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="fff28-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="fff28-151">recentPlans</span></span>|<span data-ttu-id="fff28-152">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fff28-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="fff28-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fff28-153">Read-only.</span></span> <span data-ttu-id="fff28-154">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="fff28-154">Nullable.</span></span> <span data-ttu-id="fff28-155">Gibt die [PlannerPlans](plannerplan.md) , die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fff28-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fff28-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fff28-156">JSON representation</span></span>
<span data-ttu-id="fff28-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fff28-157">The following is a JSON representation of the resource.</span></span>

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
