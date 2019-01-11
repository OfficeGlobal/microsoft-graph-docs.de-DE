---
title: ChartAxes-Ressourcentyp
description: Die Achsen des Diagramms.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 53f0e4a7344ddfab89330203f90032266e0c622d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885904"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="edf5a-103">ChartAxes-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="edf5a-103">ChartAxes resource type</span></span>

<span data-ttu-id="edf5a-104">Die Achsen des Diagramms.</span><span class="sxs-lookup"><span data-stu-id="edf5a-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="edf5a-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="edf5a-105">Methods</span></span>
<span data-ttu-id="edf5a-106">Keine</span><span class="sxs-lookup"><span data-stu-id="edf5a-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="edf5a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="edf5a-107">Properties</span></span>
<span data-ttu-id="edf5a-108">Keine</span><span class="sxs-lookup"><span data-stu-id="edf5a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="edf5a-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="edf5a-109">Relationships</span></span>
| <span data-ttu-id="edf5a-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="edf5a-110">Relationship</span></span> | <span data-ttu-id="edf5a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="edf5a-111">Type</span></span>   |<span data-ttu-id="edf5a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edf5a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edf5a-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="edf5a-113">categoryAxis</span></span>|[<span data-ttu-id="edf5a-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="edf5a-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="edf5a-p101">Stellt die Rubrikenachse in einem Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="edf5a-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="edf5a-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="edf5a-117">seriesAxis</span></span>|[<span data-ttu-id="edf5a-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="edf5a-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="edf5a-p102">Stellt die Reihenachse eines dreidimensionalen Diagramms dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="edf5a-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="edf5a-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="edf5a-121">valueAxis</span></span>|[<span data-ttu-id="edf5a-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="edf5a-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="edf5a-p103">Stellt die Größenachse in einer Achse dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="edf5a-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edf5a-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="edf5a-125">JSON representation</span></span>

<span data-ttu-id="edf5a-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="edf5a-126">Here is a JSON representation of the resource.</span></span>

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
