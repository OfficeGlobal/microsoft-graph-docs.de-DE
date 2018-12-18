---
title: ChartLegend-Ressourcentyp
description: Stellt die Legende in einem Diagramm dar.
author: lumine2008
ms.openlocfilehash: 67a55f0286bcf57157cd9912bb03ba0bd6506517
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326404"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="b4885-103">ChartLegend-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4885-103">ChartLegend resource type</span></span>

> <span data-ttu-id="b4885-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4885-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4885-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4885-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4885-106">Stellt die Legende in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="b4885-106">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b4885-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="b4885-107">Methods</span></span>

| <span data-ttu-id="b4885-108">Methode</span><span class="sxs-lookup"><span data-stu-id="b4885-108">Method</span></span>           | <span data-ttu-id="b4885-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b4885-109">Return Type</span></span>    |<span data-ttu-id="b4885-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4885-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b4885-111">ChartLegend abrufen</span><span class="sxs-lookup"><span data-stu-id="b4885-111">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="b4885-112">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b4885-112">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b4885-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4885-113">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="b4885-114">Update</span><span class="sxs-lookup"><span data-stu-id="b4885-114">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="b4885-115">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b4885-115">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b4885-116">Dient zum Aktualisieren des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4885-116">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b4885-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4885-117">Properties</span></span>
| <span data-ttu-id="b4885-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4885-118">Property</span></span>     | <span data-ttu-id="b4885-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b4885-119">Type</span></span>   |<span data-ttu-id="b4885-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4885-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4885-121">Overlay</span><span class="sxs-lookup"><span data-stu-id="b4885-121">overlay</span></span>|<span data-ttu-id="b4885-122">boolean</span><span class="sxs-lookup"><span data-stu-id="b4885-122">boolean</span></span>|<span data-ttu-id="b4885-123">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="b4885-123">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="b4885-124">Position</span><span class="sxs-lookup"><span data-stu-id="b4885-124">position</span></span>|<span data-ttu-id="b4885-125">string</span><span class="sxs-lookup"><span data-stu-id="b4885-125">string</span></span>|<span data-ttu-id="b4885-p102">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="b4885-p102">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="b4885-128">visible</span><span class="sxs-lookup"><span data-stu-id="b4885-128">visible</span></span>|<span data-ttu-id="b4885-129">boolean</span><span class="sxs-lookup"><span data-stu-id="b4885-129">boolean</span></span>|<span data-ttu-id="b4885-130">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="b4885-130">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4885-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b4885-131">Relationships</span></span>
| <span data-ttu-id="b4885-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b4885-132">Relationship</span></span> | <span data-ttu-id="b4885-133">Typ</span><span class="sxs-lookup"><span data-stu-id="b4885-133">Type</span></span>   |<span data-ttu-id="b4885-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4885-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4885-135">Format</span><span class="sxs-lookup"><span data-stu-id="b4885-135">format</span></span>|[<span data-ttu-id="b4885-136">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="b4885-136">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="b4885-p103">Stellt die Formatierung für eine Diagrammlegende dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4885-p103">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4885-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4885-139">JSON representation</span></span>

<span data-ttu-id="b4885-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4885-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
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