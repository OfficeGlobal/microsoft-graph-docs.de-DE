---
title: FilterCriteria-Ressourcentyp
description: Stellt die auf eine Spalte angewendeten Filterkriterien dar.
localization_priority: Normal
ms.openlocfilehash: 27fd3b6b211934c2cc81a11f203287c530993dde
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808568"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="511bc-103">FilterCriteria-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="511bc-103">FilterCriteria resource type</span></span>

<span data-ttu-id="511bc-104">Stellt die auf eine Spalte angewendeten Filterkriterien dar.</span><span class="sxs-lookup"><span data-stu-id="511bc-104">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="511bc-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="511bc-105">JSON representation</span></span>

<span data-ttu-id="511bc-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="511bc-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "icon": {"@odata.type": "microsoft.graph.workbookIcon"},
  "values": {"@odata.type": "microsoft.graph.Json"}
}

```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'color' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion1' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion2' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'dynamicCriteria' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'filterOn' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'icon' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'values' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table."
  ]
} -->
