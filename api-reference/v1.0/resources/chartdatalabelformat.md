---
title: ChartDataLabelFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.
ms.openlocfilehash: ec81523dc09c17cd8c7fb9d543c2214377201260
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017014"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="8a8bf-103">ChartDataLabelFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8a8bf-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="8a8bf-104">Kapselt die Formateigenschaften für die Diagrammdatenbeschriftungen.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="8a8bf-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="8a8bf-105">Methods</span></span>
<span data-ttu-id="8a8bf-106">Keine</span><span class="sxs-lookup"><span data-stu-id="8a8bf-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="8a8bf-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8a8bf-107">Properties</span></span>
<span data-ttu-id="8a8bf-108">Keine</span><span class="sxs-lookup"><span data-stu-id="8a8bf-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8a8bf-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8a8bf-109">Relationships</span></span>
| <span data-ttu-id="8a8bf-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8a8bf-110">Relationship</span></span> | <span data-ttu-id="8a8bf-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8a8bf-111">Type</span></span>   |<span data-ttu-id="8a8bf-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a8bf-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a8bf-113">fill</span><span class="sxs-lookup"><span data-stu-id="8a8bf-113">fill</span></span>|[<span data-ttu-id="8a8bf-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="8a8bf-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="8a8bf-p101">Stellt die Füllung der aktuellen Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="8a8bf-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="8a8bf-117">font</span></span>|[<span data-ttu-id="8a8bf-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="8a8bf-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="8a8bf-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für eine Diagrammdatenbeschriftung dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8a8bf-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8a8bf-121">JSON representation</span></span>

<span data-ttu-id="8a8bf-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8a8bf-122">Here is a JSON representation of the resource.</span></span>

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