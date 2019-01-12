---
title: ChartAreaFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für den gesamten Diagrammbereich.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a447b604807f3ae223445db953d45928eda9f36b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939994"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="e3c1c-103">ChartAreaFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e3c1c-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="e3c1c-104">Kapselt die Formateigenschaften für den gesamten Diagrammbereich.</span><span class="sxs-lookup"><span data-stu-id="e3c1c-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="e3c1c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="e3c1c-105">Methods</span></span>
<span data-ttu-id="e3c1c-106">Keine</span><span class="sxs-lookup"><span data-stu-id="e3c1c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e3c1c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3c1c-107">Properties</span></span>
<span data-ttu-id="e3c1c-108">Keine</span><span class="sxs-lookup"><span data-stu-id="e3c1c-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e3c1c-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3c1c-109">Relationships</span></span>
| <span data-ttu-id="e3c1c-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e3c1c-110">Relationship</span></span> | <span data-ttu-id="e3c1c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e3c1c-111">Type</span></span>   |<span data-ttu-id="e3c1c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3c1c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3c1c-113">fill</span><span class="sxs-lookup"><span data-stu-id="e3c1c-113">fill</span></span>|[<span data-ttu-id="e3c1c-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="e3c1c-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="e3c1c-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e3c1c-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="e3c1c-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="e3c1c-117">font</span></span>|[<span data-ttu-id="e3c1c-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e3c1c-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e3c1c-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e3c1c-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3c1c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3c1c-121">JSON representation</span></span>

<span data-ttu-id="e3c1c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3c1c-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
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
