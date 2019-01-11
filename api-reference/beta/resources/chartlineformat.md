---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b2b7e8bd5c0b489ed42baaa3939f7a839c74c3e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871134"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="78e90-103">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="78e90-103">ChartLineFormat resource type</span></span>

> <span data-ttu-id="78e90-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78e90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78e90-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78e90-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78e90-106">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="78e90-106">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="78e90-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="78e90-107">Methods</span></span>

| <span data-ttu-id="78e90-108">Methode</span><span class="sxs-lookup"><span data-stu-id="78e90-108">Method</span></span>           | <span data-ttu-id="78e90-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="78e90-109">Return Type</span></span>    |<span data-ttu-id="78e90-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78e90-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78e90-111">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="78e90-111">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="78e90-112">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="78e90-112">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="78e90-113">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="78e90-113">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="78e90-114">Update</span><span class="sxs-lookup"><span data-stu-id="78e90-114">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="78e90-115">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="78e90-115">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="78e90-116">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="78e90-116">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="78e90-117">Clear</span><span class="sxs-lookup"><span data-stu-id="78e90-117">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="78e90-118">Keine</span><span class="sxs-lookup"><span data-stu-id="78e90-118">None</span></span>|<span data-ttu-id="78e90-119">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="78e90-119">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="78e90-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78e90-120">Properties</span></span>
| <span data-ttu-id="78e90-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78e90-121">Property</span></span>     | <span data-ttu-id="78e90-122">Typ</span><span class="sxs-lookup"><span data-stu-id="78e90-122">Type</span></span>   |<span data-ttu-id="78e90-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78e90-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78e90-124">color</span><span class="sxs-lookup"><span data-stu-id="78e90-124">color</span></span>|<span data-ttu-id="78e90-125">string</span><span class="sxs-lookup"><span data-stu-id="78e90-125">string</span></span>|<span data-ttu-id="78e90-126">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="78e90-126">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78e90-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78e90-127">Relationships</span></span>
<span data-ttu-id="78e90-128">Keine</span><span class="sxs-lookup"><span data-stu-id="78e90-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="78e90-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78e90-129">JSON representation</span></span>

<span data-ttu-id="78e90-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78e90-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
