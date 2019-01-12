---
title: ChartAxisTitleFormat-Ressourcentyp
description: Stellt die Formatierung des Diagrammachsentitels dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959482"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="c03fa-103">ChartAxisTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c03fa-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="c03fa-104">Stellt die Formatierung des Diagrammachsentitels dar.</span><span class="sxs-lookup"><span data-stu-id="c03fa-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="c03fa-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="c03fa-105">Methods</span></span>
<span data-ttu-id="c03fa-106">Keine</span><span class="sxs-lookup"><span data-stu-id="c03fa-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c03fa-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c03fa-107">Properties</span></span>
<span data-ttu-id="c03fa-108">Keine</span><span class="sxs-lookup"><span data-stu-id="c03fa-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c03fa-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c03fa-109">Relationships</span></span>
| <span data-ttu-id="c03fa-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c03fa-110">Relationship</span></span> | <span data-ttu-id="c03fa-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c03fa-111">Type</span></span>   |<span data-ttu-id="c03fa-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c03fa-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c03fa-113">Schriftart</span><span class="sxs-lookup"><span data-stu-id="c03fa-113">font</span></span>|[<span data-ttu-id="c03fa-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c03fa-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="c03fa-p101">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. eines Diagrammachsentitel-Objekts dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c03fa-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c03fa-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c03fa-117">JSON representation</span></span>

<span data-ttu-id="c03fa-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c03fa-118">Here is a JSON representation of the resource.</span></span>

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
