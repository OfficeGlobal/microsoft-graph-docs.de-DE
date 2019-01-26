---
title: ChartAxes-Ressourcentyp
description: Die Achsen des Diagramms.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2a3744e38ffebef0c28784c0fd4be8f35b8af23
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570862"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="94a45-103">ChartAxes-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="94a45-103">ChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a45-104">Die Achsen des Diagramms.</span><span class="sxs-lookup"><span data-stu-id="94a45-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="94a45-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="94a45-105">Methods</span></span>
<span data-ttu-id="94a45-106">Keine</span><span class="sxs-lookup"><span data-stu-id="94a45-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="94a45-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94a45-107">Properties</span></span>
<span data-ttu-id="94a45-108">Keine</span><span class="sxs-lookup"><span data-stu-id="94a45-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="94a45-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94a45-109">Relationships</span></span>
| <span data-ttu-id="94a45-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="94a45-110">Relationship</span></span> | <span data-ttu-id="94a45-111">Typ</span><span class="sxs-lookup"><span data-stu-id="94a45-111">Type</span></span>   |<span data-ttu-id="94a45-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94a45-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94a45-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="94a45-113">categoryAxis</span></span>|[<span data-ttu-id="94a45-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="94a45-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="94a45-p101">Stellt die Rubrikenachse in einem Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94a45-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="94a45-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="94a45-117">seriesAxis</span></span>|[<span data-ttu-id="94a45-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="94a45-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="94a45-p102">Stellt die Reihenachse eines dreidimensionalen Diagramms dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94a45-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="94a45-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="94a45-121">valueAxis</span></span>|[<span data-ttu-id="94a45-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="94a45-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="94a45-p103">Stellt die Größenachse in einer Achse dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94a45-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94a45-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94a45-125">JSON representation</span></span>

<span data-ttu-id="94a45-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94a45-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
