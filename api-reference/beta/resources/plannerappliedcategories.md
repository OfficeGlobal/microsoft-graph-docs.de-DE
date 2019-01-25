---
title: plannerAppliedCategories-Ressourcentyp
description: Die Ressource **AppliedCategoriesCollection** stellt die Auflistung von Kategorien (oder Etiketten), die mit einer Aufgabe angewendet wurden. Es ist Teil des PlannerTask-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b4e3ae92d179669d449d33c34ade4ae4476570fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517666"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="fd5b0-104">plannerAppliedCategories-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd5b0-104">plannerAppliedCategories resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd5b0-p102">Die **AppliedCategoriesCollection**-Ressource stellt die Sammlung von Kategorien (oder Bezeichnungen) dar, die auf eine Aufgabe angewendet wurden. Sie ist Teil des [plannerTask](plannertask.md)-Objekts. Auf eine Aufgabe können bis zu 6 Kategorien angewendet werden. Kategoriebeschreibungen wie `category1`, `category2` usw. sind Teil des [planDetails ](plannerplandetails.md)-Objekts. Es handelt sich um einen offenen Typ.</span><span class="sxs-lookup"><span data-stu-id="fd5b0-p102">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object. There can be up to 6 categories applied to a task. Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object. This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="fd5b0-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd5b0-110">Properties</span></span>
<span data-ttu-id="fd5b0-p103">Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch `category1`, `category2`, `category3`, `category4`, `category5` und/oder `category6` als Eigenschaften angeben, deren Wert das boolesche `true` ist, wenn die entsprechenden Kategorien auf die Aufgabe angewendet werden. Nachfolgend ein Beispiel. Wenn sie nicht zutreffen, werden Eigenschaften automatisch entfernt, indem ihre Werte auf das boolesche `false` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="fd5b0-p103">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="fd5b0-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd5b0-115">JSON representation</span></span>

<span data-ttu-id="fd5b0-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd5b0-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="fd5b0-117">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="fd5b0-117">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerappliedcategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
