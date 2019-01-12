---
title: plannerCategoryDescriptions-Ressourcentyp
description: 'Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum planDetails-Objekt. Es können bis zu 6 Kategorien definiert werden. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1cf1ee1c6e8ccc4e90f78985b352062fce37df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984346"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="e1120-105">plannerCategoryDescriptions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e1120-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="e1120-p102">Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum [planDetails](plannerplandetails.md)-Objekt. Es können bis zu 6 Kategorien definiert werden.</span><span class="sxs-lookup"><span data-stu-id="e1120-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="e1120-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1120-109">Properties</span></span>
| <span data-ttu-id="e1120-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1120-110">Property</span></span>     | <span data-ttu-id="e1120-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e1120-111">Type</span></span>   |<span data-ttu-id="e1120-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1120-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1120-113">category1</span><span class="sxs-lookup"><span data-stu-id="e1120-113">category1</span></span>|<span data-ttu-id="e1120-114">String</span><span class="sxs-lookup"><span data-stu-id="e1120-114">String</span></span>|<span data-ttu-id="e1120-115">Mit Kategorie 1 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e1120-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="e1120-116">category2</span><span class="sxs-lookup"><span data-stu-id="e1120-116">category2</span></span>|<span data-ttu-id="e1120-117">String</span><span class="sxs-lookup"><span data-stu-id="e1120-117">String</span></span>|<span data-ttu-id="e1120-118">Mit Kategorie 2 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e1120-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="e1120-119">category3</span><span class="sxs-lookup"><span data-stu-id="e1120-119">category3</span></span>|<span data-ttu-id="e1120-120">String</span><span class="sxs-lookup"><span data-stu-id="e1120-120">String</span></span>|<span data-ttu-id="e1120-121">Mit Kategorie 3 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e1120-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="e1120-122">category4</span><span class="sxs-lookup"><span data-stu-id="e1120-122">category4</span></span>|<span data-ttu-id="e1120-123">String</span><span class="sxs-lookup"><span data-stu-id="e1120-123">String</span></span>|<span data-ttu-id="e1120-124">Mit Kategorie 4 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e1120-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="e1120-125">category5</span><span class="sxs-lookup"><span data-stu-id="e1120-125">category5</span></span>|<span data-ttu-id="e1120-126">String</span><span class="sxs-lookup"><span data-stu-id="e1120-126">String</span></span>|<span data-ttu-id="e1120-127">Mit Kategorie 5 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e1120-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="e1120-128">category6</span><span class="sxs-lookup"><span data-stu-id="e1120-128">category6</span></span>|<span data-ttu-id="e1120-129">String</span><span class="sxs-lookup"><span data-stu-id="e1120-129">String</span></span>|<span data-ttu-id="e1120-130">Mit Kategorie 6 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="e1120-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1120-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1120-131">JSON representation</span></span>
<span data-ttu-id="e1120-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1120-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
