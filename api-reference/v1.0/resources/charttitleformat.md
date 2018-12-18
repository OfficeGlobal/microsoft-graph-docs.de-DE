---
title: ChartTitleFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
ms.openlocfilehash: 16169af251a0764c99ae04c5516ad9d552d1654c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362139"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="d5d80-103">ChartTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d5d80-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="d5d80-104">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="d5d80-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="d5d80-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d5d80-105">Methods</span></span>
<span data-ttu-id="d5d80-106">Keine</span><span class="sxs-lookup"><span data-stu-id="d5d80-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d5d80-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5d80-107">Properties</span></span>
<span data-ttu-id="d5d80-108">Keine</span><span class="sxs-lookup"><span data-stu-id="d5d80-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d5d80-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d5d80-109">Relationships</span></span>
| <span data-ttu-id="d5d80-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d5d80-110">Relationship</span></span> | <span data-ttu-id="d5d80-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d5d80-111">Type</span></span>   |<span data-ttu-id="d5d80-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5d80-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5d80-113">fill</span><span class="sxs-lookup"><span data-stu-id="d5d80-113">fill</span></span>|[<span data-ttu-id="d5d80-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d5d80-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="d5d80-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d5d80-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="d5d80-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="d5d80-117">font</span></span>|[<span data-ttu-id="d5d80-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d5d80-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="d5d80-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d5d80-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="d5d80-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5d80-121">JSON representation</span></span>

<span data-ttu-id="d5d80-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5d80-122">Here is a JSON representation of the resource.</span></span>

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
