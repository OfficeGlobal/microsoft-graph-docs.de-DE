---
title: ChartDataLabelFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 586b201b0bcc70765fb68aa7736664f493f5539b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876923"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="1af8b-103">ChartDataLabelFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1af8b-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="1af8b-104">Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.</span><span class="sxs-lookup"><span data-stu-id="1af8b-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="1af8b-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="1af8b-105">Methods</span></span>
<span data-ttu-id="1af8b-106">Keine</span><span class="sxs-lookup"><span data-stu-id="1af8b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="1af8b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1af8b-107">Properties</span></span>
<span data-ttu-id="1af8b-108">Keine</span><span class="sxs-lookup"><span data-stu-id="1af8b-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1af8b-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1af8b-109">Relationships</span></span>
| <span data-ttu-id="1af8b-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1af8b-110">Relationship</span></span> | <span data-ttu-id="1af8b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1af8b-111">Type</span></span>   |<span data-ttu-id="1af8b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1af8b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1af8b-113">fill</span><span class="sxs-lookup"><span data-stu-id="1af8b-113">fill</span></span>|[<span data-ttu-id="1af8b-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="1af8b-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="1af8b-p101">Stellt die Füllung der aktuellen Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1af8b-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="1af8b-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="1af8b-117">font</span></span>|[<span data-ttu-id="1af8b-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="1af8b-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="1af8b-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für eine Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1af8b-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1af8b-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1af8b-121">JSON representation</span></span>

<span data-ttu-id="1af8b-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1af8b-122">Here is a JSON representation of the resource.</span></span>

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
