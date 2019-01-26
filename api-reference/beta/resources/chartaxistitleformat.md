---
title: ChartAxisTitleFormat-Ressourcentyp
description: Stellt die Formatierung des Diagrammachsentitels dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: aeb39c46b349bda9f71385d13ef8e9ab17320823
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575919"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="99824-103">ChartAxisTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="99824-103">ChartAxisTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99824-104">Stellt die Formatierung des Diagrammachsentitels dar.</span><span class="sxs-lookup"><span data-stu-id="99824-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="99824-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="99824-105">Methods</span></span>
<span data-ttu-id="99824-106">Keine</span><span class="sxs-lookup"><span data-stu-id="99824-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="99824-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="99824-107">Properties</span></span>
<span data-ttu-id="99824-108">Keine</span><span class="sxs-lookup"><span data-stu-id="99824-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="99824-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="99824-109">Relationships</span></span>
| <span data-ttu-id="99824-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="99824-110">Relationship</span></span> | <span data-ttu-id="99824-111">Typ</span><span class="sxs-lookup"><span data-stu-id="99824-111">Type</span></span>   |<span data-ttu-id="99824-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99824-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99824-113">Schriftart</span><span class="sxs-lookup"><span data-stu-id="99824-113">font</span></span>|[<span data-ttu-id="99824-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="99824-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="99824-p101">Stellt die Zeichenformatierung wie Schriftart, Schriftgrad, Farbe usw. eines Diagrammachsentitel-Objekts dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="99824-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99824-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="99824-117">JSON representation</span></span>

<span data-ttu-id="99824-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="99824-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
