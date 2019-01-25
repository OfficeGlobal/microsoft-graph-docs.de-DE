---
title: plannerCategoryDescriptions-Ressourcentyp
description: 'Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum planDetails-Objekt. Es können bis zu 6 Kategorien definiert werden. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 33031dc3c688e1fefb34109cb0a4a303dbe1c183
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521236"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="2da89-105">plannerCategoryDescriptions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2da89-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2da89-p102">Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum [planDetails](plannerplandetails.md)-Objekt. Es können bis zu 6 Kategorien definiert werden.</span><span class="sxs-lookup"><span data-stu-id="2da89-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="2da89-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2da89-109">Properties</span></span>
| <span data-ttu-id="2da89-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2da89-110">Property</span></span>     | <span data-ttu-id="2da89-111">Typ</span><span class="sxs-lookup"><span data-stu-id="2da89-111">Type</span></span>   |<span data-ttu-id="2da89-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2da89-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2da89-113">category1</span><span class="sxs-lookup"><span data-stu-id="2da89-113">category1</span></span>|<span data-ttu-id="2da89-114">String</span><span class="sxs-lookup"><span data-stu-id="2da89-114">String</span></span>|<span data-ttu-id="2da89-115">Mit Kategorie 1 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="2da89-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="2da89-116">category2</span><span class="sxs-lookup"><span data-stu-id="2da89-116">category2</span></span>|<span data-ttu-id="2da89-117">String</span><span class="sxs-lookup"><span data-stu-id="2da89-117">String</span></span>|<span data-ttu-id="2da89-118">Mit Kategorie 2 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="2da89-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="2da89-119">category3</span><span class="sxs-lookup"><span data-stu-id="2da89-119">category3</span></span>|<span data-ttu-id="2da89-120">String</span><span class="sxs-lookup"><span data-stu-id="2da89-120">String</span></span>|<span data-ttu-id="2da89-121">Mit Kategorie 3 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="2da89-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="2da89-122">category4</span><span class="sxs-lookup"><span data-stu-id="2da89-122">category4</span></span>|<span data-ttu-id="2da89-123">String</span><span class="sxs-lookup"><span data-stu-id="2da89-123">String</span></span>|<span data-ttu-id="2da89-124">Mit Kategorie 4 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="2da89-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="2da89-125">category5</span><span class="sxs-lookup"><span data-stu-id="2da89-125">category5</span></span>|<span data-ttu-id="2da89-126">String</span><span class="sxs-lookup"><span data-stu-id="2da89-126">String</span></span>|<span data-ttu-id="2da89-127">Mit Kategorie 5 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="2da89-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="2da89-128">category6</span><span class="sxs-lookup"><span data-stu-id="2da89-128">category6</span></span>|<span data-ttu-id="2da89-129">String</span><span class="sxs-lookup"><span data-stu-id="2da89-129">String</span></span>|<span data-ttu-id="2da89-130">Mit Kategorie 6 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="2da89-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2da89-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2da89-131">JSON representation</span></span>
<span data-ttu-id="2da89-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2da89-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannercategorydescriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
