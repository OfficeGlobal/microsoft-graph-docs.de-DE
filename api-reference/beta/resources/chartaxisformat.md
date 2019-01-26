---
title: ChartAxisFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 587c35f0bf28d695f67e61a8eefa1593317a8d5d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577109"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="e2fae-103">ChartAxisFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2fae-103">ChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2fae-104">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="e2fae-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="e2fae-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="e2fae-105">Methods</span></span>
<span data-ttu-id="e2fae-106">Keine</span><span class="sxs-lookup"><span data-stu-id="e2fae-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="e2fae-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2fae-107">Properties</span></span>
<span data-ttu-id="e2fae-108">Keine</span><span class="sxs-lookup"><span data-stu-id="e2fae-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e2fae-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2fae-109">Relationships</span></span>
| <span data-ttu-id="e2fae-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e2fae-110">Relationship</span></span> | <span data-ttu-id="e2fae-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e2fae-111">Type</span></span>   |<span data-ttu-id="e2fae-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2fae-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2fae-113">Schriftart</span><span class="sxs-lookup"><span data-stu-id="e2fae-113">font</span></span>|[<span data-ttu-id="e2fae-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e2fae-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e2fae-p101">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammachsenelement dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e2fae-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="e2fae-117">line</span><span class="sxs-lookup"><span data-stu-id="e2fae-117">line</span></span>|[<span data-ttu-id="e2fae-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e2fae-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="e2fae-p102">Stellt die Formatierung der Diagrammlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e2fae-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e2fae-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2fae-121">JSON representation</span></span>

<span data-ttu-id="e2fae-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2fae-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxisformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
