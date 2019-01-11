---
title: ChartAxisTitle-Ressourcentyp
description: Stellt den Titel einer Diagrammachse dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a78219e5833f7f85cde571dc984959b642ebe4d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894180"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="ae803-103">ChartAxisTitle-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae803-103">ChartAxisTitle resource type</span></span>

> <span data-ttu-id="ae803-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ae803-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae803-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae803-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae803-106">Stellt den Titel einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="ae803-106">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="ae803-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="ae803-107">Methods</span></span>

| <span data-ttu-id="ae803-108">Methode</span><span class="sxs-lookup"><span data-stu-id="ae803-108">Method</span></span>           | <span data-ttu-id="ae803-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ae803-109">Return Type</span></span>    |<span data-ttu-id="ae803-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae803-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae803-111">ChartAxisTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="ae803-111">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="ae803-112">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="ae803-112">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="ae803-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae803-113">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="ae803-114">Update</span><span class="sxs-lookup"><span data-stu-id="ae803-114">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="ae803-115">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="ae803-115">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="ae803-116">Dient zum Aktualisieren de chartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae803-116">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae803-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae803-117">Properties</span></span>
| <span data-ttu-id="ae803-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae803-118">Property</span></span>     | <span data-ttu-id="ae803-119">Typ</span><span class="sxs-lookup"><span data-stu-id="ae803-119">Type</span></span>   |<span data-ttu-id="ae803-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae803-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae803-121">text</span><span class="sxs-lookup"><span data-stu-id="ae803-121">text</span></span>|<span data-ttu-id="ae803-122">string</span><span class="sxs-lookup"><span data-stu-id="ae803-122">string</span></span>|<span data-ttu-id="ae803-123">Stellt den Achsentitel dar.</span><span class="sxs-lookup"><span data-stu-id="ae803-123">Represents the axis title.</span></span>|
|<span data-ttu-id="ae803-124">visible</span><span class="sxs-lookup"><span data-stu-id="ae803-124">visible</span></span>|<span data-ttu-id="ae803-125">boolean</span><span class="sxs-lookup"><span data-stu-id="ae803-125">boolean</span></span>|<span data-ttu-id="ae803-126">Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.</span><span class="sxs-lookup"><span data-stu-id="ae803-126">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae803-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae803-127">Relationships</span></span>
| <span data-ttu-id="ae803-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ae803-128">Relationship</span></span> | <span data-ttu-id="ae803-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ae803-129">Type</span></span>   |<span data-ttu-id="ae803-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae803-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae803-131">format</span><span class="sxs-lookup"><span data-stu-id="ae803-131">format</span></span>|[<span data-ttu-id="ae803-132">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="ae803-132">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="ae803-p102">Stellt die Formatierung des Diagrammachsentitels dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ae803-p102">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae803-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae803-135">JSON representation</span></span>

<span data-ttu-id="ae803-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae803-136">Here is a JSON representation of the resource.</span></span>

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
