---
title: ChartAxes-Ressourcentyp
description: Die Achsen des Diagramms.
ms.openlocfilehash: 4fc801ecdba147a26b30f07a2487eabe11acfb3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016926"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="652f1-103">ChartAxes-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="652f1-103">ChartAxes resource type</span></span>

<span data-ttu-id="652f1-104">Die Achsen des Diagramms.</span><span class="sxs-lookup"><span data-stu-id="652f1-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="652f1-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="652f1-105">Methods</span></span>
<span data-ttu-id="652f1-106">Keine</span><span class="sxs-lookup"><span data-stu-id="652f1-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="652f1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="652f1-107">Properties</span></span>
<span data-ttu-id="652f1-108">Keine</span><span class="sxs-lookup"><span data-stu-id="652f1-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="652f1-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="652f1-109">Relationships</span></span>
| <span data-ttu-id="652f1-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="652f1-110">Relationship</span></span> | <span data-ttu-id="652f1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="652f1-111">Type</span></span>   |<span data-ttu-id="652f1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="652f1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="652f1-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="652f1-113">categoryAxis</span></span>|[<span data-ttu-id="652f1-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="652f1-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="652f1-p101">Stellt die Rubrikenachse in einem Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="652f1-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="652f1-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="652f1-117">seriesAxis</span></span>|[<span data-ttu-id="652f1-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="652f1-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="652f1-p102">Stellt die Reihenachse eines dreidimensionalen Diagramms dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="652f1-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="652f1-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="652f1-121">valueAxis</span></span>|[<span data-ttu-id="652f1-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="652f1-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="652f1-p103">Stellt die Größenachse in einer Achse dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="652f1-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="652f1-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="652f1-125">JSON representation</span></span>

<span data-ttu-id="652f1-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="652f1-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->