---
title: ChartAxes-Ressourcentyp
description: Die Achsen des Diagramms.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 483a69f11425f3b8991305e6acdf6b970d0e2db1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976387"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="79d3f-103">ChartAxes-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="79d3f-103">ChartAxes resource type</span></span>

<span data-ttu-id="79d3f-104">Die Achsen des Diagramms.</span><span class="sxs-lookup"><span data-stu-id="79d3f-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="79d3f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="79d3f-105">Methods</span></span>
<span data-ttu-id="79d3f-106">Keine</span><span class="sxs-lookup"><span data-stu-id="79d3f-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="79d3f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79d3f-107">Properties</span></span>
<span data-ttu-id="79d3f-108">Keine</span><span class="sxs-lookup"><span data-stu-id="79d3f-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="79d3f-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="79d3f-109">Relationships</span></span>
| <span data-ttu-id="79d3f-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="79d3f-110">Relationship</span></span> | <span data-ttu-id="79d3f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="79d3f-111">Type</span></span>   |<span data-ttu-id="79d3f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79d3f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79d3f-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="79d3f-113">categoryAxis</span></span>|[<span data-ttu-id="79d3f-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="79d3f-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="79d3f-p101">Stellt die Rubrikenachse in einem Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="79d3f-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="79d3f-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="79d3f-117">seriesAxis</span></span>|[<span data-ttu-id="79d3f-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="79d3f-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="79d3f-p102">Stellt die Reihenachse eines dreidimensionalen Diagramms dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="79d3f-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="79d3f-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="79d3f-121">valueAxis</span></span>|[<span data-ttu-id="79d3f-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="79d3f-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="79d3f-p103">Stellt die Größenachse in einer Achse dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="79d3f-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79d3f-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79d3f-125">JSON representation</span></span>

<span data-ttu-id="79d3f-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79d3f-126">Here is a JSON representation of the resource.</span></span>

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
