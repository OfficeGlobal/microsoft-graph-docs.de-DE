---
title: ChartPoint-Ressourcentyp
description: Stellt einen Punkt einer Datenreihe in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66c58e08063bd9757ad9c174e81f35328dd2722b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912757"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="7107d-103">ChartPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7107d-103">ChartPoint resource type</span></span>

> <span data-ttu-id="7107d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7107d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7107d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7107d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7107d-106">Stellt einen Punkt einer Datenreihe in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="7107d-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7107d-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="7107d-107">Methods</span></span>

| <span data-ttu-id="7107d-108">Methode</span><span class="sxs-lookup"><span data-stu-id="7107d-108">Method</span></span>           | <span data-ttu-id="7107d-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7107d-109">Return Type</span></span>    |<span data-ttu-id="7107d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7107d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7107d-111">ChartPoint abrufen</span><span class="sxs-lookup"><span data-stu-id="7107d-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="7107d-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="7107d-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="7107d-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7107d-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="7107d-114">List</span><span class="sxs-lookup"><span data-stu-id="7107d-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="7107d-115">[ChartPoint-Sammlung](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="7107d-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="7107d-116">Dient zum Abrufen der ChartPoint-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="7107d-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="7107d-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="7107d-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="7107d-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="7107d-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="7107d-119">Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="7107d-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="7107d-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7107d-120">Properties</span></span>
| <span data-ttu-id="7107d-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7107d-121">Property</span></span>     | <span data-ttu-id="7107d-122">Typ</span><span class="sxs-lookup"><span data-stu-id="7107d-122">Type</span></span>   |<span data-ttu-id="7107d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7107d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7107d-124">Wert</span><span class="sxs-lookup"><span data-stu-id="7107d-124">value</span></span>|<span data-ttu-id="7107d-125">object</span><span class="sxs-lookup"><span data-stu-id="7107d-125">object</span></span>|<span data-ttu-id="7107d-p102">Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7107d-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7107d-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7107d-128">Relationships</span></span>
| <span data-ttu-id="7107d-129">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7107d-129">Relationship</span></span> | <span data-ttu-id="7107d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7107d-130">Type</span></span>   |<span data-ttu-id="7107d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7107d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7107d-132">format</span><span class="sxs-lookup"><span data-stu-id="7107d-132">format</span></span>|[<span data-ttu-id="7107d-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="7107d-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="7107d-p103">Kapselt die Formateigenschaften eines Diagrammpunkts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7107d-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7107d-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7107d-136">JSON representation</span></span>

<span data-ttu-id="7107d-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7107d-137">Here is a JSON representation of the resource.</span></span>

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
