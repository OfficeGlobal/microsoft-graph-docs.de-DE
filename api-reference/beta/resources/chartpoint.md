---
title: ChartPoint-Ressourcentyp
description: Stellt einen Punkt einer Datenreihe in einem Diagramm dar.
author: lumine2008
ms.openlocfilehash: f27017d5e6cc111fa759fc6c9728ed182e7fa624
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358407"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="d6d39-103">ChartPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d6d39-103">ChartPoint resource type</span></span>

> <span data-ttu-id="d6d39-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d6d39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6d39-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6d39-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6d39-106">Stellt einen Punkt einer Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="d6d39-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="d6d39-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="d6d39-107">Methods</span></span>

| <span data-ttu-id="d6d39-108">Methode</span><span class="sxs-lookup"><span data-stu-id="d6d39-108">Method</span></span>           | <span data-ttu-id="d6d39-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d6d39-109">Return Type</span></span>    |<span data-ttu-id="d6d39-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6d39-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d6d39-111">ChartPoint abrufen</span><span class="sxs-lookup"><span data-stu-id="d6d39-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="d6d39-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d6d39-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="d6d39-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6d39-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="d6d39-114">List</span><span class="sxs-lookup"><span data-stu-id="d6d39-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="d6d39-115">[ChartPoint-Sammlung](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="d6d39-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="d6d39-116">Dient zum Abrufen der ChartPoint-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="d6d39-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="d6d39-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="d6d39-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="d6d39-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d6d39-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="d6d39-119">Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="d6d39-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6d39-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d6d39-120">Properties</span></span>
| <span data-ttu-id="d6d39-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6d39-121">Property</span></span>     | <span data-ttu-id="d6d39-122">Typ</span><span class="sxs-lookup"><span data-stu-id="d6d39-122">Type</span></span>   |<span data-ttu-id="d6d39-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6d39-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6d39-124">Wert</span><span class="sxs-lookup"><span data-stu-id="d6d39-124">value</span></span>|<span data-ttu-id="d6d39-125">object</span><span class="sxs-lookup"><span data-stu-id="d6d39-125">object</span></span>|<span data-ttu-id="d6d39-p102">Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d6d39-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6d39-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d6d39-128">Relationships</span></span>
| <span data-ttu-id="d6d39-129">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d6d39-129">Relationship</span></span> | <span data-ttu-id="d6d39-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d6d39-130">Type</span></span>   |<span data-ttu-id="d6d39-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6d39-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6d39-132">Format</span><span class="sxs-lookup"><span data-stu-id="d6d39-132">format</span></span>|[<span data-ttu-id="d6d39-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="d6d39-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="d6d39-p103">Kapselt die Formateigenschaften eines Diagrammpunkts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d6d39-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6d39-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d6d39-136">JSON representation</span></span>

<span data-ttu-id="d6d39-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d6d39-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->