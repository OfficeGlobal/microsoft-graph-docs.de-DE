---
title: ChartTitle-Ressourcentyp
description: Ein Diagrammtitelobjekt eines Diagramms.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f6c843e24839b51da67bda5ed3484a32c868ae54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986915"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="edce8-103">ChartTitle-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="edce8-103">ChartTitle resource type</span></span>

<span data-ttu-id="edce8-104">Ein Diagrammtitelobjekt eines Diagramms.</span><span class="sxs-lookup"><span data-stu-id="edce8-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="edce8-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="edce8-105">Methods</span></span>

| <span data-ttu-id="edce8-106">Methode</span><span class="sxs-lookup"><span data-stu-id="edce8-106">Method</span></span>           | <span data-ttu-id="edce8-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="edce8-107">Return Type</span></span>    |<span data-ttu-id="edce8-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edce8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="edce8-109">ChartTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="edce8-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="edce8-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="edce8-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="edce8-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="edce8-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="edce8-112">Update</span><span class="sxs-lookup"><span data-stu-id="edce8-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="edce8-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="edce8-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="edce8-114">Dient zum Aktualisieren des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="edce8-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="edce8-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="edce8-115">Properties</span></span>
| <span data-ttu-id="edce8-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="edce8-116">Property</span></span>     | <span data-ttu-id="edce8-117">Typ</span><span class="sxs-lookup"><span data-stu-id="edce8-117">Type</span></span>   |<span data-ttu-id="edce8-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edce8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edce8-119">Overlay</span><span class="sxs-lookup"><span data-stu-id="edce8-119">overlay</span></span>|<span data-ttu-id="edce8-120">boolean</span><span class="sxs-lookup"><span data-stu-id="edce8-120">boolean</span></span>|<span data-ttu-id="edce8-121">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="edce8-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="edce8-122">text</span><span class="sxs-lookup"><span data-stu-id="edce8-122">text</span></span>|<span data-ttu-id="edce8-123">string</span><span class="sxs-lookup"><span data-stu-id="edce8-123">string</span></span>|<span data-ttu-id="edce8-124">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="edce8-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="edce8-125">visible</span><span class="sxs-lookup"><span data-stu-id="edce8-125">visible</span></span>|<span data-ttu-id="edce8-126">boolean</span><span class="sxs-lookup"><span data-stu-id="edce8-126">boolean</span></span>|<span data-ttu-id="edce8-127">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="edce8-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edce8-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="edce8-128">Relationships</span></span>
| <span data-ttu-id="edce8-129">Beziehung</span><span class="sxs-lookup"><span data-stu-id="edce8-129">Relationship</span></span> | <span data-ttu-id="edce8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="edce8-130">Type</span></span>   |<span data-ttu-id="edce8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edce8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edce8-132">format</span><span class="sxs-lookup"><span data-stu-id="edce8-132">format</span></span>|[<span data-ttu-id="edce8-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="edce8-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="edce8-p101">Stellt die Formatierung für einen Diagrammtitel dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="edce8-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edce8-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="edce8-136">JSON representation</span></span>

<span data-ttu-id="edce8-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="edce8-137">Here is a JSON representation of the resource.</span></span>

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
