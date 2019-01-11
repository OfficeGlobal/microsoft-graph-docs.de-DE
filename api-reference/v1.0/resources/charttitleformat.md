---
title: ChartTitleFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: ee70eb991f2981a41de3e401a420a7fc0515d7c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885547"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="b2b68-103">ChartTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b2b68-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="b2b68-104">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="b2b68-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="b2b68-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b2b68-105">Methods</span></span>
<span data-ttu-id="b2b68-106">Keine</span><span class="sxs-lookup"><span data-stu-id="b2b68-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="b2b68-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2b68-107">Properties</span></span>
<span data-ttu-id="b2b68-108">Keine</span><span class="sxs-lookup"><span data-stu-id="b2b68-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b2b68-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b2b68-109">Relationships</span></span>
| <span data-ttu-id="b2b68-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b2b68-110">Relationship</span></span> | <span data-ttu-id="b2b68-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b2b68-111">Type</span></span>   |<span data-ttu-id="b2b68-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2b68-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2b68-113">fill</span><span class="sxs-lookup"><span data-stu-id="b2b68-113">fill</span></span>|[<span data-ttu-id="b2b68-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="b2b68-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="b2b68-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b2b68-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="b2b68-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="b2b68-117">font</span></span>|[<span data-ttu-id="b2b68-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b2b68-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b2b68-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b2b68-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="b2b68-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2b68-121">JSON representation</span></span>

<span data-ttu-id="b2b68-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2b68-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
