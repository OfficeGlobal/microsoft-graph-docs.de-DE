---
title: ChartSeries-Ressourcentyp
description: Stellt eine Datenreihe in einem Diagramm dar.
author: lumine2008
ms.openlocfilehash: 60cd3e29f1b2c2f106fae0fdfb76b18657d68120
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314490"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="194d9-103">ChartSeries-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="194d9-103">ChartSeries resource type</span></span>

<span data-ttu-id="194d9-104">Stellt eine Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="194d9-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="194d9-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="194d9-105">Methods</span></span>

| <span data-ttu-id="194d9-106">Methode</span><span class="sxs-lookup"><span data-stu-id="194d9-106">Method</span></span>           | <span data-ttu-id="194d9-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="194d9-107">Return Type</span></span>    |<span data-ttu-id="194d9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="194d9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="194d9-109">ChartSeries abrufen</span><span class="sxs-lookup"><span data-stu-id="194d9-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="194d9-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="194d9-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="194d9-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="194d9-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="194d9-112">ChartPoints erstellen</span><span class="sxs-lookup"><span data-stu-id="194d9-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="194d9-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="194d9-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="194d9-114">Dient zum Erstellen eines neuen ChartPoints durch Veröffentlichen in der Punkteammlung.</span><span class="sxs-lookup"><span data-stu-id="194d9-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="194d9-115">Punkte auflisten</span><span class="sxs-lookup"><span data-stu-id="194d9-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="194d9-116">[ChartPoints-Sammlung](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="194d9-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="194d9-117">Dient zum Abrufen einer ChartPoints-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="194d9-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="194d9-118">Update</span><span class="sxs-lookup"><span data-stu-id="194d9-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="194d9-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="194d9-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="194d9-120">Dient zum Aktualisieren des ChartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="194d9-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="194d9-121">List</span><span class="sxs-lookup"><span data-stu-id="194d9-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="194d9-122">[WorkbookChartSeries](chartseries.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="194d9-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="194d9-123">Dient zum Abrufen der chartSeries-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="194d9-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="194d9-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="194d9-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="194d9-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="194d9-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="194d9-126">Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="194d9-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="194d9-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="194d9-127">Properties</span></span>
| <span data-ttu-id="194d9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="194d9-128">Property</span></span>     | <span data-ttu-id="194d9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="194d9-129">Type</span></span>   |<span data-ttu-id="194d9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="194d9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="194d9-131">name</span><span class="sxs-lookup"><span data-stu-id="194d9-131">name</span></span>|<span data-ttu-id="194d9-132">string</span><span class="sxs-lookup"><span data-stu-id="194d9-132">string</span></span>|<span data-ttu-id="194d9-133">Gibt den Namen einer Datenreihe in einem Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="194d9-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="194d9-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="194d9-134">Relationships</span></span>
| <span data-ttu-id="194d9-135">Beziehung</span><span class="sxs-lookup"><span data-stu-id="194d9-135">Relationship</span></span> | <span data-ttu-id="194d9-136">Typ</span><span class="sxs-lookup"><span data-stu-id="194d9-136">Type</span></span>   |<span data-ttu-id="194d9-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="194d9-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="194d9-138">Format</span><span class="sxs-lookup"><span data-stu-id="194d9-138">format</span></span>|[<span data-ttu-id="194d9-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="194d9-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="194d9-p101">Stellt die Formatierung für eine Diagrammdatenreihe dar, einschließlich Füllung und Linienformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="194d9-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="194d9-142">points</span><span class="sxs-lookup"><span data-stu-id="194d9-142">points</span></span>|<span data-ttu-id="194d9-143">[WorkbookChartPoint](chartpoint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="194d9-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="194d9-p102">Stellt eine Sammlung aller Punkte in der Datenreihe dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="194d9-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="194d9-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="194d9-146">JSON representation</span></span>

<span data-ttu-id="194d9-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="194d9-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->