---
title: plannerUser-Ressourcentyp
description: 'Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen Benutzer. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526879"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="46327-103">plannerUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="46327-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46327-104">Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen [Benutzer](user.md).</span><span class="sxs-lookup"><span data-stu-id="46327-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="46327-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="46327-105">Methods</span></span>

| <span data-ttu-id="46327-106">Methode</span><span class="sxs-lookup"><span data-stu-id="46327-106">Method</span></span>           | <span data-ttu-id="46327-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="46327-107">Return Type</span></span>    |<span data-ttu-id="46327-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46327-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46327-109">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="46327-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="46327-110">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="46327-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="46327-111">Rufen Sie die [PlannerTasks](plannertask.md) die ihm zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="46327-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="46327-112">Liste favoritePlans</span><span class="sxs-lookup"><span data-stu-id="46327-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="46327-113">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="46327-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="46327-114">Rufen Sie die [PlannerPlans](plannerplan.md) durch den Benutzer als bevorzugten markiert.</span><span class="sxs-lookup"><span data-stu-id="46327-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="46327-115">Liste recentPlans</span><span class="sxs-lookup"><span data-stu-id="46327-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="46327-116">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="46327-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="46327-117">Rufen Sie die [PlannerPlans](plannerplan.md) zuletzt vom Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="46327-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="46327-118">Update</span><span class="sxs-lookup"><span data-stu-id="46327-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="46327-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="46327-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="46327-120">Aktualisieren eines **PlannerUser** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="46327-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="46327-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46327-121">Properties</span></span>
| <span data-ttu-id="46327-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46327-122">Property</span></span>     | <span data-ttu-id="46327-123">Typ</span><span class="sxs-lookup"><span data-stu-id="46327-123">Type</span></span>   |<span data-ttu-id="46327-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46327-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46327-125">id</span><span class="sxs-lookup"><span data-stu-id="46327-125">id</span></span>|<span data-ttu-id="46327-126">String</span><span class="sxs-lookup"><span data-stu-id="46327-126">String</span></span>| <span data-ttu-id="46327-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="46327-127">Read-only.</span></span> <span data-ttu-id="46327-128">Bezeichner des der plannerUser</span><span class="sxs-lookup"><span data-stu-id="46327-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="46327-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="46327-129">favoritePlanReferences</span></span>|[<span data-ttu-id="46327-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="46327-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="46327-131">Eine Auflistung mit der Verweise auf die Pläne, die der Benutzer als Favoriten gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="46327-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="46327-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="46327-132">recentPlanReferences</span></span>|[<span data-ttu-id="46327-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="46327-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="46327-134">Eine Auflistung mit Verweisen auf die Pläne, die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="46327-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46327-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="46327-135">Relationships</span></span>
| <span data-ttu-id="46327-136">Beziehung</span><span class="sxs-lookup"><span data-stu-id="46327-136">Relationship</span></span> | <span data-ttu-id="46327-137">Typ</span><span class="sxs-lookup"><span data-stu-id="46327-137">Type</span></span>   |<span data-ttu-id="46327-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46327-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46327-139">tasks</span><span class="sxs-lookup"><span data-stu-id="46327-139">tasks</span></span>|<span data-ttu-id="46327-140">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="46327-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="46327-p102">Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="46327-p102">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="46327-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="46327-144">favoritePlans</span></span>|<span data-ttu-id="46327-145">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="46327-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="46327-146">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="46327-146">Read-only.</span></span> <span data-ttu-id="46327-147">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="46327-147">Nullable.</span></span> <span data-ttu-id="46327-148">Gibt die [PlannerPlans](plannerplan.md) , die der Benutzer als Favoriten gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="46327-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="46327-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="46327-149">recentPlans</span></span>|<span data-ttu-id="46327-150">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="46327-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="46327-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="46327-151">Read-only.</span></span> <span data-ttu-id="46327-152">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="46327-152">Nullable.</span></span> <span data-ttu-id="46327-153">Gibt die [PlannerPlans](plannerplan.md) , die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="46327-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46327-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46327-154">JSON representation</span></span>
<span data-ttu-id="46327-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46327-155">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
