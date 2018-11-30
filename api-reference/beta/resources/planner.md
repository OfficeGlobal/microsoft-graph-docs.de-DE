---
title: planner-Ressourcentyp
description: Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.
ms.openlocfilehash: c076eda1660cef9e31f584e5fe439f916eba81d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065996"
---
# <a name="planner-resource-type"></a><span data-ttu-id="f0a05-105">planner-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f0a05-105">planner resource type</span></span>

> <span data-ttu-id="f0a05-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f0a05-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0a05-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f0a05-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0a05-p103">Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="f0a05-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="f0a05-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="f0a05-111">Methods</span></span>

| <span data-ttu-id="f0a05-112">Methode</span><span class="sxs-lookup"><span data-stu-id="f0a05-112">Method</span></span>           | <span data-ttu-id="f0a05-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f0a05-113">Return Type</span></span>    |<span data-ttu-id="f0a05-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0a05-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0a05-115">plannerBucket erstellen</span><span class="sxs-lookup"><span data-stu-id="f0a05-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="f0a05-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="f0a05-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="f0a05-117">Dient zum Erstellen eines neuen **plannerBucket** durch Veröffentlichung in der buckets-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="f0a05-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="f0a05-118">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="f0a05-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="f0a05-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="f0a05-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="f0a05-120">Dient zum Erstellen eines neuen **plannerPlan** durch Veröffentlichung in der plans-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="f0a05-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="f0a05-121">plannerTask erstellen</span><span class="sxs-lookup"><span data-stu-id="f0a05-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="f0a05-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="f0a05-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="f0a05-123">Dient zum Erstellen einer neuen **plannerTask** durch Veröffentlichung in der tasks-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="f0a05-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0a05-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f0a05-124">Properties</span></span>
| <span data-ttu-id="f0a05-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0a05-125">Property</span></span>     | <span data-ttu-id="f0a05-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f0a05-126">Type</span></span>   |<span data-ttu-id="f0a05-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0a05-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0a05-128">id</span><span class="sxs-lookup"><span data-stu-id="f0a05-128">id</span></span>|<span data-ttu-id="f0a05-129">String</span><span class="sxs-lookup"><span data-stu-id="f0a05-129">String</span></span>| <span data-ttu-id="f0a05-p104">Schreibgeschützt. Bezeichner der **planner**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0a05-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0a05-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f0a05-132">Relationships</span></span>
| <span data-ttu-id="f0a05-133">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f0a05-133">Relationship</span></span> | <span data-ttu-id="f0a05-134">Typ</span><span class="sxs-lookup"><span data-stu-id="f0a05-134">Type</span></span>   |<span data-ttu-id="f0a05-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0a05-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0a05-136">buckets</span><span class="sxs-lookup"><span data-stu-id="f0a05-136">buckets</span></span>|<span data-ttu-id="f0a05-137">[plannerBucket](plannerbucket.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f0a05-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="f0a05-p105">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen einfaches zurück.</span><span class="sxs-lookup"><span data-stu-id="f0a05-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="f0a05-141">plans</span><span class="sxs-lookup"><span data-stu-id="f0a05-141">plans</span></span>|<span data-ttu-id="f0a05-142">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f0a05-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f0a05-p106">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Pläne zurück.</span><span class="sxs-lookup"><span data-stu-id="f0a05-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="f0a05-146">tasks</span><span class="sxs-lookup"><span data-stu-id="f0a05-146">tasks</span></span>|<span data-ttu-id="f0a05-147">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f0a05-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f0a05-p107">Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Aufgaben zurück.</span><span class="sxs-lookup"><span data-stu-id="f0a05-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0a05-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f0a05-151">JSON representation</span></span>
<span data-ttu-id="f0a05-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0a05-152">Here is a JSON representation of the resource.</span></span>

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