---
title: ChartAreaFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für den gesamten Diagrammbereich.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 79867ff3519467279abcb4b9684b713964eb8f98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838171"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="9712c-103">ChartAreaFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9712c-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="9712c-104">Kapselt die Formateigenschaften für den gesamten Diagrammbereich.</span><span class="sxs-lookup"><span data-stu-id="9712c-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="9712c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="9712c-105">Methods</span></span>
<span data-ttu-id="9712c-106">Keine</span><span class="sxs-lookup"><span data-stu-id="9712c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="9712c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9712c-107">Properties</span></span>
<span data-ttu-id="9712c-108">Keine</span><span class="sxs-lookup"><span data-stu-id="9712c-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9712c-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9712c-109">Relationships</span></span>
| <span data-ttu-id="9712c-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9712c-110">Relationship</span></span> | <span data-ttu-id="9712c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9712c-111">Type</span></span>   |<span data-ttu-id="9712c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9712c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9712c-113">fill</span><span class="sxs-lookup"><span data-stu-id="9712c-113">fill</span></span>|[<span data-ttu-id="9712c-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="9712c-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="9712c-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9712c-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="9712c-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="9712c-117">font</span></span>|[<span data-ttu-id="9712c-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="9712c-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="9712c-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9712c-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9712c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9712c-121">JSON representation</span></span>

<span data-ttu-id="9712c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9712c-122">Here is a JSON representation of the resource.</span></span>

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
