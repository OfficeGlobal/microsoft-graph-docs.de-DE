---
title: ChartPoint-Ressourcentyp
description: Stellt einen Punkt einer Datenreihe in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e8ede39ef53bfc39574ebfc86c8138a70fc31ad6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573067"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="53429-103">ChartPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="53429-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53429-104">Stellt einen Punkt einer Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="53429-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="53429-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="53429-105">Methods</span></span>

| <span data-ttu-id="53429-106">Methode</span><span class="sxs-lookup"><span data-stu-id="53429-106">Method</span></span>           | <span data-ttu-id="53429-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="53429-107">Return Type</span></span>    |<span data-ttu-id="53429-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53429-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53429-109">ChartPoint abrufen</span><span class="sxs-lookup"><span data-stu-id="53429-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="53429-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="53429-110">workbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="53429-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="53429-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="53429-112">List</span><span class="sxs-lookup"><span data-stu-id="53429-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="53429-113">[WorkbookChartPoint](chartpoint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="53429-113">[workbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="53429-114">Dient zum Abrufen der ChartPoint-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="53429-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="53429-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="53429-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="53429-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="53429-116">workbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="53429-117">Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="53429-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="53429-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="53429-118">Properties</span></span>
| <span data-ttu-id="53429-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53429-119">Property</span></span>     | <span data-ttu-id="53429-120">Typ</span><span class="sxs-lookup"><span data-stu-id="53429-120">Type</span></span>   |<span data-ttu-id="53429-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53429-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53429-122">Wert</span><span class="sxs-lookup"><span data-stu-id="53429-122">value</span></span>|<span data-ttu-id="53429-123">Json</span><span class="sxs-lookup"><span data-stu-id="53429-123">Json</span></span>|<span data-ttu-id="53429-p101">Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="53429-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="53429-126">id</span><span class="sxs-lookup"><span data-stu-id="53429-126">id</span></span>|<span data-ttu-id="53429-127">string</span><span class="sxs-lookup"><span data-stu-id="53429-127">string</span></span>|<span data-ttu-id="53429-128">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="53429-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="53429-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="53429-129">Relationships</span></span>
| <span data-ttu-id="53429-130">Beziehung</span><span class="sxs-lookup"><span data-stu-id="53429-130">Relationship</span></span> | <span data-ttu-id="53429-131">Typ</span><span class="sxs-lookup"><span data-stu-id="53429-131">Type</span></span>   |<span data-ttu-id="53429-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53429-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53429-133">format</span><span class="sxs-lookup"><span data-stu-id="53429-133">format</span></span>|[<span data-ttu-id="53429-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="53429-134">workbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="53429-p102">Kapselt die Formateigenschaften eines Diagrammpunkts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="53429-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53429-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="53429-137">JSON representation</span></span>

<span data-ttu-id="53429-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="53429-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
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
