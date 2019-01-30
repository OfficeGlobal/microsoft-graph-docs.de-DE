---
title: Chart-Ressourcentyp
description: Steht für ein Diagrammobjekt in einer Arbeitsmappe.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643234"
---
# <a name="chart-resource-type"></a><span data-ttu-id="c4f61-103">Chart-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c4f61-103">Chart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4f61-104">Steht für ein Diagrammobjekt in einer Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="c4f61-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="c4f61-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="c4f61-105">Methods</span></span>

| <span data-ttu-id="c4f61-106">Methode</span><span class="sxs-lookup"><span data-stu-id="c4f61-106">Method</span></span>           | <span data-ttu-id="c4f61-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c4f61-107">Return Type</span></span>    |<span data-ttu-id="c4f61-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4f61-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4f61-109">Chart abrufen</span><span class="sxs-lookup"><span data-stu-id="c4f61-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="c4f61-110">Chart</span><span class="sxs-lookup"><span data-stu-id="c4f61-110">Chart</span></span>](chart.md) |<span data-ttu-id="c4f61-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4f61-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="c4f61-112">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="c4f61-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="c4f61-113">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c4f61-113">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="c4f61-114">Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.</span><span class="sxs-lookup"><span data-stu-id="c4f61-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="c4f61-115">Reihe auflisten</span><span class="sxs-lookup"><span data-stu-id="c4f61-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="c4f61-116">[ChartSeries-Sammlung](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="c4f61-116">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="c4f61-117">Dient zum Abrufen einer ChartSeries-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="c4f61-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="c4f61-118">Update</span><span class="sxs-lookup"><span data-stu-id="c4f61-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="c4f61-119">Chart</span><span class="sxs-lookup"><span data-stu-id="c4f61-119">Chart</span></span>](chart.md)   |<span data-ttu-id="c4f61-120">Dient zum Aktualisieren des Chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4f61-120">Update Chart object.</span></span> |
|[<span data-ttu-id="c4f61-121">Image</span><span class="sxs-lookup"><span data-stu-id="c4f61-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="c4f61-122">Abbildung der base64-codierten Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4f61-122">Image base64 encoded string</span></span>|<span data-ttu-id="c4f61-123">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="c4f61-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="c4f61-124">Delete</span><span class="sxs-lookup"><span data-stu-id="c4f61-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="c4f61-125">Keine</span><span class="sxs-lookup"><span data-stu-id="c4f61-125">None</span></span>|<span data-ttu-id="c4f61-126">Löscht das Diagrammobjekt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="c4f61-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="c4f61-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="c4f61-128">Keine</span><span class="sxs-lookup"><span data-stu-id="c4f61-128">None</span></span>|<span data-ttu-id="c4f61-129">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="c4f61-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="c4f61-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="c4f61-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="c4f61-131">Keine</span><span class="sxs-lookup"><span data-stu-id="c4f61-131">None</span></span>|<span data-ttu-id="c4f61-132">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="c4f61-133">List</span><span class="sxs-lookup"><span data-stu-id="c4f61-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="c4f61-134">[Diagrammsammlung](chart.md)</span><span class="sxs-lookup"><span data-stu-id="c4f61-134">[Chart](chart.md) collection</span></span> |<span data-ttu-id="c4f61-135">Dient zum Abrufen der Diagrammobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="c4f61-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="c4f61-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="c4f61-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="c4f61-137">Chart</span><span class="sxs-lookup"><span data-stu-id="c4f61-137">Chart</span></span>](chart.md)|<span data-ttu-id="c4f61-138">Ruft ein Diagramm anhand seiner Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="c4f61-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="c4f61-139">Add</span><span class="sxs-lookup"><span data-stu-id="c4f61-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="c4f61-140">Chart</span><span class="sxs-lookup"><span data-stu-id="c4f61-140">Chart</span></span>](chart.md)|<span data-ttu-id="c4f61-141">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="c4f61-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4f61-142">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c4f61-142">Properties</span></span>
| <span data-ttu-id="c4f61-143">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4f61-143">Property</span></span>     | <span data-ttu-id="c4f61-144">Typ</span><span class="sxs-lookup"><span data-stu-id="c4f61-144">Type</span></span>   |<span data-ttu-id="c4f61-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4f61-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4f61-146">height</span><span class="sxs-lookup"><span data-stu-id="c4f61-146">height</span></span>|<span data-ttu-id="c4f61-147">double</span><span class="sxs-lookup"><span data-stu-id="c4f61-147">double</span></span>|<span data-ttu-id="c4f61-148">Die Höhe des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="c4f61-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="c4f61-149">id</span><span class="sxs-lookup"><span data-stu-id="c4f61-149">id</span></span>|<span data-ttu-id="c4f61-150">string</span><span class="sxs-lookup"><span data-stu-id="c4f61-150">string</span></span>|<span data-ttu-id="c4f61-p101">Ruft ein Diagramm anhand seiner Position in der Sammlung ab. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="c4f61-153">left</span><span class="sxs-lookup"><span data-stu-id="c4f61-153">left</span></span>|<span data-ttu-id="c4f61-154">double</span><span class="sxs-lookup"><span data-stu-id="c4f61-154">double</span></span>|<span data-ttu-id="c4f61-155">Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="c4f61-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="c4f61-156">name</span><span class="sxs-lookup"><span data-stu-id="c4f61-156">name</span></span>|<span data-ttu-id="c4f61-157">string</span><span class="sxs-lookup"><span data-stu-id="c4f61-157">string</span></span>|<span data-ttu-id="c4f61-158">Gibt den Namen eines Diagrammobjekts an.</span><span class="sxs-lookup"><span data-stu-id="c4f61-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="c4f61-159">top</span><span class="sxs-lookup"><span data-stu-id="c4f61-159">top</span></span>|<span data-ttu-id="c4f61-160">double</span><span class="sxs-lookup"><span data-stu-id="c4f61-160">double</span></span>|<span data-ttu-id="c4f61-161">Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).</span><span class="sxs-lookup"><span data-stu-id="c4f61-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="c4f61-162">width</span><span class="sxs-lookup"><span data-stu-id="c4f61-162">width</span></span>|<span data-ttu-id="c4f61-163">double</span><span class="sxs-lookup"><span data-stu-id="c4f61-163">double</span></span>|<span data-ttu-id="c4f61-164">Die Breite des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="c4f61-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4f61-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c4f61-165">Relationships</span></span>
| <span data-ttu-id="c4f61-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c4f61-166">Relationship</span></span> | <span data-ttu-id="c4f61-167">Typ</span><span class="sxs-lookup"><span data-stu-id="c4f61-167">Type</span></span>   |<span data-ttu-id="c4f61-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4f61-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4f61-169">Achsen</span><span class="sxs-lookup"><span data-stu-id="c4f61-169">axes</span></span>|[<span data-ttu-id="c4f61-170">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="c4f61-170">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="c4f61-p102">Die Achsen des Diagramms. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="c4f61-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="c4f61-173">dataLabels</span></span>|[<span data-ttu-id="c4f61-174">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="c4f61-174">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="c4f61-p103">Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="c4f61-177">Format</span><span class="sxs-lookup"><span data-stu-id="c4f61-177">format</span></span>|[<span data-ttu-id="c4f61-178">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="c4f61-178">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="c4f61-p104">Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="c4f61-181">legend</span><span class="sxs-lookup"><span data-stu-id="c4f61-181">legend</span></span>|[<span data-ttu-id="c4f61-182">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="c4f61-182">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="c4f61-p105">Die Legende für das Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="c4f61-185">series</span><span class="sxs-lookup"><span data-stu-id="c4f61-185">series</span></span>|<span data-ttu-id="c4f61-186">[ChartSeries-Sammlung](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="c4f61-186">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="c4f61-p106">Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="c4f61-189">title</span><span class="sxs-lookup"><span data-stu-id="c4f61-189">title</span></span>|[<span data-ttu-id="c4f61-190">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="c4f61-190">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="c4f61-p107">Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="c4f61-193">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="c4f61-193">worksheet</span></span>|[<span data-ttu-id="c4f61-194">Worksheet</span><span class="sxs-lookup"><span data-stu-id="c4f61-194">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="c4f61-p108">Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4f61-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4f61-197">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c4f61-197">JSON representation</span></span>

<span data-ttu-id="c4f61-198">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c4f61-198">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
