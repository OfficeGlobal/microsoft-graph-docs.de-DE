---
title: ChartDataLabels-Ressourcentyp
description: Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: add7ef03b4779cae799949c6eb5901fcd1e3ddaf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809009"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="75343-103">ChartDataLabels-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="75343-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="75343-104">Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.</span><span class="sxs-lookup"><span data-stu-id="75343-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="75343-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="75343-105">Methods</span></span>

| <span data-ttu-id="75343-106">Methode</span><span class="sxs-lookup"><span data-stu-id="75343-106">Method</span></span>           | <span data-ttu-id="75343-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="75343-107">Return Type</span></span>    |<span data-ttu-id="75343-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75343-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75343-109">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="75343-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="75343-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="75343-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="75343-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="75343-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="75343-112">Update</span><span class="sxs-lookup"><span data-stu-id="75343-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="75343-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="75343-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="75343-114">Dient zum Aktualisieren des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="75343-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="75343-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="75343-115">Properties</span></span>
| <span data-ttu-id="75343-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75343-116">Property</span></span>     | <span data-ttu-id="75343-117">Typ</span><span class="sxs-lookup"><span data-stu-id="75343-117">Type</span></span>   |<span data-ttu-id="75343-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75343-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75343-119">position</span><span class="sxs-lookup"><span data-stu-id="75343-119">position</span></span>|<span data-ttu-id="75343-120">string</span><span class="sxs-lookup"><span data-stu-id="75343-120">string</span></span>|<span data-ttu-id="75343-121">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt.</span><span class="sxs-lookup"><span data-stu-id="75343-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="75343-122">Die möglichen Werte sind: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="75343-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="75343-123">Separator</span><span class="sxs-lookup"><span data-stu-id="75343-123">separator</span></span>|<span data-ttu-id="75343-124">string</span><span class="sxs-lookup"><span data-stu-id="75343-124">string</span></span>|<span data-ttu-id="75343-125">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="75343-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="75343-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="75343-126">showBubbleSize</span></span>|<span data-ttu-id="75343-127">boolean</span><span class="sxs-lookup"><span data-stu-id="75343-127">boolean</span></span>|<span data-ttu-id="75343-128">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="75343-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="75343-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="75343-129">showCategoryName</span></span>|<span data-ttu-id="75343-130">boolean</span><span class="sxs-lookup"><span data-stu-id="75343-130">boolean</span></span>|<span data-ttu-id="75343-131">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="75343-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="75343-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="75343-132">showLegendKey</span></span>|<span data-ttu-id="75343-133">boolean</span><span class="sxs-lookup"><span data-stu-id="75343-133">boolean</span></span>|<span data-ttu-id="75343-134">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="75343-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="75343-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="75343-135">showPercentage</span></span>|<span data-ttu-id="75343-136">boolean</span><span class="sxs-lookup"><span data-stu-id="75343-136">boolean</span></span>|<span data-ttu-id="75343-137">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="75343-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="75343-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="75343-138">showSeriesName</span></span>|<span data-ttu-id="75343-139">boolean</span><span class="sxs-lookup"><span data-stu-id="75343-139">boolean</span></span>|<span data-ttu-id="75343-140">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="75343-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="75343-141">showValue</span><span class="sxs-lookup"><span data-stu-id="75343-141">showValue</span></span>|<span data-ttu-id="75343-142">boolean</span><span class="sxs-lookup"><span data-stu-id="75343-142">boolean</span></span>|<span data-ttu-id="75343-143">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="75343-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75343-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="75343-144">Relationships</span></span>
| <span data-ttu-id="75343-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="75343-145">Relationship</span></span> | <span data-ttu-id="75343-146">Typ</span><span class="sxs-lookup"><span data-stu-id="75343-146">Type</span></span>   |<span data-ttu-id="75343-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75343-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75343-148">format</span><span class="sxs-lookup"><span data-stu-id="75343-148">format</span></span>|[<span data-ttu-id="75343-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="75343-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="75343-p102">Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="75343-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75343-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="75343-152">JSON representation</span></span>

<span data-ttu-id="75343-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="75343-153">Here is a JSON representation of the resource.</span></span>

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
