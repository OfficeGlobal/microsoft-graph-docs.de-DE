---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b4409eb18dab41d43adc038b702a65fa8d63e4de
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640581"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="ac2e5-103">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ac2e5-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac2e5-104">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="ac2e5-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="ac2e5-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="ac2e5-105">Methods</span></span>

| <span data-ttu-id="ac2e5-106">Methode</span><span class="sxs-lookup"><span data-stu-id="ac2e5-106">Method</span></span>           | <span data-ttu-id="ac2e5-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ac2e5-107">Return Type</span></span>    |<span data-ttu-id="ac2e5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac2e5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac2e5-109">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="ac2e5-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="ac2e5-110">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ac2e5-110">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="ac2e5-111">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac2e5-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="ac2e5-112">Update</span><span class="sxs-lookup"><span data-stu-id="ac2e5-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="ac2e5-113">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ac2e5-113">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="ac2e5-114">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac2e5-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="ac2e5-115">Clear</span><span class="sxs-lookup"><span data-stu-id="ac2e5-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="ac2e5-116">Keine</span><span class="sxs-lookup"><span data-stu-id="ac2e5-116">None</span></span>|<span data-ttu-id="ac2e5-117">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="ac2e5-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac2e5-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ac2e5-118">Properties</span></span>
| <span data-ttu-id="ac2e5-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac2e5-119">Property</span></span>     | <span data-ttu-id="ac2e5-120">Typ</span><span class="sxs-lookup"><span data-stu-id="ac2e5-120">Type</span></span>   |<span data-ttu-id="ac2e5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac2e5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac2e5-122">color</span><span class="sxs-lookup"><span data-stu-id="ac2e5-122">color</span></span>|<span data-ttu-id="ac2e5-123">string</span><span class="sxs-lookup"><span data-stu-id="ac2e5-123">string</span></span>|<span data-ttu-id="ac2e5-124">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="ac2e5-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac2e5-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ac2e5-125">Relationships</span></span>
<span data-ttu-id="ac2e5-126">Keine</span><span class="sxs-lookup"><span data-stu-id="ac2e5-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ac2e5-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ac2e5-127">JSON representation</span></span>

<span data-ttu-id="ac2e5-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ac2e5-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
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
