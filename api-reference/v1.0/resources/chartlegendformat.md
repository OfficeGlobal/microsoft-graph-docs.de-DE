---
title: ChartLegendFormat-Ressourcentyp
description: Kapselt die Formateigenschaften einer Diagrammlegende.
ms.openlocfilehash: a29fd6e54e0976c7b4a391c450809868fe45939c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019630"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="efdd2-103">ChartLegendFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="efdd2-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="efdd2-104">Kapselt die Formateigenschaften einer Diagrammlegende.</span><span class="sxs-lookup"><span data-stu-id="efdd2-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="efdd2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="efdd2-105">Methods</span></span>
<span data-ttu-id="efdd2-106">Keine</span><span class="sxs-lookup"><span data-stu-id="efdd2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="efdd2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="efdd2-107">Properties</span></span>
<span data-ttu-id="efdd2-108">Keine</span><span class="sxs-lookup"><span data-stu-id="efdd2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="efdd2-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="efdd2-109">Relationships</span></span>
| <span data-ttu-id="efdd2-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="efdd2-110">Relationship</span></span> | <span data-ttu-id="efdd2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="efdd2-111">Type</span></span>   |<span data-ttu-id="efdd2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efdd2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efdd2-113">fill</span><span class="sxs-lookup"><span data-stu-id="efdd2-113">fill</span></span>|[<span data-ttu-id="efdd2-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="efdd2-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="efdd2-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="efdd2-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="efdd2-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="efdd2-117">font</span></span>|[<span data-ttu-id="efdd2-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="efdd2-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="efdd2-p102">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. einer Diagrammlegende dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="efdd2-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="efdd2-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="efdd2-121">JSON representation</span></span>

<span data-ttu-id="efdd2-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="efdd2-122">Here is a JSON representation of the resource.</span></span>

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