---
title: ChartDataLabelFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.
author: lumine2008
ms.openlocfilehash: 4c8961eb884a5ab603feda368934795cb73915d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356476"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="9bac2-103">ChartDataLabelFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9bac2-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="9bac2-104">Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.</span><span class="sxs-lookup"><span data-stu-id="9bac2-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="9bac2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="9bac2-105">Methods</span></span>
<span data-ttu-id="9bac2-106">Keine</span><span class="sxs-lookup"><span data-stu-id="9bac2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="9bac2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9bac2-107">Properties</span></span>
<span data-ttu-id="9bac2-108">Keine</span><span class="sxs-lookup"><span data-stu-id="9bac2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9bac2-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9bac2-109">Relationships</span></span>
| <span data-ttu-id="9bac2-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9bac2-110">Relationship</span></span> | <span data-ttu-id="9bac2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9bac2-111">Type</span></span>   |<span data-ttu-id="9bac2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bac2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bac2-113">fill</span><span class="sxs-lookup"><span data-stu-id="9bac2-113">fill</span></span>|[<span data-ttu-id="9bac2-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="9bac2-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="9bac2-p101">Stellt die Füllung der aktuellen Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9bac2-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="9bac2-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="9bac2-117">font</span></span>|[<span data-ttu-id="9bac2-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="9bac2-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="9bac2-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für eine Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9bac2-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9bac2-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9bac2-121">JSON representation</span></span>

<span data-ttu-id="9bac2-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9bac2-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->