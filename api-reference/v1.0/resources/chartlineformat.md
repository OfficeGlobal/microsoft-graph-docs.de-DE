---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 70e4e3d5c88fccd2a34c3fa17d5fe4bf5dcf1e5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805740"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="9c24d-103">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9c24d-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="9c24d-104">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="9c24d-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="9c24d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="9c24d-105">Methods</span></span>

| <span data-ttu-id="9c24d-106">Methode</span><span class="sxs-lookup"><span data-stu-id="9c24d-106">Method</span></span>           | <span data-ttu-id="9c24d-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9c24d-107">Return Type</span></span>    |<span data-ttu-id="9c24d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c24d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c24d-109">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="9c24d-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="9c24d-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="9c24d-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="9c24d-111">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c24d-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="9c24d-112">Update</span><span class="sxs-lookup"><span data-stu-id="9c24d-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="9c24d-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="9c24d-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="9c24d-114">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c24d-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="9c24d-115">Clear</span><span class="sxs-lookup"><span data-stu-id="9c24d-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="9c24d-116">Keine</span><span class="sxs-lookup"><span data-stu-id="9c24d-116">None</span></span>|<span data-ttu-id="9c24d-117">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="9c24d-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c24d-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c24d-118">Properties</span></span>
| <span data-ttu-id="9c24d-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c24d-119">Property</span></span>     | <span data-ttu-id="9c24d-120">Typ</span><span class="sxs-lookup"><span data-stu-id="9c24d-120">Type</span></span>   |<span data-ttu-id="9c24d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c24d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c24d-122">color</span><span class="sxs-lookup"><span data-stu-id="9c24d-122">color</span></span>|<span data-ttu-id="9c24d-123">string</span><span class="sxs-lookup"><span data-stu-id="9c24d-123">string</span></span>|<span data-ttu-id="9c24d-124">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="9c24d-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c24d-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9c24d-125">Relationships</span></span>
<span data-ttu-id="9c24d-126">Keine</span><span class="sxs-lookup"><span data-stu-id="9c24d-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c24d-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9c24d-127">JSON representation</span></span>

<span data-ttu-id="9c24d-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9c24d-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
