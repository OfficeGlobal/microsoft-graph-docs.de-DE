---
title: plannerPlan-Ressourcentyp
description: Die Ressource **PlannerPlan** stellt einen Plan in Office 365. Ein Plan kann eine Gruppe Besitz und enthält eine Auflistung von PlannerTasks. Sie können auch eine Auflistung von PlannerBuckets verfügen. Jedes Plan-Objekt ist ein Details-Objekt, das Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter Planner.
ms.openlocfilehash: cd2990bc42929c4c501e676d05d7d643dd6f7d3d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019836"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="7e750-107">plannerPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7e750-107">plannerPlan resource type</span></span>

<span data-ttu-id="7e750-p102">Die **plannerPlan**-Ressource stellt einen Plan in Office 365 dar. Ein Plan kann im Besitz einer [Gruppe](group.md) sein und enthält eine Sammlung von [plannerTasks](plannertask.md). Er kann auch über eine Sammlung von [plannerBuckets](plannerbucket.md) verfügen. Jedes Planobjekt verfügt über [details](plannerplandetails.md)-Objekt, das weitere Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Plänen und Aufgaben finden Sie unter [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="7e750-p102">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md). It can also have a collection of [plannerBuckets](plannerbucket.md). Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7e750-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="7e750-113">Methods</span></span>

| <span data-ttu-id="7e750-114">Methode</span><span class="sxs-lookup"><span data-stu-id="7e750-114">Method</span></span>           | <span data-ttu-id="7e750-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7e750-115">Return Type</span></span>    |<span data-ttu-id="7e750-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e750-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e750-117">plannerPlan abrufen</span><span class="sxs-lookup"><span data-stu-id="7e750-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="7e750-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="7e750-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="7e750-119">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7e750-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="7e750-120">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="7e750-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="7e750-121">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7e750-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="7e750-122">Dient zum Abrufen einer **plannerBucket**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="7e750-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="7e750-123">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="7e750-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="7e750-124">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7e750-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7e750-125">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="7e750-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="7e750-126">Update</span><span class="sxs-lookup"><span data-stu-id="7e750-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="7e750-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="7e750-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="7e750-128">Dient zum Aktualisieren eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7e750-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7e750-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e750-129">Properties</span></span>
| <span data-ttu-id="7e750-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e750-130">Property</span></span>     | <span data-ttu-id="7e750-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7e750-131">Type</span></span>   |<span data-ttu-id="7e750-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e750-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e750-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e750-133">createdDateTime</span></span>|<span data-ttu-id="7e750-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e750-134">DateTimeOffset</span></span>|<span data-ttu-id="7e750-p103">Schreibgeschützt. Datum und Uhrzeit der Erstellung des Plans. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7e750-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7e750-139">id</span><span class="sxs-lookup"><span data-stu-id="7e750-139">id</span></span>|<span data-ttu-id="7e750-140">String</span><span class="sxs-lookup"><span data-stu-id="7e750-140">String</span></span>| <span data-ttu-id="7e750-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7e750-141">Read-only.</span></span> <span data-ttu-id="7e750-142">ID des Plans.</span><span class="sxs-lookup"><span data-stu-id="7e750-142">ID of the plan.</span></span> <span data-ttu-id="7e750-143">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="7e750-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="7e750-144">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="7e750-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="7e750-145">owner</span><span class="sxs-lookup"><span data-stu-id="7e750-145">owner</span></span>|<span data-ttu-id="7e750-146">String</span><span class="sxs-lookup"><span data-stu-id="7e750-146">String</span></span>|<span data-ttu-id="7e750-147">Die ID der [Gruppe](group.md) , die den Plan besitzt.</span><span class="sxs-lookup"><span data-stu-id="7e750-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="7e750-148">Eine gültige Gruppe muss vorhanden sein, bevor Sie dieses Feld festgelegt werden kann.</span><span class="sxs-lookup"><span data-stu-id="7e750-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="7e750-149">Diese Eigenschaft kann nicht aktualisiert werden, nachdem er festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="7e750-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="7e750-150">title</span><span class="sxs-lookup"><span data-stu-id="7e750-150">title</span></span>|<span data-ttu-id="7e750-151">String</span><span class="sxs-lookup"><span data-stu-id="7e750-151">String</span></span>|<span data-ttu-id="7e750-p106">Erforderlich.  Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="7e750-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="7e750-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="7e750-154">createdBy</span></span>|[<span data-ttu-id="7e750-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="7e750-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="7e750-p107">Schreibgeschützt. Der Benutzer, der den Plan erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="7e750-p107">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e750-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7e750-158">Relationships</span></span>
| <span data-ttu-id="7e750-159">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7e750-159">Relationship</span></span> | <span data-ttu-id="7e750-160">Typ</span><span class="sxs-lookup"><span data-stu-id="7e750-160">Type</span></span>   |<span data-ttu-id="7e750-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e750-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e750-162">buckets</span><span class="sxs-lookup"><span data-stu-id="7e750-162">buckets</span></span>|<span data-ttu-id="7e750-163">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7e750-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="7e750-p108">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Buckets im Plan.</span><span class="sxs-lookup"><span data-stu-id="7e750-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="7e750-167">Details</span><span class="sxs-lookup"><span data-stu-id="7e750-167">details</span></span>|[<span data-ttu-id="7e750-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7e750-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="7e750-p109">Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über den Plan.</span><span class="sxs-lookup"><span data-stu-id="7e750-p109">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="7e750-172">tasks</span><span class="sxs-lookup"><span data-stu-id="7e750-172">tasks</span></span>|<span data-ttu-id="7e750-173">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7e750-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7e750-p110">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Aufgaben im Plan.</span><span class="sxs-lookup"><span data-stu-id="7e750-p110">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e750-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e750-177">JSON representation</span></span>

<span data-ttu-id="7e750-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e750-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->