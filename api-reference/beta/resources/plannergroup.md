---
title: plannerGroup-Ressourcentyp
description: Die Ressource **PlannerGroup** bietet Zugriff auf Ressourcen Planner für eine Gruppe. Es enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 54b6b1d61a98aae3918fd3fcb888f470179ece15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961708"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="734e9-104">plannerGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="734e9-104">plannerGroup resource type</span></span>

> <span data-ttu-id="734e9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="734e9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="734e9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="734e9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="734e9-p103">Die **plannerGroup**-Ressource bietet einer [Gruppe](group.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="734e9-p103">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="734e9-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="734e9-109">Methods</span></span>

| <span data-ttu-id="734e9-110">Methode</span><span class="sxs-lookup"><span data-stu-id="734e9-110">Method</span></span>           | <span data-ttu-id="734e9-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="734e9-111">Return Type</span></span>    |<span data-ttu-id="734e9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="734e9-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="734e9-113">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="734e9-113">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="734e9-114">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="734e9-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="734e9-115">Dient zum Abrufen einer **plannerPlan**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="734e9-115">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="734e9-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="734e9-116">Properties</span></span>
| <span data-ttu-id="734e9-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="734e9-117">Property</span></span>     | <span data-ttu-id="734e9-118">Typ</span><span class="sxs-lookup"><span data-stu-id="734e9-118">Type</span></span>   |<span data-ttu-id="734e9-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="734e9-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="734e9-120">id</span><span class="sxs-lookup"><span data-stu-id="734e9-120">id</span></span>|<span data-ttu-id="734e9-121">String</span><span class="sxs-lookup"><span data-stu-id="734e9-121">String</span></span>| <span data-ttu-id="734e9-p104">Schreibgeschützt. Bezeichner der **plannerGroup**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="734e9-p104">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="734e9-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="734e9-124">Relationships</span></span>
| <span data-ttu-id="734e9-125">Beziehung</span><span class="sxs-lookup"><span data-stu-id="734e9-125">Relationship</span></span> | <span data-ttu-id="734e9-126">Typ</span><span class="sxs-lookup"><span data-stu-id="734e9-126">Type</span></span>   |<span data-ttu-id="734e9-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="734e9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="734e9-128">plans</span><span class="sxs-lookup"><span data-stu-id="734e9-128">plans</span></span>|<span data-ttu-id="734e9-129">[plannerPlan](plannerplan.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="734e9-129">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="734e9-p105">Schreibgeschützt. Lässt Nullwerte zu. Gibt die [plannerPlans](plannerplan.md) im Besitz der Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="734e9-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="734e9-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="734e9-133">JSON representation</span></span>
<span data-ttu-id="734e9-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="734e9-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
