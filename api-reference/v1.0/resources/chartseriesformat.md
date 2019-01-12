---
title: ChartSeriesFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für den Diagrammdatenreihe.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fd342e55524d51b6a0382df8ca9310ea162308d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961435"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="379c1-103">ChartSeriesFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="379c1-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="379c1-104">Kapselt die Formateigenschaften für den Diagrammdatenreihe.</span><span class="sxs-lookup"><span data-stu-id="379c1-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="379c1-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="379c1-105">Methods</span></span>
<span data-ttu-id="379c1-106">Keine</span><span class="sxs-lookup"><span data-stu-id="379c1-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="379c1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="379c1-107">Properties</span></span>
<span data-ttu-id="379c1-108">Keine</span><span class="sxs-lookup"><span data-stu-id="379c1-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="379c1-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="379c1-109">Relationships</span></span>
| <span data-ttu-id="379c1-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="379c1-110">Relationship</span></span> | <span data-ttu-id="379c1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="379c1-111">Type</span></span>   |<span data-ttu-id="379c1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="379c1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="379c1-113">fill</span><span class="sxs-lookup"><span data-stu-id="379c1-113">fill</span></span>|[<span data-ttu-id="379c1-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="379c1-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="379c1-p101">Stellt die Füllung einer Diagrammdatenreihe dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="379c1-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="379c1-117">line</span><span class="sxs-lookup"><span data-stu-id="379c1-117">line</span></span>|[<span data-ttu-id="379c1-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="379c1-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="379c1-p102">Die Zeilenformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="379c1-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="379c1-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="379c1-121">JSON representation</span></span>

<span data-ttu-id="379c1-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="379c1-122">Here is a JSON representation of the resource.</span></span>

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
