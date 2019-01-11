---
title: ChartSeriesFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für den Diagrammdatenreihe.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f8a4e5fab61da3dba1c02488ff6e3a8bfd0e8fa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815855"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="dfbce-103">ChartSeriesFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dfbce-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="dfbce-104">Kapselt die Formateigenschaften für den Diagrammdatenreihe.</span><span class="sxs-lookup"><span data-stu-id="dfbce-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="dfbce-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="dfbce-105">Methods</span></span>
<span data-ttu-id="dfbce-106">Keine</span><span class="sxs-lookup"><span data-stu-id="dfbce-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="dfbce-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dfbce-107">Properties</span></span>
<span data-ttu-id="dfbce-108">Keine</span><span class="sxs-lookup"><span data-stu-id="dfbce-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dfbce-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dfbce-109">Relationships</span></span>
| <span data-ttu-id="dfbce-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="dfbce-110">Relationship</span></span> | <span data-ttu-id="dfbce-111">Typ</span><span class="sxs-lookup"><span data-stu-id="dfbce-111">Type</span></span>   |<span data-ttu-id="dfbce-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfbce-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfbce-113">fill</span><span class="sxs-lookup"><span data-stu-id="dfbce-113">fill</span></span>|[<span data-ttu-id="dfbce-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="dfbce-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="dfbce-p101">Stellt die Füllung einer Diagrammdatenreihe dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dfbce-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="dfbce-117">line</span><span class="sxs-lookup"><span data-stu-id="dfbce-117">line</span></span>|[<span data-ttu-id="dfbce-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="dfbce-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="dfbce-p102">Die Zeilenformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dfbce-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dfbce-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dfbce-121">JSON representation</span></span>

<span data-ttu-id="dfbce-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dfbce-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
