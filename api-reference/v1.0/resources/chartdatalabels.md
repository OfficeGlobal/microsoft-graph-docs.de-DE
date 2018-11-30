---
title: ChartDataLabels-Ressourcentyp
description: Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.
ms.openlocfilehash: f8cb4310ab9ca2e59325fbc4bd255ae161cc7892
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016350"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="ee39e-103">ChartDataLabels-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ee39e-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="ee39e-104">Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.</span><span class="sxs-lookup"><span data-stu-id="ee39e-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="ee39e-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="ee39e-105">Methods</span></span>

| <span data-ttu-id="ee39e-106">Methode</span><span class="sxs-lookup"><span data-stu-id="ee39e-106">Method</span></span>           | <span data-ttu-id="ee39e-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ee39e-107">Return Type</span></span>    |<span data-ttu-id="ee39e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee39e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ee39e-109">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="ee39e-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="ee39e-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="ee39e-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="ee39e-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee39e-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="ee39e-112">Update</span><span class="sxs-lookup"><span data-stu-id="ee39e-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="ee39e-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="ee39e-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="ee39e-114">Dient zum Aktualisieren des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee39e-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ee39e-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ee39e-115">Properties</span></span>
| <span data-ttu-id="ee39e-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee39e-116">Property</span></span>     | <span data-ttu-id="ee39e-117">Typ</span><span class="sxs-lookup"><span data-stu-id="ee39e-117">Type</span></span>   |<span data-ttu-id="ee39e-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee39e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee39e-119">position</span><span class="sxs-lookup"><span data-stu-id="ee39e-119">position</span></span>|<span data-ttu-id="ee39e-120">string</span><span class="sxs-lookup"><span data-stu-id="ee39e-120">string</span></span>|<span data-ttu-id="ee39e-121">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt.</span><span class="sxs-lookup"><span data-stu-id="ee39e-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="ee39e-122">Die möglichen Werte sind: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="ee39e-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="ee39e-123">Separator</span><span class="sxs-lookup"><span data-stu-id="ee39e-123">separator</span></span>|<span data-ttu-id="ee39e-124">string</span><span class="sxs-lookup"><span data-stu-id="ee39e-124">string</span></span>|<span data-ttu-id="ee39e-125">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="ee39e-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="ee39e-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="ee39e-126">showBubbleSize</span></span>|<span data-ttu-id="ee39e-127">boolean</span><span class="sxs-lookup"><span data-stu-id="ee39e-127">boolean</span></span>|<span data-ttu-id="ee39e-128">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ee39e-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="ee39e-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="ee39e-129">showCategoryName</span></span>|<span data-ttu-id="ee39e-130">boolean</span><span class="sxs-lookup"><span data-stu-id="ee39e-130">boolean</span></span>|<span data-ttu-id="ee39e-131">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ee39e-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="ee39e-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="ee39e-132">showLegendKey</span></span>|<span data-ttu-id="ee39e-133">boolean</span><span class="sxs-lookup"><span data-stu-id="ee39e-133">boolean</span></span>|<span data-ttu-id="ee39e-134">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ee39e-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="ee39e-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="ee39e-135">showPercentage</span></span>|<span data-ttu-id="ee39e-136">boolean</span><span class="sxs-lookup"><span data-stu-id="ee39e-136">boolean</span></span>|<span data-ttu-id="ee39e-137">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ee39e-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="ee39e-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="ee39e-138">showSeriesName</span></span>|<span data-ttu-id="ee39e-139">boolean</span><span class="sxs-lookup"><span data-stu-id="ee39e-139">boolean</span></span>|<span data-ttu-id="ee39e-140">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ee39e-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="ee39e-141">showValue</span><span class="sxs-lookup"><span data-stu-id="ee39e-141">showValue</span></span>|<span data-ttu-id="ee39e-142">boolean</span><span class="sxs-lookup"><span data-stu-id="ee39e-142">boolean</span></span>|<span data-ttu-id="ee39e-143">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ee39e-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee39e-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ee39e-144">Relationships</span></span>
| <span data-ttu-id="ee39e-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ee39e-145">Relationship</span></span> | <span data-ttu-id="ee39e-146">Typ</span><span class="sxs-lookup"><span data-stu-id="ee39e-146">Type</span></span>   |<span data-ttu-id="ee39e-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee39e-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee39e-148">Format</span><span class="sxs-lookup"><span data-stu-id="ee39e-148">format</span></span>|[<span data-ttu-id="ee39e-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="ee39e-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="ee39e-p102">Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ee39e-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee39e-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ee39e-152">JSON representation</span></span>

<span data-ttu-id="ee39e-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ee39e-153">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->