---
title: Chart-Ressourcentyp
description: Steht für ein Diagrammobjekt in einer Arbeitsmappe.
author: lumine2008
ms.openlocfilehash: cf03a768422fca50e68b88a64b9991aad878466f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325718"
---
# <a name="chart-resource-type"></a><span data-ttu-id="f6eee-103">Chart-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f6eee-103">Chart resource type</span></span>

> <span data-ttu-id="f6eee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6eee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6eee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6eee-106">Steht für ein Diagrammobjekt in einer Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="f6eee-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="f6eee-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="f6eee-107">Methods</span></span>

| <span data-ttu-id="f6eee-108">Methode</span><span class="sxs-lookup"><span data-stu-id="f6eee-108">Method</span></span>           | <span data-ttu-id="f6eee-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f6eee-109">Return Type</span></span>    |<span data-ttu-id="f6eee-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6eee-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f6eee-111">Chart abrufen</span><span class="sxs-lookup"><span data-stu-id="f6eee-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="f6eee-112">Chart</span><span class="sxs-lookup"><span data-stu-id="f6eee-112">Chart</span></span>](chart.md) |<span data-ttu-id="f6eee-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6eee-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="f6eee-114">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="f6eee-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="f6eee-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="f6eee-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="f6eee-116">Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.</span><span class="sxs-lookup"><span data-stu-id="f6eee-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="f6eee-117">Reihe auflisten</span><span class="sxs-lookup"><span data-stu-id="f6eee-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="f6eee-118">[ChartSeries-Sammlung](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="f6eee-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="f6eee-119">Dient zum Abrufen einer ChartSeries-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="f6eee-119">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="f6eee-120">Update</span><span class="sxs-lookup"><span data-stu-id="f6eee-120">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="f6eee-121">Chart</span><span class="sxs-lookup"><span data-stu-id="f6eee-121">Chart</span></span>](chart.md)   |<span data-ttu-id="f6eee-122">Dient zum Aktualisieren des Chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6eee-122">Update Chart object.</span></span> |
|[<span data-ttu-id="f6eee-123">Image</span><span class="sxs-lookup"><span data-stu-id="f6eee-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="f6eee-124">Abbildung der base64-codierten Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6eee-124">Image base64 encoded string</span></span>|<span data-ttu-id="f6eee-125">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="f6eee-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="f6eee-126">Delete</span><span class="sxs-lookup"><span data-stu-id="f6eee-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="f6eee-127">Keine</span><span class="sxs-lookup"><span data-stu-id="f6eee-127">None</span></span>|<span data-ttu-id="f6eee-128">Löscht das Diagrammobjekt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="f6eee-129">Setdata</span><span class="sxs-lookup"><span data-stu-id="f6eee-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="f6eee-130">Keine</span><span class="sxs-lookup"><span data-stu-id="f6eee-130">None</span></span>|<span data-ttu-id="f6eee-131">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="f6eee-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="f6eee-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="f6eee-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="f6eee-133">Keine</span><span class="sxs-lookup"><span data-stu-id="f6eee-133">None</span></span>|<span data-ttu-id="f6eee-134">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="f6eee-135">List</span><span class="sxs-lookup"><span data-stu-id="f6eee-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="f6eee-136">[Diagrammsammlung](chart.md)</span><span class="sxs-lookup"><span data-stu-id="f6eee-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="f6eee-137">Dient zum Abrufen der Diagrammobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="f6eee-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="f6eee-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="f6eee-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="f6eee-139">Chart</span><span class="sxs-lookup"><span data-stu-id="f6eee-139">Chart</span></span>](chart.md)|<span data-ttu-id="f6eee-140">Ruft ein Diagramm anhand seiner Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="f6eee-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="f6eee-141">Add</span><span class="sxs-lookup"><span data-stu-id="f6eee-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="f6eee-142">Chart</span><span class="sxs-lookup"><span data-stu-id="f6eee-142">Chart</span></span>](chart.md)|<span data-ttu-id="f6eee-143">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="f6eee-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6eee-144">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6eee-144">Properties</span></span>
| <span data-ttu-id="f6eee-145">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6eee-145">Property</span></span>     | <span data-ttu-id="f6eee-146">Typ</span><span class="sxs-lookup"><span data-stu-id="f6eee-146">Type</span></span>   |<span data-ttu-id="f6eee-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6eee-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6eee-148">height</span><span class="sxs-lookup"><span data-stu-id="f6eee-148">height</span></span>|<span data-ttu-id="f6eee-149">double</span><span class="sxs-lookup"><span data-stu-id="f6eee-149">double</span></span>|<span data-ttu-id="f6eee-150">Die Höhe des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="f6eee-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="f6eee-151">id</span><span class="sxs-lookup"><span data-stu-id="f6eee-151">id</span></span>|<span data-ttu-id="f6eee-152">string</span><span class="sxs-lookup"><span data-stu-id="f6eee-152">string</span></span>|<span data-ttu-id="f6eee-p102">Ruft ein Diagramm anhand seiner Position in der Sammlung ab. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="f6eee-155">left</span><span class="sxs-lookup"><span data-stu-id="f6eee-155">left</span></span>|<span data-ttu-id="f6eee-156">double</span><span class="sxs-lookup"><span data-stu-id="f6eee-156">double</span></span>|<span data-ttu-id="f6eee-157">Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="f6eee-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="f6eee-158">name</span><span class="sxs-lookup"><span data-stu-id="f6eee-158">name</span></span>|<span data-ttu-id="f6eee-159">string</span><span class="sxs-lookup"><span data-stu-id="f6eee-159">string</span></span>|<span data-ttu-id="f6eee-160">Gibt den Namen eines Diagrammobjekts an.</span><span class="sxs-lookup"><span data-stu-id="f6eee-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="f6eee-161">top</span><span class="sxs-lookup"><span data-stu-id="f6eee-161">top</span></span>|<span data-ttu-id="f6eee-162">double</span><span class="sxs-lookup"><span data-stu-id="f6eee-162">double</span></span>|<span data-ttu-id="f6eee-163">Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).</span><span class="sxs-lookup"><span data-stu-id="f6eee-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="f6eee-164">width</span><span class="sxs-lookup"><span data-stu-id="f6eee-164">width</span></span>|<span data-ttu-id="f6eee-165">double</span><span class="sxs-lookup"><span data-stu-id="f6eee-165">double</span></span>|<span data-ttu-id="f6eee-166">Die Breite des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="f6eee-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6eee-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6eee-167">Relationships</span></span>
| <span data-ttu-id="f6eee-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f6eee-168">Relationship</span></span> | <span data-ttu-id="f6eee-169">Typ</span><span class="sxs-lookup"><span data-stu-id="f6eee-169">Type</span></span>   |<span data-ttu-id="f6eee-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6eee-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6eee-171">Achsen</span><span class="sxs-lookup"><span data-stu-id="f6eee-171">axes</span></span>|[<span data-ttu-id="f6eee-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="f6eee-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="f6eee-p103">Die Achsen des Diagramms. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="f6eee-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="f6eee-175">dataLabels</span></span>|[<span data-ttu-id="f6eee-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="f6eee-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="f6eee-p104">Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="f6eee-179">Format</span><span class="sxs-lookup"><span data-stu-id="f6eee-179">format</span></span>|[<span data-ttu-id="f6eee-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="f6eee-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="f6eee-p105">Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="f6eee-183">legend</span><span class="sxs-lookup"><span data-stu-id="f6eee-183">legend</span></span>|[<span data-ttu-id="f6eee-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="f6eee-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="f6eee-p106">Die Legende für das Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="f6eee-187">series</span><span class="sxs-lookup"><span data-stu-id="f6eee-187">series</span></span>|<span data-ttu-id="f6eee-188">[ChartSeries-Sammlung](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="f6eee-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="f6eee-p107">Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="f6eee-191">title</span><span class="sxs-lookup"><span data-stu-id="f6eee-191">title</span></span>|[<span data-ttu-id="f6eee-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="f6eee-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="f6eee-p108">Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="f6eee-195">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="f6eee-195">worksheet</span></span>|[<span data-ttu-id="f6eee-196">Worksheet</span><span class="sxs-lookup"><span data-stu-id="f6eee-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="f6eee-p109">Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6eee-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6eee-199">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6eee-199">JSON representation</span></span>

<span data-ttu-id="f6eee-200">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6eee-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->