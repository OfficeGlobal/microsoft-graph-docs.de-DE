---
title: ChartAreaFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für den gesamten Diagrammbereich.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 637b1a886c237d6ad1f6432bf2d183c97005f981
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570855"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="fd247-103">ChartAreaFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd247-103">ChartAreaFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd247-104">Kapselt die Formateigenschaften für den gesamten Diagrammbereich.</span><span class="sxs-lookup"><span data-stu-id="fd247-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="fd247-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="fd247-105">Methods</span></span>
<span data-ttu-id="fd247-106">Keine</span><span class="sxs-lookup"><span data-stu-id="fd247-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="fd247-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd247-107">Properties</span></span>
<span data-ttu-id="fd247-108">Keine</span><span class="sxs-lookup"><span data-stu-id="fd247-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fd247-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fd247-109">Relationships</span></span>
| <span data-ttu-id="fd247-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fd247-110">Relationship</span></span> | <span data-ttu-id="fd247-111">Typ</span><span class="sxs-lookup"><span data-stu-id="fd247-111">Type</span></span>   |<span data-ttu-id="fd247-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd247-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd247-113">fill</span><span class="sxs-lookup"><span data-stu-id="fd247-113">fill</span></span>|[<span data-ttu-id="fd247-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="fd247-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="fd247-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd247-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="fd247-117">Schriftart</span><span class="sxs-lookup"><span data-stu-id="fd247-117">font</span></span>|[<span data-ttu-id="fd247-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="fd247-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="fd247-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd247-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd247-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd247-121">JSON representation</span></span>

<span data-ttu-id="fd247-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd247-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartareaformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
