---
title: ChartSeriesFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für den Diagrammdatenreihe.
ms.openlocfilehash: 81b79331580c2d7edbc52f19d1c4c9cfd57db0cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017406"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="bb31e-103">ChartSeriesFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb31e-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="bb31e-104">Kapselt die Formateigenschaften für den Diagrammdatenreihe.</span><span class="sxs-lookup"><span data-stu-id="bb31e-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="bb31e-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="bb31e-105">Methods</span></span>
<span data-ttu-id="bb31e-106">Keine</span><span class="sxs-lookup"><span data-stu-id="bb31e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="bb31e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb31e-107">Properties</span></span>
<span data-ttu-id="bb31e-108">Keine</span><span class="sxs-lookup"><span data-stu-id="bb31e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bb31e-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb31e-109">Relationships</span></span>
| <span data-ttu-id="bb31e-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bb31e-110">Relationship</span></span> | <span data-ttu-id="bb31e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="bb31e-111">Type</span></span>   |<span data-ttu-id="bb31e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb31e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb31e-113">fill</span><span class="sxs-lookup"><span data-stu-id="bb31e-113">fill</span></span>|[<span data-ttu-id="bb31e-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="bb31e-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="bb31e-p101">Stellt die Füllung einer Diagrammdatenreihe dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb31e-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="bb31e-117">line</span><span class="sxs-lookup"><span data-stu-id="bb31e-117">line</span></span>|[<span data-ttu-id="bb31e-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bb31e-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="bb31e-p102">Die Zeilenformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb31e-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bb31e-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb31e-121">JSON representation</span></span>

<span data-ttu-id="bb31e-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb31e-122">Here is a JSON representation of the resource.</span></span>

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