---
title: ChartDataLabels-Ressourcentyp
description: Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bda2c1849f154435608f311671026e224b0c7e3c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642324"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="33ec9-103">ChartDataLabels-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="33ec9-103">ChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33ec9-104">Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.</span><span class="sxs-lookup"><span data-stu-id="33ec9-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="33ec9-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="33ec9-105">Methods</span></span>

| <span data-ttu-id="33ec9-106">Methode</span><span class="sxs-lookup"><span data-stu-id="33ec9-106">Method</span></span>           | <span data-ttu-id="33ec9-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="33ec9-107">Return Type</span></span>    |<span data-ttu-id="33ec9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33ec9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33ec9-109">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="33ec9-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="33ec9-110">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="33ec9-110">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="33ec9-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="33ec9-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="33ec9-112">Update</span><span class="sxs-lookup"><span data-stu-id="33ec9-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="33ec9-113">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="33ec9-113">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="33ec9-114">Dient zum Aktualisieren des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="33ec9-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="33ec9-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="33ec9-115">Properties</span></span>
| <span data-ttu-id="33ec9-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33ec9-116">Property</span></span>     | <span data-ttu-id="33ec9-117">Typ</span><span class="sxs-lookup"><span data-stu-id="33ec9-117">Type</span></span>   |<span data-ttu-id="33ec9-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33ec9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33ec9-119">position</span><span class="sxs-lookup"><span data-stu-id="33ec9-119">position</span></span>|<span data-ttu-id="33ec9-120">string</span><span class="sxs-lookup"><span data-stu-id="33ec9-120">string</span></span>|<span data-ttu-id="33ec9-p101">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt. Mögliche Werte: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="33ec9-p101">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="33ec9-123">Separator</span><span class="sxs-lookup"><span data-stu-id="33ec9-123">separator</span></span>|<span data-ttu-id="33ec9-124">string</span><span class="sxs-lookup"><span data-stu-id="33ec9-124">string</span></span>|<span data-ttu-id="33ec9-125">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="33ec9-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="33ec9-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="33ec9-126">showBubbleSize</span></span>|<span data-ttu-id="33ec9-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33ec9-127">boolean</span></span>|<span data-ttu-id="33ec9-128">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33ec9-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="33ec9-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="33ec9-129">showCategoryName</span></span>|<span data-ttu-id="33ec9-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33ec9-130">boolean</span></span>|<span data-ttu-id="33ec9-131">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33ec9-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="33ec9-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="33ec9-132">showLegendKey</span></span>|<span data-ttu-id="33ec9-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33ec9-133">boolean</span></span>|<span data-ttu-id="33ec9-134">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33ec9-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="33ec9-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="33ec9-135">showPercentage</span></span>|<span data-ttu-id="33ec9-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33ec9-136">boolean</span></span>|<span data-ttu-id="33ec9-137">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33ec9-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="33ec9-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="33ec9-138">showSeriesName</span></span>|<span data-ttu-id="33ec9-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33ec9-139">boolean</span></span>|<span data-ttu-id="33ec9-140">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33ec9-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="33ec9-141">showValue</span><span class="sxs-lookup"><span data-stu-id="33ec9-141">showValue</span></span>|<span data-ttu-id="33ec9-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33ec9-142">boolean</span></span>|<span data-ttu-id="33ec9-143">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33ec9-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33ec9-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="33ec9-144">Relationships</span></span>
| <span data-ttu-id="33ec9-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="33ec9-145">Relationship</span></span> | <span data-ttu-id="33ec9-146">Typ</span><span class="sxs-lookup"><span data-stu-id="33ec9-146">Type</span></span>   |<span data-ttu-id="33ec9-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33ec9-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33ec9-148">format</span><span class="sxs-lookup"><span data-stu-id="33ec9-148">format</span></span>|[<span data-ttu-id="33ec9-149">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="33ec9-149">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="33ec9-p102">Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33ec9-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33ec9-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33ec9-152">JSON representation</span></span>

<span data-ttu-id="33ec9-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="33ec9-153">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabels.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
