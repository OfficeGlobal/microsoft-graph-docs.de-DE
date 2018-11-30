---
title: planner-Ressourcentyp
description: Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.
ms.openlocfilehash: e5980f6f4037b57e977b12ef223e8a5a2cf7c77c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019329"
---
# <a name="planner-resource-type"></a><span data-ttu-id="a1298-105">planner-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1298-105">planner resource type</span></span>

<span data-ttu-id="a1298-p102">Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="a1298-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="a1298-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="a1298-109">Methods</span></span>

| <span data-ttu-id="a1298-110">Methode</span><span class="sxs-lookup"><span data-stu-id="a1298-110">Method</span></span>           | <span data-ttu-id="a1298-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a1298-111">Return Type</span></span>    |<span data-ttu-id="a1298-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1298-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1298-113">plannerBucket erstellen</span><span class="sxs-lookup"><span data-stu-id="a1298-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="a1298-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="a1298-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="a1298-115">Dient zum Erstellen eines neuen **plannerBucket** durch Veröffentlichung in der buckets-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="a1298-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="a1298-116">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="a1298-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="a1298-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a1298-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="a1298-118">Dient zum Erstellen eines neuen **plannerPlan** durch Veröffentlichung in der plans-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="a1298-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="a1298-119">plannerTask erstellen</span><span class="sxs-lookup"><span data-stu-id="a1298-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="a1298-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="a1298-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="a1298-121">Dient zum Erstellen einer neuen **plannerTask** durch Veröffentlichung in der tasks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="a1298-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1298-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a1298-122">Relationships</span></span>
| <span data-ttu-id="a1298-123">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a1298-123">Relationship</span></span> | <span data-ttu-id="a1298-124">Typ</span><span class="sxs-lookup"><span data-stu-id="a1298-124">Type</span></span>   |<span data-ttu-id="a1298-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1298-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1298-126">buckets</span><span class="sxs-lookup"><span data-stu-id="a1298-126">buckets</span></span>|<span data-ttu-id="a1298-127">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a1298-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a1298-p103">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen einfaches zurück.</span><span class="sxs-lookup"><span data-stu-id="a1298-p103">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="a1298-131">plans</span><span class="sxs-lookup"><span data-stu-id="a1298-131">plans</span></span>|<span data-ttu-id="a1298-132">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a1298-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="a1298-p104">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Pläne zurück.</span><span class="sxs-lookup"><span data-stu-id="a1298-p104">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="a1298-136">tasks</span><span class="sxs-lookup"><span data-stu-id="a1298-136">tasks</span></span>|<span data-ttu-id="a1298-137">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a1298-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a1298-p105">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Aufgaben zurück.</span><span class="sxs-lookup"><span data-stu-id="a1298-p105">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1298-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1298-141">JSON representation</span></span>
<span data-ttu-id="a1298-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1298-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="a1298-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1298-143">Example</span></span>

<span data-ttu-id="a1298-144">Die **Planner** -Ressource ist im Stamm des Diagramms verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a1298-144">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->