---
title: Ressourcentyp plannerPlanContextDetails
description: Die Ressource **PlannerPlanContextDetails** enthält zusätzliche Informationen zu einer PlannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 025e5b1623333d0235ae83e061e30247a3d130f6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520249"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="b714e-103">Ressourcentyp plannerPlanContextDetails</span><span class="sxs-lookup"><span data-stu-id="b714e-103">plannerPlanContextDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b714e-104">Die Ressource **PlannerPlanContextDetails** enthält zusätzliche Informationen zu einer [PlannerPlanContext](plannerplancontext.md).</span><span class="sxs-lookup"><span data-stu-id="b714e-104">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b714e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b714e-105">Properties</span></span>
| <span data-ttu-id="b714e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b714e-106">Property</span></span>     | <span data-ttu-id="b714e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b714e-107">Type</span></span>   |<span data-ttu-id="b714e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b714e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b714e-109">url</span><span class="sxs-lookup"><span data-stu-id="b714e-109">url</span></span>|<span data-ttu-id="b714e-110">String</span><span class="sxs-lookup"><span data-stu-id="b714e-110">String</span></span>|<span data-ttu-id="b714e-111">URL des Benutzererlebnisses durch die zugeordneten [PlannerPlanContext](plannerplancontext.md)dargestellt.</span><span class="sxs-lookup"><span data-stu-id="b714e-111">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b714e-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b714e-112">JSON representation</span></span>

<span data-ttu-id="b714e-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b714e-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
