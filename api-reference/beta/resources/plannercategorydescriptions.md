---
title: plannerCategoryDescriptions-Ressourcentyp
description: 'Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum planDetails-Objekt. Es können bis zu 6 Kategorien definiert werden. '
localization_priority: Normal
ms.openlocfilehash: ebfe1fc69ccd143d6f84afab9c5c2ed2054df3d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882754"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="634d8-105">plannerCategoryDescriptions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="634d8-105">plannerCategoryDescriptions resource type</span></span>

> <span data-ttu-id="634d8-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="634d8-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="634d8-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="634d8-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="634d8-p103">Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum [planDetails](plannerplandetails.md)-Objekt. Es können bis zu 6 Kategorien definiert werden.</span><span class="sxs-lookup"><span data-stu-id="634d8-p103">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="634d8-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="634d8-111">Properties</span></span>
| <span data-ttu-id="634d8-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="634d8-112">Property</span></span>     | <span data-ttu-id="634d8-113">Typ</span><span class="sxs-lookup"><span data-stu-id="634d8-113">Type</span></span>   |<span data-ttu-id="634d8-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="634d8-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="634d8-115">category1</span><span class="sxs-lookup"><span data-stu-id="634d8-115">category1</span></span>|<span data-ttu-id="634d8-116">String</span><span class="sxs-lookup"><span data-stu-id="634d8-116">String</span></span>|<span data-ttu-id="634d8-117">Mit Kategorie 1 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="634d8-117">The label associated with Category 1</span></span>|
|<span data-ttu-id="634d8-118">category2</span><span class="sxs-lookup"><span data-stu-id="634d8-118">category2</span></span>|<span data-ttu-id="634d8-119">String</span><span class="sxs-lookup"><span data-stu-id="634d8-119">String</span></span>|<span data-ttu-id="634d8-120">Mit Kategorie 2 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="634d8-120">The label associated with Category 2</span></span>|
|<span data-ttu-id="634d8-121">category3</span><span class="sxs-lookup"><span data-stu-id="634d8-121">category3</span></span>|<span data-ttu-id="634d8-122">String</span><span class="sxs-lookup"><span data-stu-id="634d8-122">String</span></span>|<span data-ttu-id="634d8-123">Mit Kategorie 3 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="634d8-123">The label associated with Category 3</span></span>|
|<span data-ttu-id="634d8-124">category4</span><span class="sxs-lookup"><span data-stu-id="634d8-124">category4</span></span>|<span data-ttu-id="634d8-125">String</span><span class="sxs-lookup"><span data-stu-id="634d8-125">String</span></span>|<span data-ttu-id="634d8-126">Mit Kategorie 4 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="634d8-126">The label associated with Category 4</span></span>|
|<span data-ttu-id="634d8-127">category5</span><span class="sxs-lookup"><span data-stu-id="634d8-127">category5</span></span>|<span data-ttu-id="634d8-128">String</span><span class="sxs-lookup"><span data-stu-id="634d8-128">String</span></span>|<span data-ttu-id="634d8-129">Mit Kategorie 5 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="634d8-129">The label associated with Category 5</span></span>|
|<span data-ttu-id="634d8-130">category6</span><span class="sxs-lookup"><span data-stu-id="634d8-130">category6</span></span>|<span data-ttu-id="634d8-131">String</span><span class="sxs-lookup"><span data-stu-id="634d8-131">String</span></span>|<span data-ttu-id="634d8-132">Mit Kategorie 6 verknüpfte Bezeichnung.</span><span class="sxs-lookup"><span data-stu-id="634d8-132">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="634d8-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="634d8-133">JSON representation</span></span>
<span data-ttu-id="634d8-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="634d8-134">Here is a JSON representation of the resource.</span></span>

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
