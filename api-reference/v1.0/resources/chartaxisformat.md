---
title: ChartAxisFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
ms.openlocfilehash: 38679d8f6d70c336f17aa5c17c9a20e80204cfb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020130"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="af0e9-103">ChartAxisFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="af0e9-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="af0e9-104">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="af0e9-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="af0e9-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="af0e9-105">Methods</span></span>
<span data-ttu-id="af0e9-106">Keine</span><span class="sxs-lookup"><span data-stu-id="af0e9-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="af0e9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="af0e9-107">Properties</span></span>
<span data-ttu-id="af0e9-108">Keine</span><span class="sxs-lookup"><span data-stu-id="af0e9-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="af0e9-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="af0e9-109">Relationships</span></span>
| <span data-ttu-id="af0e9-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="af0e9-110">Relationship</span></span> | <span data-ttu-id="af0e9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="af0e9-111">Type</span></span>   |<span data-ttu-id="af0e9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af0e9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af0e9-113">Schriftart</span><span class="sxs-lookup"><span data-stu-id="af0e9-113">font</span></span>|[<span data-ttu-id="af0e9-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="af0e9-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="af0e9-p101">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammachsenelement dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="af0e9-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="af0e9-117">line</span><span class="sxs-lookup"><span data-stu-id="af0e9-117">line</span></span>|[<span data-ttu-id="af0e9-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="af0e9-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="af0e9-p102">Stellt die Formatierung der Diagrammlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="af0e9-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="af0e9-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="af0e9-121">JSON representation</span></span>

<span data-ttu-id="af0e9-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="af0e9-122">Here is a JSON representation of the resource.</span></span>

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