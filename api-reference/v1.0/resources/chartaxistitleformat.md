---
title: ChartAxisTitleFormat-Ressourcentyp
description: Stellt die Formatierung des Diagrammachsentitels dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4aa96f0a346d8b08832464097b258a92b1db44df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840313"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="b4ec7-103">ChartAxisTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4ec7-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="b4ec7-104">Stellt die Formatierung des Diagrammachsentitels dar.</span><span class="sxs-lookup"><span data-stu-id="b4ec7-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="b4ec7-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b4ec7-105">Methods</span></span>
<span data-ttu-id="b4ec7-106">Keine</span><span class="sxs-lookup"><span data-stu-id="b4ec7-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="b4ec7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4ec7-107">Properties</span></span>
<span data-ttu-id="b4ec7-108">Keine</span><span class="sxs-lookup"><span data-stu-id="b4ec7-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b4ec7-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b4ec7-109">Relationships</span></span>
| <span data-ttu-id="b4ec7-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b4ec7-110">Relationship</span></span> | <span data-ttu-id="b4ec7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b4ec7-111">Type</span></span>   |<span data-ttu-id="b4ec7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4ec7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4ec7-113">Schriftart</span><span class="sxs-lookup"><span data-stu-id="b4ec7-113">font</span></span>|[<span data-ttu-id="b4ec7-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b4ec7-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b4ec7-p101">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. eines Diagrammachsentitel-Objekts dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4ec7-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4ec7-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4ec7-117">JSON representation</span></span>

<span data-ttu-id="b4ec7-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4ec7-118">Here is a JSON representation of the resource.</span></span>

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
