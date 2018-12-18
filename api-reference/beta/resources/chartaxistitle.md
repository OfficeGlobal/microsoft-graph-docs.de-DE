---
title: ChartAxisTitle-Ressourcentyp
description: Stellt den Titel einer Diagrammachse dar.
author: lumine2008
ms.openlocfilehash: f787e4572c0b0f499740e2ba1e790fec1ce7ba61
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357295"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="d797e-103">ChartAxisTitle-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d797e-103">ChartAxisTitle resource type</span></span>

> <span data-ttu-id="d797e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d797e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d797e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d797e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d797e-106">Stellt den Titel einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="d797e-106">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="d797e-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="d797e-107">Methods</span></span>

| <span data-ttu-id="d797e-108">Methode</span><span class="sxs-lookup"><span data-stu-id="d797e-108">Method</span></span>           | <span data-ttu-id="d797e-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d797e-109">Return Type</span></span>    |<span data-ttu-id="d797e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d797e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d797e-111">ChartAxisTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="d797e-111">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="d797e-112">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="d797e-112">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="d797e-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d797e-113">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="d797e-114">Update</span><span class="sxs-lookup"><span data-stu-id="d797e-114">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="d797e-115">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="d797e-115">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="d797e-116">Dient zum Aktualisieren de chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d797e-116">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d797e-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d797e-117">Properties</span></span>
| <span data-ttu-id="d797e-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d797e-118">Property</span></span>     | <span data-ttu-id="d797e-119">Typ</span><span class="sxs-lookup"><span data-stu-id="d797e-119">Type</span></span>   |<span data-ttu-id="d797e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d797e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d797e-121">text</span><span class="sxs-lookup"><span data-stu-id="d797e-121">text</span></span>|<span data-ttu-id="d797e-122">string</span><span class="sxs-lookup"><span data-stu-id="d797e-122">string</span></span>|<span data-ttu-id="d797e-123">Stellt den Achsentitel dar.</span><span class="sxs-lookup"><span data-stu-id="d797e-123">Represents the axis title.</span></span>|
|<span data-ttu-id="d797e-124">visible</span><span class="sxs-lookup"><span data-stu-id="d797e-124">visible</span></span>|<span data-ttu-id="d797e-125">boolean</span><span class="sxs-lookup"><span data-stu-id="d797e-125">boolean</span></span>|<span data-ttu-id="d797e-126">Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.</span><span class="sxs-lookup"><span data-stu-id="d797e-126">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d797e-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d797e-127">Relationships</span></span>
| <span data-ttu-id="d797e-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d797e-128">Relationship</span></span> | <span data-ttu-id="d797e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d797e-129">Type</span></span>   |<span data-ttu-id="d797e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d797e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d797e-131">Format</span><span class="sxs-lookup"><span data-stu-id="d797e-131">format</span></span>|[<span data-ttu-id="d797e-132">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="d797e-132">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="d797e-p102">Stellt die Formatierung des Diagrammachsentitels dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d797e-p102">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d797e-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d797e-135">JSON representation</span></span>

<span data-ttu-id="d797e-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d797e-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->