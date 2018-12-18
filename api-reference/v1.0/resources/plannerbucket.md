---
title: plannerBucket-Ressourcentyp
description: ) für Aufgaben in einem Plan in Office 365. Er ist in einem PlannerPlan enthalten und kann eine Auflistung von PlannerTasks haben.
author: TarkanSevilmis
ms.openlocfilehash: 09c9fab569a819f0545e5c851da12be98b45b150
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331444"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="e4050-104">plannerBucket-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e4050-104">plannerBucket resource type</span></span>

<span data-ttu-id="e4050-p102">Die **plannerBucket**-Ressource stellt einen Bucket (bzw. eine „benutzerdefinierte Spalte“) für Aufgaben in einem Plan in Office 365 dar. Sie ist in einem [plannerPlan](plannerplan.md) enthalten und kann eine Sammlung von [plannerTasks](plannertask.md) haben.</span><span class="sxs-lookup"><span data-stu-id="e4050-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="e4050-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="e4050-107">Methods</span></span>

| <span data-ttu-id="e4050-108">Methode</span><span class="sxs-lookup"><span data-stu-id="e4050-108">Method</span></span>           | <span data-ttu-id="e4050-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e4050-109">Return Type</span></span>    |<span data-ttu-id="e4050-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4050-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4050-111">plannerBucket abrufen</span><span class="sxs-lookup"><span data-stu-id="e4050-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="e4050-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e4050-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="e4050-113">Dient zum Lesen der Eigenschaften und Beziehungen des **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4050-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="e4050-114">plannerTasks auflisten</span><span class="sxs-lookup"><span data-stu-id="e4050-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="e4050-115">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e4050-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e4050-116">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="e4050-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="e4050-117">Create</span><span class="sxs-lookup"><span data-stu-id="e4050-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="e4050-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e4050-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="e4050-119">Dient zum Erstellen eines neuen **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4050-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="e4050-120">Update</span><span class="sxs-lookup"><span data-stu-id="e4050-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="e4050-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e4050-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="e4050-122">Dient zum Aktualisieren eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4050-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="e4050-123">Delete</span><span class="sxs-lookup"><span data-stu-id="e4050-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="e4050-124">Keine</span><span class="sxs-lookup"><span data-stu-id="e4050-124">None</span></span> |<span data-ttu-id="e4050-125">Dient zum Löschen eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4050-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4050-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e4050-126">Properties</span></span>
| <span data-ttu-id="e4050-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4050-127">Property</span></span>     | <span data-ttu-id="e4050-128">Typ</span><span class="sxs-lookup"><span data-stu-id="e4050-128">Type</span></span>   |<span data-ttu-id="e4050-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4050-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4050-130">id</span><span class="sxs-lookup"><span data-stu-id="e4050-130">id</span></span>|<span data-ttu-id="e4050-131">String</span><span class="sxs-lookup"><span data-stu-id="e4050-131">String</span></span>| <span data-ttu-id="e4050-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e4050-132">Read-only.</span></span> <span data-ttu-id="e4050-133">ID des Bucket.</span><span class="sxs-lookup"><span data-stu-id="e4050-133">ID of the bucket.</span></span> <span data-ttu-id="e4050-134">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="e4050-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e4050-135">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="e4050-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e4050-136">name</span><span class="sxs-lookup"><span data-stu-id="e4050-136">name</span></span>|<span data-ttu-id="e4050-137">String</span><span class="sxs-lookup"><span data-stu-id="e4050-137">String</span></span>|<span data-ttu-id="e4050-138">Name des Buckets.</span><span class="sxs-lookup"><span data-stu-id="e4050-138">Name of the bucket.</span></span>|
|<span data-ttu-id="e4050-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="e4050-139">orderHint</span></span>|<span data-ttu-id="e4050-140">String</span><span class="sxs-lookup"><span data-stu-id="e4050-140">String</span></span>|<span data-ttu-id="e4050-p104">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="e4050-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e4050-143">planId</span><span class="sxs-lookup"><span data-stu-id="e4050-143">planId</span></span>|<span data-ttu-id="e4050-144">String</span><span class="sxs-lookup"><span data-stu-id="e4050-144">String</span></span>|<span data-ttu-id="e4050-145">Plan-ID, zu der der Bucket gehört.</span><span class="sxs-lookup"><span data-stu-id="e4050-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4050-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e4050-146">Relationships</span></span>
| <span data-ttu-id="e4050-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e4050-147">Relationship</span></span> | <span data-ttu-id="e4050-148">Typ</span><span class="sxs-lookup"><span data-stu-id="e4050-148">Type</span></span>   |<span data-ttu-id="e4050-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4050-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4050-150">tasks</span><span class="sxs-lookup"><span data-stu-id="e4050-150">tasks</span></span>|<span data-ttu-id="e4050-151">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e4050-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e4050-p105">Schreibgeschützt. Lässt Nullwerte zu. Die Sammlung von Aufgaben im Bucket.</span><span class="sxs-lookup"><span data-stu-id="e4050-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4050-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e4050-155">JSON representation</span></span>
<span data-ttu-id="e4050-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e4050-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->