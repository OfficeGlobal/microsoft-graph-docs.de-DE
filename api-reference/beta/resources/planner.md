---
title: planner-Ressourcentyp
description: Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: cf2877d5f413f3e54e1e0e750da1f22d6f9ffd95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925182"
---
# <a name="planner-resource-type"></a><span data-ttu-id="92063-105">planner-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="92063-105">planner resource type</span></span>

> <span data-ttu-id="92063-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92063-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92063-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92063-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92063-p103">Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="92063-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="92063-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="92063-111">Methods</span></span>

| <span data-ttu-id="92063-112">Methode</span><span class="sxs-lookup"><span data-stu-id="92063-112">Method</span></span>           | <span data-ttu-id="92063-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="92063-113">Return Type</span></span>    |<span data-ttu-id="92063-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92063-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92063-115">plannerBucket erstellen</span><span class="sxs-lookup"><span data-stu-id="92063-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="92063-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="92063-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="92063-117">Dient zum Erstellen eines neuen **plannerBucket** durch Veröffentlichung in der buckets-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="92063-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="92063-118">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="92063-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="92063-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="92063-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="92063-120">Dient zum Erstellen eines neuen **plannerPlan** durch Veröffentlichung in der plans-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="92063-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="92063-121">plannerTask erstellen</span><span class="sxs-lookup"><span data-stu-id="92063-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="92063-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="92063-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="92063-123">Dient zum Erstellen einer neuen **plannerTask** durch Veröffentlichung in der tasks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="92063-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="92063-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92063-124">Properties</span></span>
| <span data-ttu-id="92063-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92063-125">Property</span></span>     | <span data-ttu-id="92063-126">Typ</span><span class="sxs-lookup"><span data-stu-id="92063-126">Type</span></span>   |<span data-ttu-id="92063-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92063-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92063-128">id</span><span class="sxs-lookup"><span data-stu-id="92063-128">id</span></span>|<span data-ttu-id="92063-129">String</span><span class="sxs-lookup"><span data-stu-id="92063-129">String</span></span>| <span data-ttu-id="92063-p104">Schreibgeschützt. Bezeichner der **planner**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="92063-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92063-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="92063-132">Relationships</span></span>
| <span data-ttu-id="92063-133">Beziehung</span><span class="sxs-lookup"><span data-stu-id="92063-133">Relationship</span></span> | <span data-ttu-id="92063-134">Typ</span><span class="sxs-lookup"><span data-stu-id="92063-134">Type</span></span>   |<span data-ttu-id="92063-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92063-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92063-136">buckets</span><span class="sxs-lookup"><span data-stu-id="92063-136">buckets</span></span>|<span data-ttu-id="92063-137">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="92063-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="92063-p105">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen einfaches zurück.</span><span class="sxs-lookup"><span data-stu-id="92063-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="92063-141">plans</span><span class="sxs-lookup"><span data-stu-id="92063-141">plans</span></span>|<span data-ttu-id="92063-142">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="92063-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="92063-p106">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Pläne zurück.</span><span class="sxs-lookup"><span data-stu-id="92063-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="92063-146">tasks</span><span class="sxs-lookup"><span data-stu-id="92063-146">tasks</span></span>|<span data-ttu-id="92063-147">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="92063-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="92063-p107">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Aufgaben zurück.</span><span class="sxs-lookup"><span data-stu-id="92063-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92063-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92063-151">JSON representation</span></span>
<span data-ttu-id="92063-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92063-152">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
