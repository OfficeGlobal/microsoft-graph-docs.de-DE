---
title: ChartPoint-Ressourcentyp
description: Stellt einen Punkt einer Datenreihe in einem Diagramm dar.
ms.openlocfilehash: 93c89bca61f27924621df0376bdf50e925e25c86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019351"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="f71f2-103">ChartPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f71f2-103">ChartPoint resource type</span></span>

<span data-ttu-id="f71f2-104">Stellt einen Punkt einer Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="f71f2-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f71f2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="f71f2-105">Methods</span></span>

| <span data-ttu-id="f71f2-106">Methode</span><span class="sxs-lookup"><span data-stu-id="f71f2-106">Method</span></span>           | <span data-ttu-id="f71f2-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f71f2-107">Return Type</span></span>    |<span data-ttu-id="f71f2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f71f2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f71f2-109">ChartPoint abrufen</span><span class="sxs-lookup"><span data-stu-id="f71f2-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="f71f2-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="f71f2-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="f71f2-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f71f2-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="f71f2-112">List</span><span class="sxs-lookup"><span data-stu-id="f71f2-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="f71f2-113">[WorkbookChartPoint](chartpoint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f71f2-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="f71f2-114">Dient zum Abrufen der ChartPoint-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="f71f2-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="f71f2-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="f71f2-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="f71f2-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="f71f2-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="f71f2-117">Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="f71f2-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="f71f2-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f71f2-118">Properties</span></span>
| <span data-ttu-id="f71f2-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f71f2-119">Property</span></span>     | <span data-ttu-id="f71f2-120">Typ</span><span class="sxs-lookup"><span data-stu-id="f71f2-120">Type</span></span>   |<span data-ttu-id="f71f2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f71f2-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f71f2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f71f2-122">value</span></span>|<span data-ttu-id="f71f2-123">Json</span><span class="sxs-lookup"><span data-stu-id="f71f2-123">Json</span></span>|<span data-ttu-id="f71f2-p101">Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f71f2-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="f71f2-126">id</span><span class="sxs-lookup"><span data-stu-id="f71f2-126">id</span></span>|<span data-ttu-id="f71f2-127">string</span><span class="sxs-lookup"><span data-stu-id="f71f2-127">string</span></span>|<span data-ttu-id="f71f2-128">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="f71f2-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="f71f2-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f71f2-129">Relationships</span></span>
| <span data-ttu-id="f71f2-130">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f71f2-130">Relationship</span></span> | <span data-ttu-id="f71f2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f71f2-131">Type</span></span>   |<span data-ttu-id="f71f2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f71f2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f71f2-133">Format</span><span class="sxs-lookup"><span data-stu-id="f71f2-133">format</span></span>|[<span data-ttu-id="f71f2-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="f71f2-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="f71f2-p102">Kapselt die Formateigenschaften eines Diagrammpunkts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f71f2-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f71f2-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f71f2-137">JSON representation</span></span>

<span data-ttu-id="f71f2-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f71f2-138">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->