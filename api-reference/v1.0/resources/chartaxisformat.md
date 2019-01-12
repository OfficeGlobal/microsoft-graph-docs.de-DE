---
title: ChartAxisFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92258887c9646890ee63d14aebcd32ada7a8aaa6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952111"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="dbc20-103">ChartAxisFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dbc20-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="dbc20-104">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="dbc20-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="dbc20-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="dbc20-105">Methods</span></span>
<span data-ttu-id="dbc20-106">Keine</span><span class="sxs-lookup"><span data-stu-id="dbc20-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="dbc20-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dbc20-107">Properties</span></span>
<span data-ttu-id="dbc20-108">Keine</span><span class="sxs-lookup"><span data-stu-id="dbc20-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dbc20-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dbc20-109">Relationships</span></span>
| <span data-ttu-id="dbc20-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="dbc20-110">Relationship</span></span> | <span data-ttu-id="dbc20-111">Typ</span><span class="sxs-lookup"><span data-stu-id="dbc20-111">Type</span></span>   |<span data-ttu-id="dbc20-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbc20-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbc20-113">Schriftart</span><span class="sxs-lookup"><span data-stu-id="dbc20-113">font</span></span>|[<span data-ttu-id="dbc20-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="dbc20-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="dbc20-p101">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammachsenelement dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dbc20-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="dbc20-117">line</span><span class="sxs-lookup"><span data-stu-id="dbc20-117">line</span></span>|[<span data-ttu-id="dbc20-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="dbc20-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="dbc20-p102">Stellt die Formatierung der Diagrammlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dbc20-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dbc20-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dbc20-121">JSON representation</span></span>

<span data-ttu-id="dbc20-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dbc20-122">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
