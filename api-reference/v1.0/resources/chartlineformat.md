---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9da0c29acf49d0e183a2ded4652fe0972f21bf76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925917"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="b8e79-103">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8e79-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="b8e79-104">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="b8e79-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="b8e79-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b8e79-105">Methods</span></span>

| <span data-ttu-id="b8e79-106">Methode</span><span class="sxs-lookup"><span data-stu-id="b8e79-106">Method</span></span>           | <span data-ttu-id="b8e79-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b8e79-107">Return Type</span></span>    |<span data-ttu-id="b8e79-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8e79-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8e79-109">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="b8e79-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="b8e79-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b8e79-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="b8e79-111">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8e79-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="b8e79-112">Update</span><span class="sxs-lookup"><span data-stu-id="b8e79-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="b8e79-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b8e79-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="b8e79-114">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8e79-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="b8e79-115">Clear</span><span class="sxs-lookup"><span data-stu-id="b8e79-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="b8e79-116">Keine</span><span class="sxs-lookup"><span data-stu-id="b8e79-116">None</span></span>|<span data-ttu-id="b8e79-117">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="b8e79-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8e79-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8e79-118">Properties</span></span>
| <span data-ttu-id="b8e79-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8e79-119">Property</span></span>     | <span data-ttu-id="b8e79-120">Typ</span><span class="sxs-lookup"><span data-stu-id="b8e79-120">Type</span></span>   |<span data-ttu-id="b8e79-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8e79-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8e79-122">color</span><span class="sxs-lookup"><span data-stu-id="b8e79-122">color</span></span>|<span data-ttu-id="b8e79-123">string</span><span class="sxs-lookup"><span data-stu-id="b8e79-123">string</span></span>|<span data-ttu-id="b8e79-124">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="b8e79-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8e79-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8e79-125">Relationships</span></span>
<span data-ttu-id="b8e79-126">Keine</span><span class="sxs-lookup"><span data-stu-id="b8e79-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8e79-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8e79-127">JSON representation</span></span>

<span data-ttu-id="b8e79-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8e79-128">Here is a JSON representation of the resource.</span></span>

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
