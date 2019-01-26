---
title: ChartPointFormat-Ressourcentyp
description: Stellt das Formatierungsobjekt für Diagrammpunkte dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3004577a5ca9687b4bef85f59cfcc8eb528c4a66
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573305"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="e5513-103">ChartPointFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e5513-103">ChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5513-104">Stellt das Formatierungsobjekt für Diagrammpunkte dar.</span><span class="sxs-lookup"><span data-stu-id="e5513-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="e5513-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="e5513-105">Methods</span></span>
<span data-ttu-id="e5513-106">Keine</span><span class="sxs-lookup"><span data-stu-id="e5513-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e5513-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e5513-107">Properties</span></span>
<span data-ttu-id="e5513-108">Keine</span><span class="sxs-lookup"><span data-stu-id="e5513-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e5513-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e5513-109">Relationships</span></span>
| <span data-ttu-id="e5513-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e5513-110">Relationship</span></span> | <span data-ttu-id="e5513-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e5513-111">Type</span></span>   |<span data-ttu-id="e5513-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5513-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5513-113">fill</span><span class="sxs-lookup"><span data-stu-id="e5513-113">fill</span></span>|[<span data-ttu-id="e5513-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="e5513-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="e5513-p101">Stellt die Füllung eines Diagramms dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e5513-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e5513-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e5513-117">JSON representation</span></span>

<span data-ttu-id="e5513-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5513-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpointformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
