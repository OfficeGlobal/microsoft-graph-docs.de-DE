---
title: Chart-Ressourcentyp
description: Steht für ein Diagrammobjekt in einer Arbeitsmappe.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529523"
---
# <a name="chart-resource-type"></a><span data-ttu-id="18a4f-103">Chart-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="18a4f-103">Chart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18a4f-104">Steht für ein Diagrammobjekt in einer Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="18a4f-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="18a4f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="18a4f-105">Methods</span></span>

| <span data-ttu-id="18a4f-106">Methode</span><span class="sxs-lookup"><span data-stu-id="18a4f-106">Method</span></span>           | <span data-ttu-id="18a4f-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="18a4f-107">Return Type</span></span>    |<span data-ttu-id="18a4f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18a4f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18a4f-109">Chart abrufen</span><span class="sxs-lookup"><span data-stu-id="18a4f-109">[Get Chart](../api/chart-get.md)</span></span> | [<span data-ttu-id="18a4f-110">Chart</span><span class="sxs-lookup"><span data-stu-id="18a4f-110">Chart</span></span>](chart.md) |<span data-ttu-id="18a4f-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="18a4f-111">Read properties and relationships of chart object.</span></span>|
|<span data-ttu-id="18a4f-112">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="18a4f-112">[Create ChartSeries](../api/chart-post-series.md)</span></span> |<span data-ttu-id="18a4f-113">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="18a4f-113">[ChartSeries](chartseries.md)</span></span>| <span data-ttu-id="18a4f-114">Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.</span><span class="sxs-lookup"><span data-stu-id="18a4f-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|<span data-ttu-id="18a4f-115">Reihe auflisten</span><span class="sxs-lookup"><span data-stu-id="18a4f-115">[List series](../api/chart-list-series.md)</span></span> |<span data-ttu-id="18a4f-116">ChartSeries-Sammlung</span><span class="sxs-lookup"><span data-stu-id="18a4f-116">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="18a4f-117">Dient zum Abrufen einer ChartSeries-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="18a4f-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="18a4f-118">Update</span><span class="sxs-lookup"><span data-stu-id="18a4f-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="18a4f-119">Chart</span><span class="sxs-lookup"><span data-stu-id="18a4f-119">Chart</span></span>](chart.md)   |<span data-ttu-id="18a4f-120">Dient zum Aktualisieren des Chart-Objekts.</span><span class="sxs-lookup"><span data-stu-id="18a4f-120">Update Chart object.</span></span> |
|[<span data-ttu-id="18a4f-121">Image</span><span class="sxs-lookup"><span data-stu-id="18a4f-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="18a4f-122">Abbildung der base64-codierten Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="18a4f-122">Image base64 encoded string</span></span>|<span data-ttu-id="18a4f-123">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="18a4f-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="18a4f-124">Delete</span><span class="sxs-lookup"><span data-stu-id="18a4f-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="18a4f-125">Keine</span><span class="sxs-lookup"><span data-stu-id="18a4f-125">None</span></span>|<span data-ttu-id="18a4f-126">Löscht das Diagrammobjekt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="18a4f-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="18a4f-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="18a4f-128">Keine</span><span class="sxs-lookup"><span data-stu-id="18a4f-128">None</span></span>|<span data-ttu-id="18a4f-129">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="18a4f-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="18a4f-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="18a4f-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="18a4f-131">Keine</span><span class="sxs-lookup"><span data-stu-id="18a4f-131">None</span></span>|<span data-ttu-id="18a4f-132">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="18a4f-133">List</span><span class="sxs-lookup"><span data-stu-id="18a4f-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="18a4f-134">Diagrammsammlung</span><span class="sxs-lookup"><span data-stu-id="18a4f-134">[Chart](chart.md) collection</span></span> |<span data-ttu-id="18a4f-135">Dient zum Abrufen der Diagrammobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="18a4f-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="18a4f-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="18a4f-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="18a4f-137">Chart</span><span class="sxs-lookup"><span data-stu-id="18a4f-137">Chart</span></span>](chart.md)|<span data-ttu-id="18a4f-138">Ruft ein Diagramm anhand seiner Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="18a4f-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="18a4f-139">Add</span><span class="sxs-lookup"><span data-stu-id="18a4f-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="18a4f-140">Chart</span><span class="sxs-lookup"><span data-stu-id="18a4f-140">Chart</span></span>](chart.md)|<span data-ttu-id="18a4f-141">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="18a4f-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="18a4f-142">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="18a4f-142">Properties</span></span>
| <span data-ttu-id="18a4f-143">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="18a4f-143">Property</span></span>     | <span data-ttu-id="18a4f-144">Typ</span><span class="sxs-lookup"><span data-stu-id="18a4f-144">Type</span></span>   |<span data-ttu-id="18a4f-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18a4f-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18a4f-146">height</span><span class="sxs-lookup"><span data-stu-id="18a4f-146">height</span></span>|<span data-ttu-id="18a4f-147">double</span><span class="sxs-lookup"><span data-stu-id="18a4f-147">double</span></span>|<span data-ttu-id="18a4f-148">Die Höhe des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="18a4f-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="18a4f-149">id</span><span class="sxs-lookup"><span data-stu-id="18a4f-149">id</span></span>|<span data-ttu-id="18a4f-150">string</span><span class="sxs-lookup"><span data-stu-id="18a4f-150">string</span></span>|<span data-ttu-id="18a4f-p101">Ruft ein Diagramm anhand seiner Position in der Sammlung ab. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="18a4f-153">left</span><span class="sxs-lookup"><span data-stu-id="18a4f-153">left</span></span>|<span data-ttu-id="18a4f-154">double</span><span class="sxs-lookup"><span data-stu-id="18a4f-154">double</span></span>|<span data-ttu-id="18a4f-155">Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="18a4f-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="18a4f-156">name</span><span class="sxs-lookup"><span data-stu-id="18a4f-156">name</span></span>|<span data-ttu-id="18a4f-157">string</span><span class="sxs-lookup"><span data-stu-id="18a4f-157">string</span></span>|<span data-ttu-id="18a4f-158">Gibt den Namen eines Diagrammobjekts an.</span><span class="sxs-lookup"><span data-stu-id="18a4f-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="18a4f-159">top</span><span class="sxs-lookup"><span data-stu-id="18a4f-159">top</span></span>|<span data-ttu-id="18a4f-160">double</span><span class="sxs-lookup"><span data-stu-id="18a4f-160">double</span></span>|<span data-ttu-id="18a4f-161">Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).</span><span class="sxs-lookup"><span data-stu-id="18a4f-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="18a4f-162">width</span><span class="sxs-lookup"><span data-stu-id="18a4f-162">width</span></span>|<span data-ttu-id="18a4f-163">double</span><span class="sxs-lookup"><span data-stu-id="18a4f-163">double</span></span>|<span data-ttu-id="18a4f-164">Die Breite des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="18a4f-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18a4f-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="18a4f-165">Relationships</span></span>
| <span data-ttu-id="18a4f-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="18a4f-166">Relationship</span></span> | <span data-ttu-id="18a4f-167">Typ</span><span class="sxs-lookup"><span data-stu-id="18a4f-167">Type</span></span>   |<span data-ttu-id="18a4f-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18a4f-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18a4f-169">Achsen</span><span class="sxs-lookup"><span data-stu-id="18a4f-169">axes</span></span>|[<span data-ttu-id="18a4f-170">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="18a4f-170">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="18a4f-p102">Die Achsen des Diagramms. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="18a4f-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="18a4f-173">dataLabels</span></span>|[<span data-ttu-id="18a4f-174">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="18a4f-174">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="18a4f-p103">Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="18a4f-177">Format</span><span class="sxs-lookup"><span data-stu-id="18a4f-177">format</span></span>|[<span data-ttu-id="18a4f-178">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="18a4f-178">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="18a4f-p104">Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="18a4f-181">legend</span><span class="sxs-lookup"><span data-stu-id="18a4f-181">legend</span></span>|[<span data-ttu-id="18a4f-182">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="18a4f-182">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="18a4f-p105">Die Legende für das Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="18a4f-185">series</span><span class="sxs-lookup"><span data-stu-id="18a4f-185">series</span></span>|<span data-ttu-id="18a4f-186">[ChartSeries-Sammlung](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="18a4f-186">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="18a4f-p106">Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="18a4f-189">title</span><span class="sxs-lookup"><span data-stu-id="18a4f-189">title</span></span>|[<span data-ttu-id="18a4f-190">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="18a4f-190">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="18a4f-p107">Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="18a4f-193">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="18a4f-193">worksheet</span></span>|[<span data-ttu-id="18a4f-194">Worksheet</span><span class="sxs-lookup"><span data-stu-id="18a4f-194">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="18a4f-p108">Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18a4f-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18a4f-197">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="18a4f-197">JSON representation</span></span>

<span data-ttu-id="18a4f-198">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="18a4f-198">Here is a JSON representation of the resource.</span></span>

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
