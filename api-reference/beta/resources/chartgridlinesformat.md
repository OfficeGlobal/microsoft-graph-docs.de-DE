---
title: ChartGridlinesFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammgitternetzlinien.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cf2e9f1202774cc971cc09a2ce1904df2e1fb5a2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573284"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="81205-103">ChartGridlinesFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="81205-103">ChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81205-104">Kapselt die Formateigenschaften für die Diagrammgitternetzlinien.</span><span class="sxs-lookup"><span data-stu-id="81205-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="81205-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="81205-105">Methods</span></span>
<span data-ttu-id="81205-106">Keine</span><span class="sxs-lookup"><span data-stu-id="81205-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="81205-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81205-107">Properties</span></span>
<span data-ttu-id="81205-108">Keine</span><span class="sxs-lookup"><span data-stu-id="81205-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="81205-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="81205-109">Relationships</span></span>
| <span data-ttu-id="81205-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="81205-110">Relationship</span></span> | <span data-ttu-id="81205-111">Typ</span><span class="sxs-lookup"><span data-stu-id="81205-111">Type</span></span>   |<span data-ttu-id="81205-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81205-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81205-113">line</span><span class="sxs-lookup"><span data-stu-id="81205-113">line</span></span>|[<span data-ttu-id="81205-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="81205-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="81205-p101">Stellt die Formatierung der Diagrammlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="81205-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="81205-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81205-117">JSON representation</span></span>

<span data-ttu-id="81205-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81205-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlinesformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
