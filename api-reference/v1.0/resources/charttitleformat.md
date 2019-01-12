---
title: ChartTitleFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3a2c16d37d2ca86d7cafbb4047ee0bcea1ee4bde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977115"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="80e4d-103">ChartTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="80e4d-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="80e4d-104">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="80e4d-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="80e4d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="80e4d-105">Methods</span></span>
<span data-ttu-id="80e4d-106">Keine</span><span class="sxs-lookup"><span data-stu-id="80e4d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="80e4d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80e4d-107">Properties</span></span>
<span data-ttu-id="80e4d-108">Keine</span><span class="sxs-lookup"><span data-stu-id="80e4d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="80e4d-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="80e4d-109">Relationships</span></span>
| <span data-ttu-id="80e4d-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="80e4d-110">Relationship</span></span> | <span data-ttu-id="80e4d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="80e4d-111">Type</span></span>   |<span data-ttu-id="80e4d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80e4d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80e4d-113">fill</span><span class="sxs-lookup"><span data-stu-id="80e4d-113">fill</span></span>|[<span data-ttu-id="80e4d-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="80e4d-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="80e4d-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80e4d-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="80e4d-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="80e4d-117">font</span></span>|[<span data-ttu-id="80e4d-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="80e4d-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="80e4d-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80e4d-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="80e4d-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80e4d-121">JSON representation</span></span>

<span data-ttu-id="80e4d-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80e4d-122">Here is a JSON representation of the resource.</span></span>

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
