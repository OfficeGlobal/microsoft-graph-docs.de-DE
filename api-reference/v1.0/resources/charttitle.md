---
title: ChartTitle-Ressourcentyp
description: Ein Diagrammtitelobjekt eines Diagramms.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6cf6a2e6355fc4bc8955899dde48f9cc843e920c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879415"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="41256-103">ChartTitle-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="41256-103">ChartTitle resource type</span></span>

<span data-ttu-id="41256-104">Ein Diagrammtitelobjekt eines Diagramms.</span><span class="sxs-lookup"><span data-stu-id="41256-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="41256-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="41256-105">Methods</span></span>

| <span data-ttu-id="41256-106">Methode</span><span class="sxs-lookup"><span data-stu-id="41256-106">Method</span></span>           | <span data-ttu-id="41256-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="41256-107">Return Type</span></span>    |<span data-ttu-id="41256-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41256-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41256-109">ChartTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="41256-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="41256-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="41256-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="41256-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41256-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="41256-112">Update</span><span class="sxs-lookup"><span data-stu-id="41256-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="41256-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="41256-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="41256-114">Dient zum Aktualisieren des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41256-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="41256-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41256-115">Properties</span></span>
| <span data-ttu-id="41256-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41256-116">Property</span></span>     | <span data-ttu-id="41256-117">Typ</span><span class="sxs-lookup"><span data-stu-id="41256-117">Type</span></span>   |<span data-ttu-id="41256-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41256-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41256-119">Overlay</span><span class="sxs-lookup"><span data-stu-id="41256-119">overlay</span></span>|<span data-ttu-id="41256-120">boolean</span><span class="sxs-lookup"><span data-stu-id="41256-120">boolean</span></span>|<span data-ttu-id="41256-121">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="41256-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="41256-122">text</span><span class="sxs-lookup"><span data-stu-id="41256-122">text</span></span>|<span data-ttu-id="41256-123">string</span><span class="sxs-lookup"><span data-stu-id="41256-123">string</span></span>|<span data-ttu-id="41256-124">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="41256-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="41256-125">visible</span><span class="sxs-lookup"><span data-stu-id="41256-125">visible</span></span>|<span data-ttu-id="41256-126">boolean</span><span class="sxs-lookup"><span data-stu-id="41256-126">boolean</span></span>|<span data-ttu-id="41256-127">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="41256-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41256-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="41256-128">Relationships</span></span>
| <span data-ttu-id="41256-129">Beziehung</span><span class="sxs-lookup"><span data-stu-id="41256-129">Relationship</span></span> | <span data-ttu-id="41256-130">Typ</span><span class="sxs-lookup"><span data-stu-id="41256-130">Type</span></span>   |<span data-ttu-id="41256-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41256-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41256-132">format</span><span class="sxs-lookup"><span data-stu-id="41256-132">format</span></span>|[<span data-ttu-id="41256-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="41256-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="41256-p101">Stellt die Formatierung für einen Diagrammtitel dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="41256-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41256-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41256-136">JSON representation</span></span>

<span data-ttu-id="41256-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41256-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
