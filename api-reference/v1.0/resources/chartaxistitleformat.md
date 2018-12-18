---
title: ChartAxisTitleFormat-Ressourcentyp
description: Stellt die Formatierung des Diagrammachsentitels dar.
author: lumine2008
ms.openlocfilehash: 7a160f02f06c74edeee09f91b2b117ea437291e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343022"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="58032-103">ChartAxisTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="58032-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="58032-104">Stellt die Formatierung des Diagrammachsentitels dar.</span><span class="sxs-lookup"><span data-stu-id="58032-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="58032-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="58032-105">Methods</span></span>
<span data-ttu-id="58032-106">Keine</span><span class="sxs-lookup"><span data-stu-id="58032-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="58032-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="58032-107">Properties</span></span>
<span data-ttu-id="58032-108">Keine</span><span class="sxs-lookup"><span data-stu-id="58032-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="58032-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="58032-109">Relationships</span></span>
| <span data-ttu-id="58032-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="58032-110">Relationship</span></span> | <span data-ttu-id="58032-111">Typ</span><span class="sxs-lookup"><span data-stu-id="58032-111">Type</span></span>   |<span data-ttu-id="58032-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58032-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58032-113">Schriftart</span><span class="sxs-lookup"><span data-stu-id="58032-113">font</span></span>|[<span data-ttu-id="58032-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="58032-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="58032-p101">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. eines Diagrammachsentitel-Objekts dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="58032-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58032-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="58032-117">JSON representation</span></span>

<span data-ttu-id="58032-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="58032-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->