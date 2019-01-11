---
title: plannerBucket-Ressourcentyp
description: ) für Aufgaben in einem Plan in Office 365. Er ist in einem PlannerPlan enthalten und kann eine Auflistung von PlannerTasks haben.
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 4868fb3925fa3ae94571d5cc93b0da12434b00dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808120"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="3cc6a-104">plannerBucket-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3cc6a-104">plannerBucket resource type</span></span>

> <span data-ttu-id="3cc6a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cc6a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3cc6a-p103">Die **plannerBucket**-Ressource stellt einen Bucket (bzw. eine „benutzerdefinierte Spalte“) für Aufgaben in einem Plan in Office 365 dar. Sie ist in einem [plannerPlan](plannerplan.md) enthalten und kann eine Sammlung von [plannerTasks](plannertask.md) haben.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-p103">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="3cc6a-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="3cc6a-109">Methods</span></span>

| <span data-ttu-id="3cc6a-110">Methode</span><span class="sxs-lookup"><span data-stu-id="3cc6a-110">Method</span></span>           | <span data-ttu-id="3cc6a-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3cc6a-111">Return Type</span></span>    |<span data-ttu-id="3cc6a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cc6a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3cc6a-113">plannerBucket abrufen</span><span class="sxs-lookup"><span data-stu-id="3cc6a-113">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="3cc6a-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3cc6a-114">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="3cc6a-115">Dient zum Lesen der Eigenschaften und Beziehungen des **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-115">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="3cc6a-116">plannerTasks auflisten</span><span class="sxs-lookup"><span data-stu-id="3cc6a-116">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="3cc6a-117">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3cc6a-117">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3cc6a-118">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-118">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="3cc6a-119">Create</span><span class="sxs-lookup"><span data-stu-id="3cc6a-119">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="3cc6a-120">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3cc6a-120">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="3cc6a-121">Dient zum Erstellen eines neuen **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-121">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="3cc6a-122">Update</span><span class="sxs-lookup"><span data-stu-id="3cc6a-122">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="3cc6a-123">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3cc6a-123">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="3cc6a-124">Dient zum Aktualisieren eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-124">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="3cc6a-125">Delete</span><span class="sxs-lookup"><span data-stu-id="3cc6a-125">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="3cc6a-126">Keine</span><span class="sxs-lookup"><span data-stu-id="3cc6a-126">None</span></span> |<span data-ttu-id="3cc6a-127">Dient zum Löschen eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-127">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3cc6a-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3cc6a-128">Properties</span></span>
| <span data-ttu-id="3cc6a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3cc6a-129">Property</span></span>     | <span data-ttu-id="3cc6a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3cc6a-130">Type</span></span>   |<span data-ttu-id="3cc6a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cc6a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cc6a-132">id</span><span class="sxs-lookup"><span data-stu-id="3cc6a-132">id</span></span>|<span data-ttu-id="3cc6a-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cc6a-133">String</span></span>| <span data-ttu-id="3cc6a-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-134">Read-only.</span></span> <span data-ttu-id="3cc6a-135">ID des Bucket.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-135">ID of the bucket.</span></span> <span data-ttu-id="3cc6a-136">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-136">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="3cc6a-137">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-137">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="3cc6a-138">name</span><span class="sxs-lookup"><span data-stu-id="3cc6a-138">name</span></span>|<span data-ttu-id="3cc6a-139">String</span><span class="sxs-lookup"><span data-stu-id="3cc6a-139">String</span></span>|<span data-ttu-id="3cc6a-140">Name des Buckets.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-140">Name of the bucket.</span></span>|
|<span data-ttu-id="3cc6a-141">orderHint</span><span class="sxs-lookup"><span data-stu-id="3cc6a-141">orderHint</span></span>|<span data-ttu-id="3cc6a-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3cc6a-142">String</span></span>|<span data-ttu-id="3cc6a-p105">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="3cc6a-145">planId</span><span class="sxs-lookup"><span data-stu-id="3cc6a-145">planId</span></span>|<span data-ttu-id="3cc6a-146">String</span><span class="sxs-lookup"><span data-stu-id="3cc6a-146">String</span></span>|<span data-ttu-id="3cc6a-147">Plan-ID, zu der der Bucket gehört.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-147">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cc6a-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3cc6a-148">Relationships</span></span>
| <span data-ttu-id="3cc6a-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3cc6a-149">Relationship</span></span> | <span data-ttu-id="3cc6a-150">Typ</span><span class="sxs-lookup"><span data-stu-id="3cc6a-150">Type</span></span>   |<span data-ttu-id="3cc6a-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cc6a-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cc6a-152">tasks</span><span class="sxs-lookup"><span data-stu-id="3cc6a-152">tasks</span></span>|<span data-ttu-id="3cc6a-153">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3cc6a-153">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3cc6a-p106">Schreibgeschützt. Lässt Nullwerte zu. Die Sammlung von Aufgaben im Bucket.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-p106">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cc6a-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3cc6a-157">JSON representation</span></span>
<span data-ttu-id="3cc6a-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3cc6a-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
