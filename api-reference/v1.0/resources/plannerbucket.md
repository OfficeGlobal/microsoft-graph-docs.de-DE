---
title: plannerBucket-Ressourcentyp
description: ) für Aufgaben in einem Plan in Office 365. Er ist in einem PlannerPlan enthalten und kann eine Auflistung von PlannerTasks haben.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 8cfc25e5554b20d4f808c8929b53549f4c44d7a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982834"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="cea9a-104">plannerBucket-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cea9a-104">plannerBucket resource type</span></span>

<span data-ttu-id="cea9a-p102">Die **plannerBucket**-Ressource stellt einen Bucket (bzw. eine „benutzerdefinierte Spalte“) für Aufgaben in einem Plan in Office 365 dar. Sie ist in einem [plannerPlan](plannerplan.md) enthalten und kann eine Sammlung von [plannerTasks](plannertask.md) haben.</span><span class="sxs-lookup"><span data-stu-id="cea9a-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="cea9a-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="cea9a-107">Methods</span></span>

| <span data-ttu-id="cea9a-108">Methode</span><span class="sxs-lookup"><span data-stu-id="cea9a-108">Method</span></span>           | <span data-ttu-id="cea9a-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cea9a-109">Return Type</span></span>    |<span data-ttu-id="cea9a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cea9a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cea9a-111">plannerBucket abrufen</span><span class="sxs-lookup"><span data-stu-id="cea9a-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="cea9a-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="cea9a-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="cea9a-113">Dient zum Lesen der Eigenschaften und Beziehungen des **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cea9a-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="cea9a-114">plannerTasks auflisten</span><span class="sxs-lookup"><span data-stu-id="cea9a-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="cea9a-115">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cea9a-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="cea9a-116">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="cea9a-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="cea9a-117">Create</span><span class="sxs-lookup"><span data-stu-id="cea9a-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="cea9a-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="cea9a-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="cea9a-119">Dient zum Erstellen eines neuen **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cea9a-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="cea9a-120">Update</span><span class="sxs-lookup"><span data-stu-id="cea9a-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="cea9a-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="cea9a-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="cea9a-122">Dient zum Aktualisieren eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cea9a-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="cea9a-123">Delete</span><span class="sxs-lookup"><span data-stu-id="cea9a-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="cea9a-124">Keine</span><span class="sxs-lookup"><span data-stu-id="cea9a-124">None</span></span> |<span data-ttu-id="cea9a-125">Dient zum Löschen eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cea9a-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cea9a-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cea9a-126">Properties</span></span>
| <span data-ttu-id="cea9a-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cea9a-127">Property</span></span>     | <span data-ttu-id="cea9a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="cea9a-128">Type</span></span>   |<span data-ttu-id="cea9a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cea9a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cea9a-130">id</span><span class="sxs-lookup"><span data-stu-id="cea9a-130">id</span></span>|<span data-ttu-id="cea9a-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cea9a-131">String</span></span>| <span data-ttu-id="cea9a-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cea9a-132">Read-only.</span></span> <span data-ttu-id="cea9a-133">ID des Bucket.</span><span class="sxs-lookup"><span data-stu-id="cea9a-133">ID of the bucket.</span></span> <span data-ttu-id="cea9a-134">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="cea9a-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="cea9a-135">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="cea9a-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="cea9a-136">name</span><span class="sxs-lookup"><span data-stu-id="cea9a-136">name</span></span>|<span data-ttu-id="cea9a-137">String</span><span class="sxs-lookup"><span data-stu-id="cea9a-137">String</span></span>|<span data-ttu-id="cea9a-138">Name des Buckets.</span><span class="sxs-lookup"><span data-stu-id="cea9a-138">Name of the bucket.</span></span>|
|<span data-ttu-id="cea9a-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="cea9a-139">orderHint</span></span>|<span data-ttu-id="cea9a-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cea9a-140">String</span></span>|<span data-ttu-id="cea9a-p104">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="cea9a-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="cea9a-143">planId</span><span class="sxs-lookup"><span data-stu-id="cea9a-143">planId</span></span>|<span data-ttu-id="cea9a-144">String</span><span class="sxs-lookup"><span data-stu-id="cea9a-144">String</span></span>|<span data-ttu-id="cea9a-145">Plan-ID, zu der der Bucket gehört.</span><span class="sxs-lookup"><span data-stu-id="cea9a-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cea9a-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cea9a-146">Relationships</span></span>
| <span data-ttu-id="cea9a-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="cea9a-147">Relationship</span></span> | <span data-ttu-id="cea9a-148">Typ</span><span class="sxs-lookup"><span data-stu-id="cea9a-148">Type</span></span>   |<span data-ttu-id="cea9a-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cea9a-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cea9a-150">tasks</span><span class="sxs-lookup"><span data-stu-id="cea9a-150">tasks</span></span>|<span data-ttu-id="cea9a-151">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cea9a-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="cea9a-p105">Schreibgeschützt. Lässt Nullwerte zu. Die Sammlung von Aufgaben im Bucket.</span><span class="sxs-lookup"><span data-stu-id="cea9a-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cea9a-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cea9a-155">JSON representation</span></span>
<span data-ttu-id="cea9a-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cea9a-156">Here is a JSON representation of the resource.</span></span>

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
