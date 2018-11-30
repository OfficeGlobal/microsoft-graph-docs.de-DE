---
title: ChartSeries-Ressourcentyp
description: Stellt eine Datenreihe in einem Diagramm dar.
ms.openlocfilehash: 301fd3ba3c299108836bbd92497f4d6f6af94b0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066050"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="19421-103">ChartSeries-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="19421-103">ChartSeries resource type</span></span>

> <span data-ttu-id="19421-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19421-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19421-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19421-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19421-106">Stellt eine Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="19421-106">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="19421-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="19421-107">Methods</span></span>

| <span data-ttu-id="19421-108">Methode</span><span class="sxs-lookup"><span data-stu-id="19421-108">Method</span></span>           | <span data-ttu-id="19421-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="19421-109">Return Type</span></span>    |<span data-ttu-id="19421-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19421-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19421-111">ChartSeries abrufen</span><span class="sxs-lookup"><span data-stu-id="19421-111">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="19421-112">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="19421-112">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="19421-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="19421-113">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="19421-114">ChartPoints erstellen</span><span class="sxs-lookup"><span data-stu-id="19421-114">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="19421-115">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="19421-115">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="19421-116">Dient zum Erstellen eines neuen ChartPoints durch Veröffentlichen in der Punkteammlung.</span><span class="sxs-lookup"><span data-stu-id="19421-116">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="19421-117">Punkte auflisten</span><span class="sxs-lookup"><span data-stu-id="19421-117">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="19421-118">[ChartPoints-Sammlung](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="19421-118">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="19421-119">Dient zum Abrufen einer ChartPoints-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="19421-119">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="19421-120">Update</span><span class="sxs-lookup"><span data-stu-id="19421-120">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="19421-121">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="19421-121">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="19421-122">Dient zum Aktualisieren des ChartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="19421-122">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="19421-123">List</span><span class="sxs-lookup"><span data-stu-id="19421-123">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="19421-124">[ChartSeries-Sammlung](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="19421-124">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="19421-125">Dient zum Abrufen der chartSeries-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="19421-125">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="19421-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="19421-126">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="19421-127">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="19421-127">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="19421-128">Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="19421-128">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="19421-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="19421-129">Properties</span></span>
| <span data-ttu-id="19421-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19421-130">Property</span></span>     | <span data-ttu-id="19421-131">Typ</span><span class="sxs-lookup"><span data-stu-id="19421-131">Type</span></span>   |<span data-ttu-id="19421-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19421-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19421-133">name</span><span class="sxs-lookup"><span data-stu-id="19421-133">name</span></span>|<span data-ttu-id="19421-134">string</span><span class="sxs-lookup"><span data-stu-id="19421-134">string</span></span>|<span data-ttu-id="19421-135">Gibt den Namen einer Datenreihe in einem Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="19421-135">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19421-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="19421-136">Relationships</span></span>
| <span data-ttu-id="19421-137">Beziehung</span><span class="sxs-lookup"><span data-stu-id="19421-137">Relationship</span></span> | <span data-ttu-id="19421-138">Typ</span><span class="sxs-lookup"><span data-stu-id="19421-138">Type</span></span>   |<span data-ttu-id="19421-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19421-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19421-140">Format</span><span class="sxs-lookup"><span data-stu-id="19421-140">format</span></span>|[<span data-ttu-id="19421-141">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="19421-141">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="19421-p102">Stellt die Formatierung für eine Diagrammdatenreihe dar, einschließlich Füllung und Linienformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19421-p102">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="19421-144">points</span><span class="sxs-lookup"><span data-stu-id="19421-144">points</span></span>|<span data-ttu-id="19421-145">[ChartPoints-Sammlung](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="19421-145">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="19421-p103">Stellt eine Sammlung aller Punkte in der Datenreihe dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19421-p103">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19421-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="19421-148">JSON representation</span></span>

<span data-ttu-id="19421-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="19421-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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