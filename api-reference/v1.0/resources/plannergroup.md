---
title: plannerGroup-Ressourcentyp
description: Die Ressource **PlannerGroup** bietet Zugriff auf Ressourcen Planner für eine Gruppe. Es enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
ms.openlocfilehash: ac55c0acd3561205654383cbb1b3d264c219d1a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871967"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="0f7a8-104">plannerGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f7a8-104">plannerGroup resource type</span></span>

<span data-ttu-id="0f7a8-p102">Die **plannerGroup**-Ressource bietet einer [Gruppe](group.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="0f7a8-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="0f7a8-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="0f7a8-107">Methods</span></span>

| <span data-ttu-id="0f7a8-108">Methode</span><span class="sxs-lookup"><span data-stu-id="0f7a8-108">Method</span></span>           | <span data-ttu-id="0f7a8-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0f7a8-109">Return Type</span></span>    |<span data-ttu-id="0f7a8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f7a8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f7a8-111">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="0f7a8-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="0f7a8-112">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0f7a8-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="0f7a8-113">Dient zum Abrufen einer **plannerPlan**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="0f7a8-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f7a8-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f7a8-114">Properties</span></span>
| <span data-ttu-id="0f7a8-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f7a8-115">Property</span></span>     | <span data-ttu-id="0f7a8-116">Typ</span><span class="sxs-lookup"><span data-stu-id="0f7a8-116">Type</span></span>   |<span data-ttu-id="0f7a8-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f7a8-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f7a8-118">id</span><span class="sxs-lookup"><span data-stu-id="0f7a8-118">id</span></span>|<span data-ttu-id="0f7a8-119">String</span><span class="sxs-lookup"><span data-stu-id="0f7a8-119">String</span></span>| <span data-ttu-id="0f7a8-p103">Schreibgeschützt. Bezeichner der **plannerGroup**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f7a8-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f7a8-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f7a8-122">Relationships</span></span>
| <span data-ttu-id="0f7a8-123">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0f7a8-123">Relationship</span></span> | <span data-ttu-id="0f7a8-124">Typ</span><span class="sxs-lookup"><span data-stu-id="0f7a8-124">Type</span></span>   |<span data-ttu-id="0f7a8-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f7a8-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f7a8-126">plans</span><span class="sxs-lookup"><span data-stu-id="0f7a8-126">plans</span></span>|<span data-ttu-id="0f7a8-127">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0f7a8-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="0f7a8-p104">Schreibgeschützt. Lässt Nullwerte zu. Gibt die [plannerPlans](plannerplan.md) im Besitz der Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="0f7a8-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f7a8-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f7a8-131">JSON representation</span></span>
<span data-ttu-id="0f7a8-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f7a8-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
