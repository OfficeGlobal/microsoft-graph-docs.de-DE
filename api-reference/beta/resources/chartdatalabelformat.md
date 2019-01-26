---
title: ChartDataLabelFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a82e88bd8ba083271a821dc86435b0ce55364cec
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572605"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="738c8-103">ChartDataLabelFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="738c8-103">ChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="738c8-104">Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.</span><span class="sxs-lookup"><span data-stu-id="738c8-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="738c8-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="738c8-105">Methods</span></span>
<span data-ttu-id="738c8-106">Keine</span><span class="sxs-lookup"><span data-stu-id="738c8-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="738c8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="738c8-107">Properties</span></span>
<span data-ttu-id="738c8-108">Keine</span><span class="sxs-lookup"><span data-stu-id="738c8-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="738c8-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="738c8-109">Relationships</span></span>
| <span data-ttu-id="738c8-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="738c8-110">Relationship</span></span> | <span data-ttu-id="738c8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="738c8-111">Type</span></span>   |<span data-ttu-id="738c8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="738c8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="738c8-113">fill</span><span class="sxs-lookup"><span data-stu-id="738c8-113">fill</span></span>|[<span data-ttu-id="738c8-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="738c8-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="738c8-p101">Stellt die Füllung der aktuellen Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="738c8-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="738c8-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="738c8-117">font</span></span>|[<span data-ttu-id="738c8-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="738c8-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="738c8-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für eine Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="738c8-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="738c8-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="738c8-121">JSON representation</span></span>

<span data-ttu-id="738c8-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="738c8-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabelformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
