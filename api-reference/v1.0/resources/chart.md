---
title: Chart-Ressourcentyp
description: Steht für ein Diagrammobjekt in einer Arbeitsmappe.
author: lumine2008
ms.openlocfilehash: c8cbc297c3906a913a6b5962ea8bb0a048d70005
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311746"
---
# <a name="chart-resource-type"></a><span data-ttu-id="2be29-103">Chart-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2be29-103">Chart resource type</span></span>

<span data-ttu-id="2be29-104">Steht für ein Diagrammobjekt in einer Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="2be29-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="2be29-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="2be29-105">Methods</span></span>

| <span data-ttu-id="2be29-106">Methode</span><span class="sxs-lookup"><span data-stu-id="2be29-106">Method</span></span>           | <span data-ttu-id="2be29-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2be29-107">Return Type</span></span>    |<span data-ttu-id="2be29-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2be29-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2be29-109">Chart abrufen</span><span class="sxs-lookup"><span data-stu-id="2be29-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="2be29-110">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="2be29-110">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="2be29-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2be29-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="2be29-112">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="2be29-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="2be29-113">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="2be29-113">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="2be29-114">Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.</span><span class="sxs-lookup"><span data-stu-id="2be29-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="2be29-115">Reihe auflisten</span><span class="sxs-lookup"><span data-stu-id="2be29-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="2be29-116">[WorkbookChartSeries](chartseries.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2be29-116">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="2be29-117">Dient zum Abrufen einer ChartSeries-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="2be29-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="2be29-118">Update</span><span class="sxs-lookup"><span data-stu-id="2be29-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="2be29-119">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="2be29-119">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="2be29-120">Dient zum Aktualisieren des Chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2be29-120">Update Chart object.</span></span> |
|[<span data-ttu-id="2be29-121">Image</span><span class="sxs-lookup"><span data-stu-id="2be29-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="2be29-122">Abbildung der base64-codierten Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2be29-122">Image base64 encoded string</span></span>|<span data-ttu-id="2be29-123">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="2be29-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="2be29-124">Delete</span><span class="sxs-lookup"><span data-stu-id="2be29-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="2be29-125">Keine</span><span class="sxs-lookup"><span data-stu-id="2be29-125">None</span></span>|<span data-ttu-id="2be29-126">Löscht das Diagrammobjekt.</span><span class="sxs-lookup"><span data-stu-id="2be29-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="2be29-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="2be29-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="2be29-128">Keine</span><span class="sxs-lookup"><span data-stu-id="2be29-128">None</span></span>|<span data-ttu-id="2be29-129">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="2be29-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="2be29-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="2be29-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="2be29-131">Keine</span><span class="sxs-lookup"><span data-stu-id="2be29-131">None</span></span>|<span data-ttu-id="2be29-132">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="2be29-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="2be29-133">List</span><span class="sxs-lookup"><span data-stu-id="2be29-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="2be29-134">[WorkbookChart](chart.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2be29-134">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="2be29-135">Dient zum Abrufen der Diagrammobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="2be29-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="2be29-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="2be29-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="2be29-137">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="2be29-137">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="2be29-138">Ruft ein Diagramm anhand seiner Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="2be29-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="2be29-139">Add</span><span class="sxs-lookup"><span data-stu-id="2be29-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="2be29-140">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="2be29-140">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="2be29-141">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="2be29-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="2be29-142">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2be29-142">Properties</span></span>
| <span data-ttu-id="2be29-143">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2be29-143">Property</span></span>     | <span data-ttu-id="2be29-144">Typ</span><span class="sxs-lookup"><span data-stu-id="2be29-144">Type</span></span>   |<span data-ttu-id="2be29-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2be29-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2be29-146">height</span><span class="sxs-lookup"><span data-stu-id="2be29-146">height</span></span>|<span data-ttu-id="2be29-147">double</span><span class="sxs-lookup"><span data-stu-id="2be29-147">double</span></span>|<span data-ttu-id="2be29-148">Die Höhe des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="2be29-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="2be29-149">id</span><span class="sxs-lookup"><span data-stu-id="2be29-149">id</span></span>|<span data-ttu-id="2be29-150">string</span><span class="sxs-lookup"><span data-stu-id="2be29-150">string</span></span>|<span data-ttu-id="2be29-p101">Ruft ein Diagramm anhand seiner Position in der Sammlung ab. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="2be29-153">left</span><span class="sxs-lookup"><span data-stu-id="2be29-153">left</span></span>|<span data-ttu-id="2be29-154">double</span><span class="sxs-lookup"><span data-stu-id="2be29-154">double</span></span>|<span data-ttu-id="2be29-155">Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="2be29-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="2be29-156">name</span><span class="sxs-lookup"><span data-stu-id="2be29-156">name</span></span>|<span data-ttu-id="2be29-157">string</span><span class="sxs-lookup"><span data-stu-id="2be29-157">string</span></span>|<span data-ttu-id="2be29-158">Gibt den Namen eines Diagrammobjekts an.</span><span class="sxs-lookup"><span data-stu-id="2be29-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="2be29-159">top</span><span class="sxs-lookup"><span data-stu-id="2be29-159">top</span></span>|<span data-ttu-id="2be29-160">double</span><span class="sxs-lookup"><span data-stu-id="2be29-160">double</span></span>|<span data-ttu-id="2be29-161">Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).</span><span class="sxs-lookup"><span data-stu-id="2be29-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="2be29-162">width</span><span class="sxs-lookup"><span data-stu-id="2be29-162">width</span></span>|<span data-ttu-id="2be29-163">double</span><span class="sxs-lookup"><span data-stu-id="2be29-163">double</span></span>|<span data-ttu-id="2be29-164">Die Breite des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="2be29-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2be29-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2be29-165">Relationships</span></span>
| <span data-ttu-id="2be29-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2be29-166">Relationship</span></span> | <span data-ttu-id="2be29-167">Typ</span><span class="sxs-lookup"><span data-stu-id="2be29-167">Type</span></span>   |<span data-ttu-id="2be29-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2be29-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2be29-169">Achsen</span><span class="sxs-lookup"><span data-stu-id="2be29-169">axes</span></span>|[<span data-ttu-id="2be29-170">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="2be29-170">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="2be29-p102">Die Achsen des Diagramms. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="2be29-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="2be29-173">dataLabels</span></span>|[<span data-ttu-id="2be29-174">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2be29-174">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="2be29-p103">Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="2be29-177">Format</span><span class="sxs-lookup"><span data-stu-id="2be29-177">format</span></span>|[<span data-ttu-id="2be29-178">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="2be29-178">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="2be29-p104">Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="2be29-181">legend</span><span class="sxs-lookup"><span data-stu-id="2be29-181">legend</span></span>|[<span data-ttu-id="2be29-182">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="2be29-182">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="2be29-p105">Die Legende für das Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="2be29-185">series</span><span class="sxs-lookup"><span data-stu-id="2be29-185">series</span></span>|<span data-ttu-id="2be29-186">[WorkbookChartSeries](chartseries.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2be29-186">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="2be29-p106">Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="2be29-189">title</span><span class="sxs-lookup"><span data-stu-id="2be29-189">title</span></span>|[<span data-ttu-id="2be29-190">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="2be29-190">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="2be29-p107">Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="2be29-193">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="2be29-193">worksheet</span></span>|[<span data-ttu-id="2be29-194">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="2be29-194">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="2be29-p108">Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2be29-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2be29-197">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2be29-197">JSON representation</span></span>

<span data-ttu-id="2be29-198">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2be29-198">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
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