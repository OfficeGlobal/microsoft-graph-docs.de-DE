---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6bede2e3e8eeb44dbac67832621a2b1586c6b319
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577053"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="e8786-103">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e8786-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8786-104">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="e8786-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="e8786-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="e8786-105">Methods</span></span>

| <span data-ttu-id="e8786-106">Methode</span><span class="sxs-lookup"><span data-stu-id="e8786-106">Method</span></span>           | <span data-ttu-id="e8786-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e8786-107">Return Type</span></span>    |<span data-ttu-id="e8786-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8786-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8786-109">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="e8786-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="e8786-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e8786-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="e8786-111">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8786-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="e8786-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e8786-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="e8786-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e8786-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="e8786-114">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8786-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="e8786-115">Clear</span><span class="sxs-lookup"><span data-stu-id="e8786-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="e8786-116">Keine</span><span class="sxs-lookup"><span data-stu-id="e8786-116">None</span></span>|<span data-ttu-id="e8786-117">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="e8786-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8786-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e8786-118">Properties</span></span>
| <span data-ttu-id="e8786-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8786-119">Property</span></span>     | <span data-ttu-id="e8786-120">Typ</span><span class="sxs-lookup"><span data-stu-id="e8786-120">Type</span></span>   |<span data-ttu-id="e8786-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8786-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8786-122">color</span><span class="sxs-lookup"><span data-stu-id="e8786-122">color</span></span>|<span data-ttu-id="e8786-123">string</span><span class="sxs-lookup"><span data-stu-id="e8786-123">string</span></span>|<span data-ttu-id="e8786-124">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="e8786-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8786-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e8786-125">Relationships</span></span>
<span data-ttu-id="e8786-126">Keine</span><span class="sxs-lookup"><span data-stu-id="e8786-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e8786-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e8786-127">JSON representation</span></span>

<span data-ttu-id="e8786-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e8786-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlineformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
