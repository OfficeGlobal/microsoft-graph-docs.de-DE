---
title: plannerUser-Ressourcentyp
description: Die Ressource **PlannerUser** bieten Zugriff auf Ressourcen Planner für einen Benutzer. Es enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953560"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="bfb56-104">plannerUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bfb56-104">plannerUser resource type</span></span>

<span data-ttu-id="bfb56-p102">Die **plannerUser**-Ressource bietet einem [Benutzer](user.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="bfb56-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="bfb56-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="bfb56-107">Methods</span></span>

| <span data-ttu-id="bfb56-108">Methode</span><span class="sxs-lookup"><span data-stu-id="bfb56-108">Method</span></span>           | <span data-ttu-id="bfb56-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bfb56-109">Return Type</span></span>    |<span data-ttu-id="bfb56-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfb56-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bfb56-111">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="bfb56-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="bfb56-112">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfb56-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="bfb56-113">Dient zum Abrufen einer **plannerPlan**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="bfb56-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="bfb56-114">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="bfb56-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="bfb56-115">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfb56-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="bfb56-116">Dient zum Abrufen einer **plannerTask**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="bfb56-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="bfb56-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bfb56-117">Properties</span></span>
| <span data-ttu-id="bfb56-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bfb56-118">Property</span></span>     | <span data-ttu-id="bfb56-119">Typ</span><span class="sxs-lookup"><span data-stu-id="bfb56-119">Type</span></span>   |<span data-ttu-id="bfb56-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfb56-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfb56-121">id</span><span class="sxs-lookup"><span data-stu-id="bfb56-121">id</span></span>|<span data-ttu-id="bfb56-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfb56-122">String</span></span>| <span data-ttu-id="bfb56-p103">Schreibgeschützt. Bezeichner der plannerUser-Ressource.</span><span class="sxs-lookup"><span data-stu-id="bfb56-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfb56-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bfb56-125">Relationships</span></span>
| <span data-ttu-id="bfb56-126">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bfb56-126">Relationship</span></span> | <span data-ttu-id="bfb56-127">Typ</span><span class="sxs-lookup"><span data-stu-id="bfb56-127">Type</span></span>   |<span data-ttu-id="bfb56-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfb56-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfb56-129">plans</span><span class="sxs-lookup"><span data-stu-id="bfb56-129">plans</span></span>|<span data-ttu-id="bfb56-130">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfb56-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="bfb56-p104">Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="bfb56-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="bfb56-134">tasks</span><span class="sxs-lookup"><span data-stu-id="bfb56-134">tasks</span></span>|<span data-ttu-id="bfb56-135">[plannerTask](plannertask.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfb56-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="bfb56-p105">Schreibgeschützt. Lässt Nullwerte zu. Gibt die für den Benutzer freigegebenen [plannerPlans](plannerplan.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="bfb56-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfb56-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bfb56-139">JSON representation</span></span>
<span data-ttu-id="bfb56-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bfb56-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
