---
title: SortField-Ressourcentyp
description: Stellt eine Bedingung in einem Sortiervorgang dar.
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825970"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="693d6-103">SortField-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="693d6-103">SortField resource type</span></span>

<span data-ttu-id="693d6-104">Stellt eine Bedingung in einem Sortiervorgang dar.</span><span class="sxs-lookup"><span data-stu-id="693d6-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="693d6-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="693d6-105">Properties</span></span>
| <span data-ttu-id="693d6-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="693d6-106">Property</span></span>     | <span data-ttu-id="693d6-107">Typ</span><span class="sxs-lookup"><span data-stu-id="693d6-107">Type</span></span>   |<span data-ttu-id="693d6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693d6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="693d6-109">ascending</span><span class="sxs-lookup"><span data-stu-id="693d6-109">ascending</span></span>|<span data-ttu-id="693d6-110">boolean</span><span class="sxs-lookup"><span data-stu-id="693d6-110">boolean</span></span>|<span data-ttu-id="693d6-111">Stellt dar, ob die Sortierung in aufsteigender Reihenfolge ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="693d6-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="693d6-112">color</span><span class="sxs-lookup"><span data-stu-id="693d6-112">color</span></span>|<span data-ttu-id="693d6-113">string</span><span class="sxs-lookup"><span data-stu-id="693d6-113">string</span></span>|<span data-ttu-id="693d6-114">Stellt die Farbe dar, die das Ziel der Bedingung ist, wenn die Sortierung für die Schrift- oder Zellenfarbe gilt.</span><span class="sxs-lookup"><span data-stu-id="693d6-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="693d6-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="693d6-115">dataOption</span></span>|<span data-ttu-id="693d6-116">string</span><span class="sxs-lookup"><span data-stu-id="693d6-116">string</span></span>|<span data-ttu-id="693d6-117">Weitere Sortieroptionen für dieses Feld darstellt.</span><span class="sxs-lookup"><span data-stu-id="693d6-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="693d6-118">Die möglichen Werte sind: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="693d6-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="693d6-119">Key</span><span class="sxs-lookup"><span data-stu-id="693d6-119">key</span></span>|<span data-ttu-id="693d6-120">int</span><span class="sxs-lookup"><span data-stu-id="693d6-120">int</span></span>|<span data-ttu-id="693d6-p102">Stellt die Spalte (oder Zeile, je nach Sortierausrichtung) dar, für die die Bedingung gilt. Wird als Offset von der ersten Spalte (oder Zeile) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="693d6-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="693d6-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="693d6-123">sortOn</span></span>|<span data-ttu-id="693d6-124">string</span><span class="sxs-lookup"><span data-stu-id="693d6-124">string</span></span>|<span data-ttu-id="693d6-125">Stellt den Typ der Sortierung der diese Bedingung.</span><span class="sxs-lookup"><span data-stu-id="693d6-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="693d6-126">Die möglichen Werte sind: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="693d6-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="693d6-127">Symbol</span><span class="sxs-lookup"><span data-stu-id="693d6-127">icon</span></span>|[<span data-ttu-id="693d6-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="693d6-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="693d6-129">Stellt das Symbol dar, das das Ziel der Bedingung ist, wenn die Sortierung für das Symbol der Zelle gilt.</span><span class="sxs-lookup"><span data-stu-id="693d6-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="693d6-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="693d6-130">JSON representation</span></span>

<span data-ttu-id="693d6-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="693d6-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
