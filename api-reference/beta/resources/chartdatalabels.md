---
title: ChartDataLabels-Ressourcentyp
description: Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.
ms.openlocfilehash: d226c5edb3fecc3a2e27fae32060f786f790d7e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063351"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="91bfd-103">ChartDataLabels-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91bfd-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="91bfd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91bfd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91bfd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91bfd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91bfd-106">Stellt eine Sammlung aller Datenbeschriftungen an einem Diagrammpunkt dar.</span><span class="sxs-lookup"><span data-stu-id="91bfd-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="91bfd-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="91bfd-107">Methods</span></span>

| <span data-ttu-id="91bfd-108">Methode</span><span class="sxs-lookup"><span data-stu-id="91bfd-108">Method</span></span>           | <span data-ttu-id="91bfd-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="91bfd-109">Return Type</span></span>    |<span data-ttu-id="91bfd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91bfd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91bfd-111">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="91bfd-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="91bfd-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="91bfd-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="91bfd-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91bfd-113">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="91bfd-114">Update</span><span class="sxs-lookup"><span data-stu-id="91bfd-114">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="91bfd-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="91bfd-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="91bfd-116">Dient zum Aktualisieren des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91bfd-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="91bfd-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91bfd-117">Properties</span></span>
| <span data-ttu-id="91bfd-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91bfd-118">Property</span></span>     | <span data-ttu-id="91bfd-119">Typ</span><span class="sxs-lookup"><span data-stu-id="91bfd-119">Type</span></span>   |<span data-ttu-id="91bfd-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91bfd-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91bfd-121">position</span><span class="sxs-lookup"><span data-stu-id="91bfd-121">position</span></span>|<span data-ttu-id="91bfd-122">string</span><span class="sxs-lookup"><span data-stu-id="91bfd-122">string</span></span>|<span data-ttu-id="91bfd-p102">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt. Mögliche Werte: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="91bfd-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="91bfd-125">Separator</span><span class="sxs-lookup"><span data-stu-id="91bfd-125">separator</span></span>|<span data-ttu-id="91bfd-126">string</span><span class="sxs-lookup"><span data-stu-id="91bfd-126">string</span></span>|<span data-ttu-id="91bfd-127">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="91bfd-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="91bfd-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="91bfd-128">showBubbleSize</span></span>|<span data-ttu-id="91bfd-129">boolean</span><span class="sxs-lookup"><span data-stu-id="91bfd-129">boolean</span></span>|<span data-ttu-id="91bfd-130">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="91bfd-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="91bfd-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="91bfd-131">showCategoryName</span></span>|<span data-ttu-id="91bfd-132">boolean</span><span class="sxs-lookup"><span data-stu-id="91bfd-132">boolean</span></span>|<span data-ttu-id="91bfd-133">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="91bfd-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="91bfd-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="91bfd-134">showLegendKey</span></span>|<span data-ttu-id="91bfd-135">boolean</span><span class="sxs-lookup"><span data-stu-id="91bfd-135">boolean</span></span>|<span data-ttu-id="91bfd-136">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="91bfd-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="91bfd-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="91bfd-137">showPercentage</span></span>|<span data-ttu-id="91bfd-138">boolean</span><span class="sxs-lookup"><span data-stu-id="91bfd-138">boolean</span></span>|<span data-ttu-id="91bfd-139">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="91bfd-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="91bfd-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="91bfd-140">showSeriesName</span></span>|<span data-ttu-id="91bfd-141">boolean</span><span class="sxs-lookup"><span data-stu-id="91bfd-141">boolean</span></span>|<span data-ttu-id="91bfd-142">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="91bfd-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="91bfd-143">showValue</span><span class="sxs-lookup"><span data-stu-id="91bfd-143">showValue</span></span>|<span data-ttu-id="91bfd-144">boolean</span><span class="sxs-lookup"><span data-stu-id="91bfd-144">boolean</span></span>|<span data-ttu-id="91bfd-145">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="91bfd-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91bfd-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91bfd-146">Relationships</span></span>
| <span data-ttu-id="91bfd-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="91bfd-147">Relationship</span></span> | <span data-ttu-id="91bfd-148">Typ</span><span class="sxs-lookup"><span data-stu-id="91bfd-148">Type</span></span>   |<span data-ttu-id="91bfd-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91bfd-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91bfd-150">Format</span><span class="sxs-lookup"><span data-stu-id="91bfd-150">format</span></span>|[<span data-ttu-id="91bfd-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="91bfd-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="91bfd-p103">Stellt das Format der Diagrammdatenbeschriftungen dar, einschließlich Füllung und Formatierung der Schriftart. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91bfd-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91bfd-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91bfd-154">JSON representation</span></span>

<span data-ttu-id="91bfd-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91bfd-155">Here is a JSON representation of the resource.</span></span>

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