---
title: plannerPlan-Ressourcentyp
description: Die Ressource **PlannerPlan** stellt einen Plan in Office 365. Ein Plan kann eine Gruppe Besitz und enthält eine Auflistung von PlannerTasks. Sie können auch eine Auflistung von PlannerBuckets verfügen. Jedes Plan-Objekt ist ein Details-Objekt, das Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b5d95b1bfab7404007c3139833e54f155c10d9aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950522"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="62dbe-107">plannerPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="62dbe-107">plannerPlan resource type</span></span>

> <span data-ttu-id="62dbe-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="62dbe-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62dbe-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62dbe-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62dbe-110">Die Ressource **PlannerPlan** stellt einen Plan in Office 365.</span><span class="sxs-lookup"><span data-stu-id="62dbe-110">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="62dbe-111">Ein Plan kann eine [Gruppe](group.md) Besitz und enthält eine Auflistung von [PlannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="62dbe-111">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="62dbe-112">Sie können auch eine Auflistung von [PlannerBuckets](plannerbucket.md)verfügen.</span><span class="sxs-lookup"><span data-stu-id="62dbe-112">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="62dbe-113">Jedes Plan-Objekt ist ein [Details](plannerplandetails.md) -Objekt, das Informationen über den Plan enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="62dbe-113">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="62dbe-114">Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="62dbe-114">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="62dbe-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="62dbe-115">Methods</span></span>

| <span data-ttu-id="62dbe-116">Methode</span><span class="sxs-lookup"><span data-stu-id="62dbe-116">Method</span></span>           | <span data-ttu-id="62dbe-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="62dbe-117">Return Type</span></span>    |<span data-ttu-id="62dbe-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62dbe-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="62dbe-119">plannerPlan abrufen</span><span class="sxs-lookup"><span data-stu-id="62dbe-119">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="62dbe-120">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="62dbe-120">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="62dbe-121">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="62dbe-121">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="62dbe-122">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="62dbe-122">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="62dbe-123">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="62dbe-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="62dbe-124">Dient zum Abrufen einer **plannerBucket**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="62dbe-124">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="62dbe-125">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="62dbe-125">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="62dbe-126">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="62dbe-126">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="62dbe-127">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="62dbe-127">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="62dbe-128">Update</span><span class="sxs-lookup"><span data-stu-id="62dbe-128">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="62dbe-129">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="62dbe-129">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="62dbe-130">Dient zum Aktualisieren eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="62dbe-130">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="62dbe-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="62dbe-131">Properties</span></span>
| <span data-ttu-id="62dbe-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62dbe-132">Property</span></span>     | <span data-ttu-id="62dbe-133">Typ</span><span class="sxs-lookup"><span data-stu-id="62dbe-133">Type</span></span>   |<span data-ttu-id="62dbe-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62dbe-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62dbe-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62dbe-135">createdDateTime</span></span>|<span data-ttu-id="62dbe-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62dbe-136">DateTimeOffset</span></span>|<span data-ttu-id="62dbe-p104">Schreibgeschützt. Datum und Uhrzeit der Erstellung des Plans. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="62dbe-p104">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="62dbe-141">id</span><span class="sxs-lookup"><span data-stu-id="62dbe-141">id</span></span>|<span data-ttu-id="62dbe-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62dbe-142">String</span></span>| <span data-ttu-id="62dbe-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62dbe-143">Read-only.</span></span> <span data-ttu-id="62dbe-144">ID des Plans.</span><span class="sxs-lookup"><span data-stu-id="62dbe-144">ID of the plan.</span></span> <span data-ttu-id="62dbe-145">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="62dbe-145">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="62dbe-146">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="62dbe-146">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="62dbe-147">owner</span><span class="sxs-lookup"><span data-stu-id="62dbe-147">owner</span></span>|<span data-ttu-id="62dbe-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62dbe-148">String</span></span>|<span data-ttu-id="62dbe-149">Die ID der [Gruppe](group.md) , die den Plan besitzt.</span><span class="sxs-lookup"><span data-stu-id="62dbe-149">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="62dbe-150">Eine gültige Gruppe muss vorhanden sein, bevor Sie dieses Feld festgelegt werden kann.</span><span class="sxs-lookup"><span data-stu-id="62dbe-150">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="62dbe-151">Diese Eigenschaft kann nicht aktualisiert werden, nachdem er festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="62dbe-151">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="62dbe-152">title</span><span class="sxs-lookup"><span data-stu-id="62dbe-152">title</span></span>|<span data-ttu-id="62dbe-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62dbe-153">String</span></span>|<span data-ttu-id="62dbe-p107">Erforderlich.  Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="62dbe-p107">Required. Title of the plan.</span></span>|
|<span data-ttu-id="62dbe-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="62dbe-156">createdBy</span></span>|[<span data-ttu-id="62dbe-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="62dbe-157">identitySet</span></span>](identityset.md)|<span data-ttu-id="62dbe-p108">Schreibgeschützt. Der Benutzer, der den Plan erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="62dbe-p108">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="62dbe-160">Kontext</span><span class="sxs-lookup"><span data-stu-id="62dbe-160">contexts</span></span>|[<span data-ttu-id="62dbe-161">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="62dbe-161">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="62dbe-162">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62dbe-162">Read-only.</span></span> <span data-ttu-id="62dbe-163">Zusätzliche Benutzererlebnis, in denen dieser Plan verwendet wird, dargestellt als [PlannerPlanContext](plannerplancontext.md) Einträge.</span><span class="sxs-lookup"><span data-stu-id="62dbe-163">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62dbe-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="62dbe-164">Relationships</span></span>
| <span data-ttu-id="62dbe-165">Beziehung</span><span class="sxs-lookup"><span data-stu-id="62dbe-165">Relationship</span></span> | <span data-ttu-id="62dbe-166">Typ</span><span class="sxs-lookup"><span data-stu-id="62dbe-166">Type</span></span>   |<span data-ttu-id="62dbe-167">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62dbe-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62dbe-168">buckets</span><span class="sxs-lookup"><span data-stu-id="62dbe-168">buckets</span></span>|<span data-ttu-id="62dbe-169">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="62dbe-169">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="62dbe-p110">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Buckets im Plan.</span><span class="sxs-lookup"><span data-stu-id="62dbe-p110">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="62dbe-173">Details</span><span class="sxs-lookup"><span data-stu-id="62dbe-173">details</span></span>|[<span data-ttu-id="62dbe-174">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="62dbe-174">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="62dbe-p111">Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über den Plan.</span><span class="sxs-lookup"><span data-stu-id="62dbe-p111">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="62dbe-178">tasks</span><span class="sxs-lookup"><span data-stu-id="62dbe-178">tasks</span></span>|<span data-ttu-id="62dbe-179">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="62dbe-179">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="62dbe-p112">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Aufgaben im Plan.</span><span class="sxs-lookup"><span data-stu-id="62dbe-p112">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62dbe-183">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="62dbe-183">JSON representation</span></span>

<span data-ttu-id="62dbe-184">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="62dbe-184">Here is a JSON representation of the resource.</span></span>

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
