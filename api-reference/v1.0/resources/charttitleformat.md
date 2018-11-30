---
title: ChartTitleFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
ms.openlocfilehash: 7e84412adb46981a0a2b8570ed28c62d36936e36
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016875"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="71097-103">ChartTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71097-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="71097-104">Kapselt die Formateigenschaften für die Diagrammachse.</span><span class="sxs-lookup"><span data-stu-id="71097-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="71097-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="71097-105">Methods</span></span>
<span data-ttu-id="71097-106">Keine</span><span class="sxs-lookup"><span data-stu-id="71097-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="71097-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71097-107">Properties</span></span>
<span data-ttu-id="71097-108">Keine</span><span class="sxs-lookup"><span data-stu-id="71097-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="71097-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71097-109">Relationships</span></span>
| <span data-ttu-id="71097-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="71097-110">Relationship</span></span> | <span data-ttu-id="71097-111">Typ</span><span class="sxs-lookup"><span data-stu-id="71097-111">Type</span></span>   |<span data-ttu-id="71097-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71097-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71097-113">fill</span><span class="sxs-lookup"><span data-stu-id="71097-113">fill</span></span>|[<span data-ttu-id="71097-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="71097-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="71097-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71097-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="71097-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="71097-117">font</span></span>|[<span data-ttu-id="71097-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="71097-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="71097-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71097-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="71097-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71097-121">JSON representation</span></span>

<span data-ttu-id="71097-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71097-122">Here is a JSON representation of the resource.</span></span>

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
