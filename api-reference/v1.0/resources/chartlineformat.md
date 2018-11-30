---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
ms.openlocfilehash: 6e43818bc55972585deff5aa2add1d513f031360
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016845"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="29ab7-103">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="29ab7-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="29ab7-104">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="29ab7-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="29ab7-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="29ab7-105">Methods</span></span>

| <span data-ttu-id="29ab7-106">Methode</span><span class="sxs-lookup"><span data-stu-id="29ab7-106">Method</span></span>           | <span data-ttu-id="29ab7-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="29ab7-107">Return Type</span></span>    |<span data-ttu-id="29ab7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29ab7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29ab7-109">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="29ab7-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="29ab7-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="29ab7-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="29ab7-111">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="29ab7-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="29ab7-112">Update</span><span class="sxs-lookup"><span data-stu-id="29ab7-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="29ab7-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="29ab7-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="29ab7-114">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="29ab7-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="29ab7-115">Löschen</span><span class="sxs-lookup"><span data-stu-id="29ab7-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="29ab7-116">Keine</span><span class="sxs-lookup"><span data-stu-id="29ab7-116">None</span></span>|<span data-ttu-id="29ab7-117">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="29ab7-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="29ab7-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="29ab7-118">Properties</span></span>
| <span data-ttu-id="29ab7-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29ab7-119">Property</span></span>     | <span data-ttu-id="29ab7-120">Typ</span><span class="sxs-lookup"><span data-stu-id="29ab7-120">Type</span></span>   |<span data-ttu-id="29ab7-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29ab7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29ab7-122">color</span><span class="sxs-lookup"><span data-stu-id="29ab7-122">color</span></span>|<span data-ttu-id="29ab7-123">string</span><span class="sxs-lookup"><span data-stu-id="29ab7-123">string</span></span>|<span data-ttu-id="29ab7-124">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="29ab7-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29ab7-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="29ab7-125">Relationships</span></span>
<span data-ttu-id="29ab7-126">Keine</span><span class="sxs-lookup"><span data-stu-id="29ab7-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="29ab7-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="29ab7-127">JSON representation</span></span>

<span data-ttu-id="29ab7-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="29ab7-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
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