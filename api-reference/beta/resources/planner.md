---
title: planner-Ressourcentyp
description: Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523400"
---
# <a name="planner-resource-type"></a><span data-ttu-id="fdbbe-105">planner-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fdbbe-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdbbe-p102">Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="fdbbe-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="fdbbe-109">Methods</span></span>

| <span data-ttu-id="fdbbe-110">Methode</span><span class="sxs-lookup"><span data-stu-id="fdbbe-110">Method</span></span>           | <span data-ttu-id="fdbbe-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fdbbe-111">Return Type</span></span>    |<span data-ttu-id="fdbbe-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdbbe-113">plannerBucket erstellen</span><span class="sxs-lookup"><span data-stu-id="fdbbe-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="fdbbe-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fdbbe-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="fdbbe-115">Dient zum Erstellen eines neuen **plannerBucket** durch Veröffentlichung in der buckets-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="fdbbe-116">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="fdbbe-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="fdbbe-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fdbbe-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="fdbbe-118">Dient zum Erstellen eines neuen **plannerPlan** durch Veröffentlichung in der plans-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="fdbbe-119">plannerTask erstellen</span><span class="sxs-lookup"><span data-stu-id="fdbbe-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="fdbbe-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="fdbbe-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="fdbbe-121">Dient zum Erstellen einer neuen **plannerTask** durch Veröffentlichung in der tasks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdbbe-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdbbe-122">Properties</span></span>
| <span data-ttu-id="fdbbe-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdbbe-123">Property</span></span>     | <span data-ttu-id="fdbbe-124">Typ</span><span class="sxs-lookup"><span data-stu-id="fdbbe-124">Type</span></span>   |<span data-ttu-id="fdbbe-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdbbe-126">id</span><span class="sxs-lookup"><span data-stu-id="fdbbe-126">id</span></span>|<span data-ttu-id="fdbbe-127">String</span><span class="sxs-lookup"><span data-stu-id="fdbbe-127">String</span></span>| <span data-ttu-id="fdbbe-p103">Schreibgeschützt. Bezeichner der **planner**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-p103">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdbbe-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdbbe-130">Relationships</span></span>
| <span data-ttu-id="fdbbe-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-131">Relationship</span></span> | <span data-ttu-id="fdbbe-132">Typ</span><span class="sxs-lookup"><span data-stu-id="fdbbe-132">Type</span></span>   |<span data-ttu-id="fdbbe-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdbbe-134">buckets</span><span class="sxs-lookup"><span data-stu-id="fdbbe-134">buckets</span></span>|<span data-ttu-id="fdbbe-135">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="fdbbe-p104">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen einfaches zurück.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-p104">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="fdbbe-139">plans</span><span class="sxs-lookup"><span data-stu-id="fdbbe-139">plans</span></span>|<span data-ttu-id="fdbbe-140">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="fdbbe-p105">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Pläne zurück.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-p105">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="fdbbe-144">tasks</span><span class="sxs-lookup"><span data-stu-id="fdbbe-144">tasks</span></span>|<span data-ttu-id="fdbbe-145">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fdbbe-p106">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Aufgaben zurück.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-p106">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdbbe-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdbbe-149">JSON representation</span></span>
<span data-ttu-id="fdbbe-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdbbe-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planner.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
