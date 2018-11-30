---
title: ChartAxisTitle-Ressourcentyp
description: Stellt den Titel einer Diagrammachse dar.
ms.openlocfilehash: ede660e2ba5d0ab34e8b985574e3077ca06b32b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017410"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="b0b64-103">ChartAxisTitle-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b0b64-103">ChartAxisTitle resource type</span></span>

<span data-ttu-id="b0b64-104">Stellt den Titel einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="b0b64-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="b0b64-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b0b64-105">Methods</span></span>

| <span data-ttu-id="b0b64-106">Methode</span><span class="sxs-lookup"><span data-stu-id="b0b64-106">Method</span></span>           | <span data-ttu-id="b0b64-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b0b64-107">Return Type</span></span>    |<span data-ttu-id="b0b64-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0b64-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0b64-109">ChartAxisTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="b0b64-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="b0b64-110">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="b0b64-110">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="b0b64-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0b64-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="b0b64-112">Update</span><span class="sxs-lookup"><span data-stu-id="b0b64-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="b0b64-113">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="b0b64-113">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="b0b64-114">Dient zum Aktualisieren de chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0b64-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0b64-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b0b64-115">Properties</span></span>
| <span data-ttu-id="b0b64-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0b64-116">Property</span></span>     | <span data-ttu-id="b0b64-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b0b64-117">Type</span></span>   |<span data-ttu-id="b0b64-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0b64-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0b64-119">text</span><span class="sxs-lookup"><span data-stu-id="b0b64-119">text</span></span>|<span data-ttu-id="b0b64-120">string</span><span class="sxs-lookup"><span data-stu-id="b0b64-120">string</span></span>|<span data-ttu-id="b0b64-121">Stellt den Achsentitel dar.</span><span class="sxs-lookup"><span data-stu-id="b0b64-121">Represents the axis title.</span></span>|
|<span data-ttu-id="b0b64-122">visible</span><span class="sxs-lookup"><span data-stu-id="b0b64-122">visible</span></span>|<span data-ttu-id="b0b64-123">boolean</span><span class="sxs-lookup"><span data-stu-id="b0b64-123">boolean</span></span>|<span data-ttu-id="b0b64-124">Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.</span><span class="sxs-lookup"><span data-stu-id="b0b64-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0b64-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b0b64-125">Relationships</span></span>
| <span data-ttu-id="b0b64-126">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b0b64-126">Relationship</span></span> | <span data-ttu-id="b0b64-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b0b64-127">Type</span></span>   |<span data-ttu-id="b0b64-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0b64-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0b64-129">Format</span><span class="sxs-lookup"><span data-stu-id="b0b64-129">format</span></span>|[<span data-ttu-id="b0b64-130">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="b0b64-130">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="b0b64-p101">Stellt die Formatierung des Diagrammachsentitels dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b0b64-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0b64-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b0b64-133">JSON representation</span></span>

<span data-ttu-id="b0b64-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b0b64-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
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