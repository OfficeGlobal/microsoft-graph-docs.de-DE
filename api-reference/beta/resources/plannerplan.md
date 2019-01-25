---
title: plannerPlan-Ressourcentyp
description: Die Ressource **PlannerPlan** stellt einen Plan in Office 365. Ein Plan kann eine Gruppe Besitz und enthält eine Auflistung von PlannerTasks. Sie können auch eine Auflistung von PlannerBuckets verfügen. Jedes Plan-Objekt ist ein Details-Objekt, das Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529551"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="70c58-107">plannerPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="70c58-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70c58-108">Die Ressource **PlannerPlan** stellt einen Plan in Office 365.</span><span class="sxs-lookup"><span data-stu-id="70c58-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="70c58-109">Ein Plan kann eine [Gruppe](group.md) Besitz und enthält eine Auflistung von [PlannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="70c58-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="70c58-110">Sie können auch eine Auflistung von [PlannerBuckets](plannerbucket.md)verfügen.</span><span class="sxs-lookup"><span data-stu-id="70c58-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="70c58-111">Jedes Plan-Objekt ist ein [Details](plannerplandetails.md) -Objekt, das Informationen über den Plan enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="70c58-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="70c58-112">Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="70c58-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="70c58-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="70c58-113">Methods</span></span>

| <span data-ttu-id="70c58-114">Methode</span><span class="sxs-lookup"><span data-stu-id="70c58-114">Method</span></span>           | <span data-ttu-id="70c58-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="70c58-115">Return Type</span></span>    |<span data-ttu-id="70c58-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c58-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70c58-117">plannerPlan abrufen</span><span class="sxs-lookup"><span data-stu-id="70c58-117">[Get plannerPlan](../api/plannerplan-get.md)</span></span> | [<span data-ttu-id="70c58-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="70c58-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="70c58-119">Dient zum Lesen der Eigenschaften und Beziehungen eines plannerPlan-Objekts.</span><span class="sxs-lookup"><span data-stu-id="70c58-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|<span data-ttu-id="70c58-120">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="70c58-120">[List buckets](../api/plannerplan-list-buckets.md)</span></span> |<span data-ttu-id="70c58-121">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70c58-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="70c58-122">Dient zum Abrufen einer plannerBucket-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="70c58-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="70c58-123">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="70c58-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="70c58-124">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70c58-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="70c58-125">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="70c58-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="70c58-126">Update</span><span class="sxs-lookup"><span data-stu-id="70c58-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="70c58-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="70c58-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="70c58-128">Dient zum Aktualisieren eines plannerPlan-Objekts.</span><span class="sxs-lookup"><span data-stu-id="70c58-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="70c58-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70c58-129">Properties</span></span>
| <span data-ttu-id="70c58-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70c58-130">Property</span></span>     | <span data-ttu-id="70c58-131">Typ</span><span class="sxs-lookup"><span data-stu-id="70c58-131">Type</span></span>   |<span data-ttu-id="70c58-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c58-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70c58-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70c58-133">createdDateTime</span></span>|<span data-ttu-id="70c58-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c58-134">DateTimeOffset</span></span>|<span data-ttu-id="70c58-p103">Schreibgeschützt. Datum und Uhrzeit der Erstellung des Plans. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="70c58-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="70c58-139">id</span><span class="sxs-lookup"><span data-stu-id="70c58-139">id</span></span>|<span data-ttu-id="70c58-140">String</span><span class="sxs-lookup"><span data-stu-id="70c58-140">String</span></span>| <span data-ttu-id="70c58-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70c58-141">Read-only.</span></span> <span data-ttu-id="70c58-142">ID des Plans.</span><span class="sxs-lookup"><span data-stu-id="70c58-142">ID of the plan.</span></span> <span data-ttu-id="70c58-143">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="70c58-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="70c58-144">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="70c58-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="70c58-145">owner</span><span class="sxs-lookup"><span data-stu-id="70c58-145">owner</span></span>|<span data-ttu-id="70c58-146">String</span><span class="sxs-lookup"><span data-stu-id="70c58-146">String</span></span>|<span data-ttu-id="70c58-147">Die ID der [Gruppe](group.md) , die den Plan besitzt.</span><span class="sxs-lookup"><span data-stu-id="70c58-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="70c58-148">Eine gültige Gruppe muss vorhanden sein, bevor Sie dieses Feld festgelegt werden kann.</span><span class="sxs-lookup"><span data-stu-id="70c58-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="70c58-149">Diese Eigenschaft kann nicht aktualisiert werden, nachdem er festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="70c58-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="70c58-150">title</span><span class="sxs-lookup"><span data-stu-id="70c58-150">title</span></span>|<span data-ttu-id="70c58-151">String</span><span class="sxs-lookup"><span data-stu-id="70c58-151">String</span></span>|<span data-ttu-id="70c58-p106">Erforderlich.  Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="70c58-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="70c58-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="70c58-154">createdBy</span></span>|[<span data-ttu-id="70c58-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="70c58-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="70c58-p107">Schreibgeschützt. Der Benutzer, der den Plan erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="70c58-p107">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="70c58-158">Kontext</span><span class="sxs-lookup"><span data-stu-id="70c58-158">contexts</span></span>|[<span data-ttu-id="70c58-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="70c58-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="70c58-160">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70c58-160">Read-only.</span></span> <span data-ttu-id="70c58-161">Zusätzliche Benutzererlebnis, in denen dieser Plan verwendet wird, dargestellt als [PlannerPlanContext](plannerplancontext.md) Einträge.</span><span class="sxs-lookup"><span data-stu-id="70c58-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70c58-162">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="70c58-162">Relationships</span></span>
| <span data-ttu-id="70c58-163">Beziehung</span><span class="sxs-lookup"><span data-stu-id="70c58-163">Relationship</span></span> | <span data-ttu-id="70c58-164">Typ</span><span class="sxs-lookup"><span data-stu-id="70c58-164">Type</span></span>   |<span data-ttu-id="70c58-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c58-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70c58-166">buckets</span><span class="sxs-lookup"><span data-stu-id="70c58-166">buckets</span></span>|<span data-ttu-id="70c58-167">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70c58-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="70c58-p109">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Buckets im Plan.</span><span class="sxs-lookup"><span data-stu-id="70c58-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="70c58-171">Details</span><span class="sxs-lookup"><span data-stu-id="70c58-171">details</span></span>|[<span data-ttu-id="70c58-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="70c58-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="70c58-p110">Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über den Plan.</span><span class="sxs-lookup"><span data-stu-id="70c58-p110">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="70c58-176">tasks</span><span class="sxs-lookup"><span data-stu-id="70c58-176">tasks</span></span>|<span data-ttu-id="70c58-177">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70c58-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="70c58-p111">Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Aufgaben im Plan.</span><span class="sxs-lookup"><span data-stu-id="70c58-p111">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70c58-181">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70c58-181">JSON representation</span></span>

<span data-ttu-id="70c58-182">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70c58-182">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
