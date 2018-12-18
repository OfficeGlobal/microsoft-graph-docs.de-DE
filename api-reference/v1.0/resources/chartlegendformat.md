---
title: ChartLegendFormat-Ressourcentyp
description: Kapselt die Formateigenschaften einer Diagrammlegende.
author: lumine2008
ms.openlocfilehash: 6ef6f2d26ade1d8d93489fbc560d4e0eb511bc86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334377"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="7437e-103">ChartLegendFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7437e-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="7437e-104">Kapselt die Formateigenschaften einer Diagrammlegende.</span><span class="sxs-lookup"><span data-stu-id="7437e-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="7437e-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="7437e-105">Methods</span></span>
<span data-ttu-id="7437e-106">Keine</span><span class="sxs-lookup"><span data-stu-id="7437e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="7437e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7437e-107">Properties</span></span>
<span data-ttu-id="7437e-108">Keine</span><span class="sxs-lookup"><span data-stu-id="7437e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7437e-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7437e-109">Relationships</span></span>
| <span data-ttu-id="7437e-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7437e-110">Relationship</span></span> | <span data-ttu-id="7437e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7437e-111">Type</span></span>   |<span data-ttu-id="7437e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7437e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7437e-113">fill</span><span class="sxs-lookup"><span data-stu-id="7437e-113">fill</span></span>|[<span data-ttu-id="7437e-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="7437e-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="7437e-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7437e-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="7437e-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="7437e-117">font</span></span>|[<span data-ttu-id="7437e-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="7437e-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="7437e-p102">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. einer Diagrammlegende dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7437e-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7437e-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7437e-121">JSON representation</span></span>

<span data-ttu-id="7437e-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7437e-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->