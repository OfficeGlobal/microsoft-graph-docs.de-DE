---
title: ChartPoint-Ressourcentyp
description: Stellt einen Punkt einer Datenreihe in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fd50e2e0b0f289f719dd6636eab16544e6a80f5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641967"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="31a9d-103">ChartPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="31a9d-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31a9d-104">Stellt einen Punkt einer Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="31a9d-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="31a9d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="31a9d-105">Methods</span></span>

| <span data-ttu-id="31a9d-106">Methode</span><span class="sxs-lookup"><span data-stu-id="31a9d-106">Method</span></span>           | <span data-ttu-id="31a9d-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="31a9d-107">Return Type</span></span>    |<span data-ttu-id="31a9d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31a9d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31a9d-109">ChartPoint abrufen</span><span class="sxs-lookup"><span data-stu-id="31a9d-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="31a9d-110">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="31a9d-110">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="31a9d-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="31a9d-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="31a9d-112">List</span><span class="sxs-lookup"><span data-stu-id="31a9d-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="31a9d-113">[ChartPoint-Sammlung](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="31a9d-113">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="31a9d-114">Dient zum Abrufen der ChartPoint-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="31a9d-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="31a9d-115">Itemat</span><span class="sxs-lookup"><span data-stu-id="31a9d-115">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="31a9d-116">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="31a9d-116">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="31a9d-117">Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="31a9d-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="31a9d-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="31a9d-118">Properties</span></span>
| <span data-ttu-id="31a9d-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31a9d-119">Property</span></span>     | <span data-ttu-id="31a9d-120">Typ</span><span class="sxs-lookup"><span data-stu-id="31a9d-120">Type</span></span>   |<span data-ttu-id="31a9d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31a9d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31a9d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="31a9d-122">value</span></span>|<span data-ttu-id="31a9d-123">object</span><span class="sxs-lookup"><span data-stu-id="31a9d-123">object</span></span>|<span data-ttu-id="31a9d-p101">Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="31a9d-p101">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31a9d-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="31a9d-126">Relationships</span></span>
| <span data-ttu-id="31a9d-127">Beziehung</span><span class="sxs-lookup"><span data-stu-id="31a9d-127">Relationship</span></span> | <span data-ttu-id="31a9d-128">Typ</span><span class="sxs-lookup"><span data-stu-id="31a9d-128">Type</span></span>   |<span data-ttu-id="31a9d-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31a9d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31a9d-130">format</span><span class="sxs-lookup"><span data-stu-id="31a9d-130">format</span></span>|[<span data-ttu-id="31a9d-131">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="31a9d-131">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="31a9d-p102">Kapselt die Formateigenschaften eines Diagrammpunkts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="31a9d-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31a9d-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="31a9d-134">JSON representation</span></span>

<span data-ttu-id="31a9d-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="31a9d-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
