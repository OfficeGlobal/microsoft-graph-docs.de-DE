---
title: ChartSeries-Ressourcentyp
description: Stellt eine Datenreihe in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a3a19793629a5e100830565e224541930e2180de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834895"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="d4809-103">ChartSeries-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4809-103">ChartSeries resource type</span></span>

<span data-ttu-id="d4809-104">Stellt eine Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="d4809-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="d4809-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d4809-105">Methods</span></span>

| <span data-ttu-id="d4809-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d4809-106">Method</span></span>           | <span data-ttu-id="d4809-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d4809-107">Return Type</span></span>    |<span data-ttu-id="d4809-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4809-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4809-109">ChartSeries abrufen</span><span class="sxs-lookup"><span data-stu-id="d4809-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="d4809-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="d4809-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="d4809-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4809-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="d4809-112">ChartPoints erstellen</span><span class="sxs-lookup"><span data-stu-id="d4809-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="d4809-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="d4809-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="d4809-114">Dient zum Erstellen eines neuen ChartPoints durch Veröffentlichen in der Punkteammlung.</span><span class="sxs-lookup"><span data-stu-id="d4809-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="d4809-115">Punkte auflisten</span><span class="sxs-lookup"><span data-stu-id="d4809-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="d4809-116">[ChartPoints-Sammlung](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="d4809-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="d4809-117">Dient zum Abrufen einer ChartPoints-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="d4809-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="d4809-118">Update</span><span class="sxs-lookup"><span data-stu-id="d4809-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="d4809-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="d4809-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="d4809-120">Dient zum Aktualisieren des ChartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4809-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="d4809-121">List</span><span class="sxs-lookup"><span data-stu-id="d4809-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="d4809-122">[WorkbookChartSeries](chartseries.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4809-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="d4809-123">Dient zum Abrufen der chartSeries-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="d4809-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="d4809-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="d4809-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="d4809-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="d4809-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="d4809-126">Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="d4809-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="d4809-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4809-127">Properties</span></span>
| <span data-ttu-id="d4809-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4809-128">Property</span></span>     | <span data-ttu-id="d4809-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d4809-129">Type</span></span>   |<span data-ttu-id="d4809-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4809-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4809-131">name</span><span class="sxs-lookup"><span data-stu-id="d4809-131">name</span></span>|<span data-ttu-id="d4809-132">string</span><span class="sxs-lookup"><span data-stu-id="d4809-132">string</span></span>|<span data-ttu-id="d4809-133">Gibt den Namen einer Datenreihe in einem Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="d4809-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4809-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4809-134">Relationships</span></span>
| <span data-ttu-id="d4809-135">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d4809-135">Relationship</span></span> | <span data-ttu-id="d4809-136">Typ</span><span class="sxs-lookup"><span data-stu-id="d4809-136">Type</span></span>   |<span data-ttu-id="d4809-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4809-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4809-138">format</span><span class="sxs-lookup"><span data-stu-id="d4809-138">format</span></span>|[<span data-ttu-id="d4809-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="d4809-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="d4809-p101">Stellt die Formatierung für eine Diagrammdatenreihe dar, einschließlich Füllung und Linienformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4809-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="d4809-142">points</span><span class="sxs-lookup"><span data-stu-id="d4809-142">points</span></span>|<span data-ttu-id="d4809-143">[WorkbookChartPoint](chartpoint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4809-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="d4809-p102">Stellt eine Sammlung aller Punkte in der Datenreihe dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4809-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4809-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4809-146">JSON representation</span></span>

<span data-ttu-id="d4809-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4809-147">Here is a JSON representation of the resource.</span></span>

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
