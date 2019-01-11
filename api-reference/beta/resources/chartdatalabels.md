---
title: ChartDataLabels-Ressourcentyp
description: Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7e45db4129422c32af809d46c076b2f6d82eff89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876195"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="0d63d-103">ChartDataLabels-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0d63d-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="0d63d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0d63d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d63d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d63d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d63d-106">Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.</span><span class="sxs-lookup"><span data-stu-id="0d63d-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="0d63d-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="0d63d-107">Methods</span></span>

| <span data-ttu-id="0d63d-108">Methode</span><span class="sxs-lookup"><span data-stu-id="0d63d-108">Method</span></span>           | <span data-ttu-id="0d63d-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0d63d-109">Return Type</span></span>    |<span data-ttu-id="0d63d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d63d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d63d-111">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="0d63d-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="0d63d-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0d63d-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0d63d-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d63d-113">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="0d63d-114">Update</span><span class="sxs-lookup"><span data-stu-id="0d63d-114">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="0d63d-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0d63d-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0d63d-116">Dient zum Aktualisieren des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d63d-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d63d-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d63d-117">Properties</span></span>
| <span data-ttu-id="0d63d-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d63d-118">Property</span></span>     | <span data-ttu-id="0d63d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="0d63d-119">Type</span></span>   |<span data-ttu-id="0d63d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d63d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d63d-121">position</span><span class="sxs-lookup"><span data-stu-id="0d63d-121">position</span></span>|<span data-ttu-id="0d63d-122">string</span><span class="sxs-lookup"><span data-stu-id="0d63d-122">string</span></span>|<span data-ttu-id="0d63d-p102">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt. Mögliche Werte: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="0d63d-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="0d63d-125">Separator</span><span class="sxs-lookup"><span data-stu-id="0d63d-125">separator</span></span>|<span data-ttu-id="0d63d-126">string</span><span class="sxs-lookup"><span data-stu-id="0d63d-126">string</span></span>|<span data-ttu-id="0d63d-127">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="0d63d-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0d63d-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0d63d-128">showBubbleSize</span></span>|<span data-ttu-id="0d63d-129">boolean</span><span class="sxs-lookup"><span data-stu-id="0d63d-129">boolean</span></span>|<span data-ttu-id="0d63d-130">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0d63d-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0d63d-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0d63d-131">showCategoryName</span></span>|<span data-ttu-id="0d63d-132">boolean</span><span class="sxs-lookup"><span data-stu-id="0d63d-132">boolean</span></span>|<span data-ttu-id="0d63d-133">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0d63d-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0d63d-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0d63d-134">showLegendKey</span></span>|<span data-ttu-id="0d63d-135">boolean</span><span class="sxs-lookup"><span data-stu-id="0d63d-135">boolean</span></span>|<span data-ttu-id="0d63d-136">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0d63d-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0d63d-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0d63d-137">showPercentage</span></span>|<span data-ttu-id="0d63d-138">boolean</span><span class="sxs-lookup"><span data-stu-id="0d63d-138">boolean</span></span>|<span data-ttu-id="0d63d-139">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0d63d-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0d63d-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0d63d-140">showSeriesName</span></span>|<span data-ttu-id="0d63d-141">boolean</span><span class="sxs-lookup"><span data-stu-id="0d63d-141">boolean</span></span>|<span data-ttu-id="0d63d-142">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0d63d-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0d63d-143">showValue</span><span class="sxs-lookup"><span data-stu-id="0d63d-143">showValue</span></span>|<span data-ttu-id="0d63d-144">boolean</span><span class="sxs-lookup"><span data-stu-id="0d63d-144">boolean</span></span>|<span data-ttu-id="0d63d-145">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0d63d-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d63d-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d63d-146">Relationships</span></span>
| <span data-ttu-id="0d63d-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0d63d-147">Relationship</span></span> | <span data-ttu-id="0d63d-148">Typ</span><span class="sxs-lookup"><span data-stu-id="0d63d-148">Type</span></span>   |<span data-ttu-id="0d63d-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d63d-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d63d-150">format</span><span class="sxs-lookup"><span data-stu-id="0d63d-150">format</span></span>|[<span data-ttu-id="0d63d-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="0d63d-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="0d63d-p103">Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0d63d-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d63d-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d63d-154">JSON representation</span></span>

<span data-ttu-id="0d63d-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d63d-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
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
