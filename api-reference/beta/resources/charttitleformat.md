---
title: ChartTitleFormat-Ressourcentyp
description: Kapselt die Formateigenschaften für die Diagrammachse.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7dd9400873234fd73ebe506a49caf6583d05b75b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574012"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="e9ed9-103">ChartTitleFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e9ed9-103">ChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="methods"></a><span data-ttu-id="e9ed9-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="e9ed9-104">Methods</span></span>
<span data-ttu-id="e9ed9-105">Keine</span><span class="sxs-lookup"><span data-stu-id="e9ed9-105">None</span></span>

## <a name="properties"></a><span data-ttu-id="e9ed9-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9ed9-106">Properties</span></span>
<span data-ttu-id="e9ed9-107">Keine</span><span class="sxs-lookup"><span data-stu-id="e9ed9-107">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e9ed9-108">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e9ed9-108">Relationships</span></span>
| <span data-ttu-id="e9ed9-109">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e9ed9-109">Relationship</span></span> | <span data-ttu-id="e9ed9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e9ed9-110">Type</span></span>   |<span data-ttu-id="e9ed9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9ed9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9ed9-112">fill</span><span class="sxs-lookup"><span data-stu-id="e9ed9-112">fill</span></span>|[<span data-ttu-id="e9ed9-113">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="e9ed9-113">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="e9ed9-p101">Stellt die Füllung eines Objekts dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e9ed9-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="e9ed9-116">Schriftart</span><span class="sxs-lookup"><span data-stu-id="e9ed9-116">font</span></span>|[<span data-ttu-id="e9ed9-117">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e9ed9-117">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e9ed9-p102">Stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für das aktuelle Objekt dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e9ed9-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="e9ed9-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9ed9-120">JSON representation</span></span>

<span data-ttu-id="e9ed9-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9ed9-121">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
