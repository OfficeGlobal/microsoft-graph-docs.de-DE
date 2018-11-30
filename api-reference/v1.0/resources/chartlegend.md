---
title: ChartLegend-Ressourcentyp
description: Stellt die Legende in einem Diagramm dar.
ms.openlocfilehash: 9066e69da4100c711f9b0b19165a58d94a8bb142
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017166"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="4acb2-103">ChartLegend-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4acb2-103">ChartLegend resource type</span></span>

<span data-ttu-id="4acb2-104">Stellt die Legende in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="4acb2-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="4acb2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="4acb2-105">Methods</span></span>

| <span data-ttu-id="4acb2-106">Methode</span><span class="sxs-lookup"><span data-stu-id="4acb2-106">Method</span></span>           | <span data-ttu-id="4acb2-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4acb2-107">Return Type</span></span>    |<span data-ttu-id="4acb2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4acb2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4acb2-109">ChartLegend abrufen</span><span class="sxs-lookup"><span data-stu-id="4acb2-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="4acb2-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="4acb2-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="4acb2-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4acb2-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="4acb2-112">Update</span><span class="sxs-lookup"><span data-stu-id="4acb2-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="4acb2-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="4acb2-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="4acb2-114">Dient zum Aktualisieren des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4acb2-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4acb2-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4acb2-115">Properties</span></span>
| <span data-ttu-id="4acb2-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4acb2-116">Property</span></span>     | <span data-ttu-id="4acb2-117">Typ</span><span class="sxs-lookup"><span data-stu-id="4acb2-117">Type</span></span>   |<span data-ttu-id="4acb2-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4acb2-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4acb2-119">Overlay</span><span class="sxs-lookup"><span data-stu-id="4acb2-119">overlay</span></span>|<span data-ttu-id="4acb2-120">boolean</span><span class="sxs-lookup"><span data-stu-id="4acb2-120">boolean</span></span>|<span data-ttu-id="4acb2-121">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="4acb2-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="4acb2-122">Position</span><span class="sxs-lookup"><span data-stu-id="4acb2-122">position</span></span>|<span data-ttu-id="4acb2-123">string</span><span class="sxs-lookup"><span data-stu-id="4acb2-123">string</span></span>|<span data-ttu-id="4acb2-124">Die Position der Legende im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="4acb2-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="4acb2-125">Die möglichen Werte sind: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="4acb2-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="4acb2-126">visible</span><span class="sxs-lookup"><span data-stu-id="4acb2-126">visible</span></span>|<span data-ttu-id="4acb2-127">boolean</span><span class="sxs-lookup"><span data-stu-id="4acb2-127">boolean</span></span>|<span data-ttu-id="4acb2-128">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="4acb2-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4acb2-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4acb2-129">Relationships</span></span>
| <span data-ttu-id="4acb2-130">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4acb2-130">Relationship</span></span> | <span data-ttu-id="4acb2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4acb2-131">Type</span></span>   |<span data-ttu-id="4acb2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4acb2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4acb2-133">Format</span><span class="sxs-lookup"><span data-stu-id="4acb2-133">format</span></span>|[<span data-ttu-id="4acb2-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="4acb2-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="4acb2-p102">Stellt die Formatierung für eine Diagrammlegende dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4acb2-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4acb2-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4acb2-137">JSON representation</span></span>

<span data-ttu-id="4acb2-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4acb2-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->