---
title: ChartLegend-Ressourcentyp
description: Stellt die Legende in einem Diagramm dar.
ms.openlocfilehash: d01eee45245d17fb142ddb75b70a6cde6a89213c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064880"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="710e9-103">ChartLegend-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="710e9-103">ChartLegend resource type</span></span>

> <span data-ttu-id="710e9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="710e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="710e9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="710e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="710e9-106">Stellt die Legende in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="710e9-106">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="710e9-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="710e9-107">Methods</span></span>

| <span data-ttu-id="710e9-108">Methode</span><span class="sxs-lookup"><span data-stu-id="710e9-108">Method</span></span>           | <span data-ttu-id="710e9-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="710e9-109">Return Type</span></span>    |<span data-ttu-id="710e9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="710e9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="710e9-111">ChartLegend abrufen</span><span class="sxs-lookup"><span data-stu-id="710e9-111">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="710e9-112">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="710e9-112">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="710e9-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="710e9-113">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="710e9-114">Update</span><span class="sxs-lookup"><span data-stu-id="710e9-114">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="710e9-115">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="710e9-115">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="710e9-116">Dient zum Aktualisieren des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="710e9-116">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="710e9-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="710e9-117">Properties</span></span>
| <span data-ttu-id="710e9-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="710e9-118">Property</span></span>     | <span data-ttu-id="710e9-119">Typ</span><span class="sxs-lookup"><span data-stu-id="710e9-119">Type</span></span>   |<span data-ttu-id="710e9-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="710e9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="710e9-121">Overlay</span><span class="sxs-lookup"><span data-stu-id="710e9-121">overlay</span></span>|<span data-ttu-id="710e9-122">boolean</span><span class="sxs-lookup"><span data-stu-id="710e9-122">boolean</span></span>|<span data-ttu-id="710e9-123">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="710e9-123">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="710e9-124">Position</span><span class="sxs-lookup"><span data-stu-id="710e9-124">position</span></span>|<span data-ttu-id="710e9-125">string</span><span class="sxs-lookup"><span data-stu-id="710e9-125">string</span></span>|<span data-ttu-id="710e9-p102">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="710e9-p102">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="710e9-128">visible</span><span class="sxs-lookup"><span data-stu-id="710e9-128">visible</span></span>|<span data-ttu-id="710e9-129">boolean</span><span class="sxs-lookup"><span data-stu-id="710e9-129">boolean</span></span>|<span data-ttu-id="710e9-130">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="710e9-130">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="710e9-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="710e9-131">Relationships</span></span>
| <span data-ttu-id="710e9-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="710e9-132">Relationship</span></span> | <span data-ttu-id="710e9-133">Typ</span><span class="sxs-lookup"><span data-stu-id="710e9-133">Type</span></span>   |<span data-ttu-id="710e9-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="710e9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="710e9-135">Format</span><span class="sxs-lookup"><span data-stu-id="710e9-135">format</span></span>|[<span data-ttu-id="710e9-136">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="710e9-136">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="710e9-p103">Stellt die Formatierung für eine Diagrammlegende dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="710e9-p103">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="710e9-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="710e9-139">JSON representation</span></span>

<span data-ttu-id="710e9-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="710e9-140">Here is a JSON representation of the resource.</span></span>

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