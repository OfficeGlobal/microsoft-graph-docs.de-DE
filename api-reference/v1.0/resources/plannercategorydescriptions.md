---
title: plannerCategoryDescriptions-Ressourcentyp
description: 'Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum planDetails-Objekt. Es können bis zu 6 Kategorien definiert werden. '
ms.openlocfilehash: e71cbd1f41d23747691b3738b5a46ff302a72168
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017025"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="20ea2-105">plannerCategoryDescriptions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="20ea2-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="20ea2-p102">Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum [planDetails](plannerplandetails.md)-Objekt. Es können bis zu 6 Kategorien definiert werden.</span><span class="sxs-lookup"><span data-stu-id="20ea2-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="20ea2-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20ea2-109">Properties</span></span>
| <span data-ttu-id="20ea2-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20ea2-110">Property</span></span>     | <span data-ttu-id="20ea2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="20ea2-111">Type</span></span>   |<span data-ttu-id="20ea2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20ea2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20ea2-113">category1</span><span class="sxs-lookup"><span data-stu-id="20ea2-113">category1</span></span>|<span data-ttu-id="20ea2-114">String</span><span class="sxs-lookup"><span data-stu-id="20ea2-114">String</span></span>|<span data-ttu-id="20ea2-115">Mit Kategorie 1 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="20ea2-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="20ea2-116">category2</span><span class="sxs-lookup"><span data-stu-id="20ea2-116">category2</span></span>|<span data-ttu-id="20ea2-117">String</span><span class="sxs-lookup"><span data-stu-id="20ea2-117">String</span></span>|<span data-ttu-id="20ea2-118">Mit Kategorie 2 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="20ea2-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="20ea2-119">category3</span><span class="sxs-lookup"><span data-stu-id="20ea2-119">category3</span></span>|<span data-ttu-id="20ea2-120">String</span><span class="sxs-lookup"><span data-stu-id="20ea2-120">String</span></span>|<span data-ttu-id="20ea2-121">Mit Kategorie 3 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="20ea2-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="20ea2-122">category4</span><span class="sxs-lookup"><span data-stu-id="20ea2-122">category4</span></span>|<span data-ttu-id="20ea2-123">String</span><span class="sxs-lookup"><span data-stu-id="20ea2-123">String</span></span>|<span data-ttu-id="20ea2-124">Mit Kategorie 4 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="20ea2-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="20ea2-125">category5</span><span class="sxs-lookup"><span data-stu-id="20ea2-125">category5</span></span>|<span data-ttu-id="20ea2-126">String</span><span class="sxs-lookup"><span data-stu-id="20ea2-126">String</span></span>|<span data-ttu-id="20ea2-127">Mit Kategorie 5 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="20ea2-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="20ea2-128">category6</span><span class="sxs-lookup"><span data-stu-id="20ea2-128">category6</span></span>|<span data-ttu-id="20ea2-129">String</span><span class="sxs-lookup"><span data-stu-id="20ea2-129">String</span></span>|<span data-ttu-id="20ea2-130">Mit Kategorie 6 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="20ea2-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20ea2-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20ea2-131">JSON representation</span></span>
<span data-ttu-id="20ea2-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20ea2-132">Here is a JSON representation of the resource.</span></span>

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