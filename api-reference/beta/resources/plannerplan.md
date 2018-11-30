---
title: plannerPlan-Ressourcentyp
description: Die Ressource **PlannerPlan** stellt einen Plan in Office 365. Ein Plan kann eine Gruppe Besitz und enthält eine Auflistung von PlannerTasks. Sie können auch eine Auflistung von PlannerBuckets verfügen. Jedes Plan-Objekt ist ein Details-Objekt, das Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter Planner.
ms.openlocfilehash: 236b6cb5d35e11a30bcb4371e0563b56ac93de8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060346"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="c9f49-107">plannerPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c9f49-107">plannerPlan resource type</span></span>

> <span data-ttu-id="c9f49-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9f49-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9f49-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9f49-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9f49-110">Die Ressource **PlannerPlan** stellt einen Plan in Office 365.</span><span class="sxs-lookup"><span data-stu-id="c9f49-110">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="c9f49-111">Ein Plan kann eine [Gruppe](group.md) Besitz und enthält eine Auflistung von [PlannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="c9f49-111">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="c9f49-112">Sie können auch eine Auflistung von [PlannerBuckets](plannerbucket.md)verfügen.</span><span class="sxs-lookup"><span data-stu-id="c9f49-112">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="c9f49-113">Jedes Plan-Objekt ist ein [Details](plannerplandetails.md) -Objekt, das Informationen über den Plan enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="c9f49-113">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="c9f49-114">Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c9f49-114">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="c9f49-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="c9f49-115">Methods</span></span>

| <span data-ttu-id="c9f49-116">Methode</span><span class="sxs-lookup"><span data-stu-id="c9f49-116">Method</span></span>           | <span data-ttu-id="c9f49-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c9f49-117">Return Type</span></span>    |<span data-ttu-id="c9f49-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9f49-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9f49-119">plannerPlan abrufen</span><span class="sxs-lookup"><span data-stu-id="c9f49-119">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="c9f49-120">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c9f49-120">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c9f49-121">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9f49-121">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="c9f49-122">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="c9f49-122">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="c9f49-123">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c9f49-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c9f49-124">Dient zum Abrufen einer **plannerBucket**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="c9f49-124">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="c9f49-125">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="c9f49-125">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="c9f49-126">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c9f49-126">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c9f49-127">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="c9f49-127">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="c9f49-128">Update</span><span class="sxs-lookup"><span data-stu-id="c9f49-128">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="c9f49-129">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c9f49-129">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c9f49-130">Dient zum Aktualisieren eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9f49-130">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c9f49-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9f49-131">Properties</span></span>
| <span data-ttu-id="c9f49-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9f49-132">Property</span></span>     | <span data-ttu-id="c9f49-133">Typ</span><span class="sxs-lookup"><span data-stu-id="c9f49-133">Type</span></span>   |<span data-ttu-id="c9f49-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9f49-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9f49-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9f49-135">createdDateTime</span></span>|<span data-ttu-id="c9f49-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9f49-136">DateTimeOffset</span></span>|<span data-ttu-id="c9f49-p104">Schreibgeschützt. Datum und Uhrzeit der Erstellung des Plans. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c9f49-p104">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9f49-141">id</span><span class="sxs-lookup"><span data-stu-id="c9f49-141">id</span></span>|<span data-ttu-id="c9f49-142">String</span><span class="sxs-lookup"><span data-stu-id="c9f49-142">String</span></span>| <span data-ttu-id="c9f49-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c9f49-143">Read-only.</span></span> <span data-ttu-id="c9f49-144">ID des Plans.</span><span class="sxs-lookup"><span data-stu-id="c9f49-144">ID of the plan.</span></span> <span data-ttu-id="c9f49-145">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="c9f49-145">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c9f49-146">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="c9f49-146">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c9f49-147">owner</span><span class="sxs-lookup"><span data-stu-id="c9f49-147">owner</span></span>|<span data-ttu-id="c9f49-148">String</span><span class="sxs-lookup"><span data-stu-id="c9f49-148">String</span></span>|<span data-ttu-id="c9f49-149">Die ID der [Gruppe](group.md) , die den Plan besitzt.</span><span class="sxs-lookup"><span data-stu-id="c9f49-149">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="c9f49-150">Eine gültige Gruppe muss vorhanden sein, bevor Sie dieses Feld festgelegt werden kann.</span><span class="sxs-lookup"><span data-stu-id="c9f49-150">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="c9f49-151">Diese Eigenschaft kann nicht aktualisiert werden, nachdem er festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="c9f49-151">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="c9f49-152">title</span><span class="sxs-lookup"><span data-stu-id="c9f49-152">title</span></span>|<span data-ttu-id="c9f49-153">String</span><span class="sxs-lookup"><span data-stu-id="c9f49-153">String</span></span>|<span data-ttu-id="c9f49-p107">Erforderlich.  Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="c9f49-p107">Required. Title of the plan.</span></span>|
|<span data-ttu-id="c9f49-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="c9f49-156">createdBy</span></span>|[<span data-ttu-id="c9f49-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="c9f49-157">identitySet</span></span>](identityset.md)|<span data-ttu-id="c9f49-p108">Schreibgeschützt. Der Benutzer, der den Plan erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="c9f49-p108">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="c9f49-160">Kontext</span><span class="sxs-lookup"><span data-stu-id="c9f49-160">contexts</span></span>|[<span data-ttu-id="c9f49-161">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="c9f49-161">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="c9f49-162">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c9f49-162">Read-only.</span></span> <span data-ttu-id="c9f49-163">Zusätzliche Benutzererlebnis, in denen dieser Plan verwendet wird, dargestellt als [PlannerPlanContext](plannerplancontext.md) Einträge.</span><span class="sxs-lookup"><span data-stu-id="c9f49-163">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9f49-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9f49-164">Relationships</span></span>
| <span data-ttu-id="c9f49-165">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c9f49-165">Relationship</span></span> | <span data-ttu-id="c9f49-166">Typ</span><span class="sxs-lookup"><span data-stu-id="c9f49-166">Type</span></span>   |<span data-ttu-id="c9f49-167">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9f49-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9f49-168">buckets</span><span class="sxs-lookup"><span data-stu-id="c9f49-168">buckets</span></span>|<span data-ttu-id="c9f49-169">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c9f49-169">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c9f49-p110">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Buckets im Plan.</span><span class="sxs-lookup"><span data-stu-id="c9f49-p110">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="c9f49-173">Details</span><span class="sxs-lookup"><span data-stu-id="c9f49-173">details</span></span>|[<span data-ttu-id="c9f49-174">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c9f49-174">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="c9f49-p111">Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über den Plan.</span><span class="sxs-lookup"><span data-stu-id="c9f49-p111">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="c9f49-178">tasks</span><span class="sxs-lookup"><span data-stu-id="c9f49-178">tasks</span></span>|<span data-ttu-id="c9f49-179">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c9f49-179">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c9f49-p112">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Aufgaben im Plan.</span><span class="sxs-lookup"><span data-stu-id="c9f49-p112">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9f49-183">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9f49-183">JSON representation</span></span>

<span data-ttu-id="c9f49-184">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9f49-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
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