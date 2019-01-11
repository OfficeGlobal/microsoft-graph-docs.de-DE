---
title: SortField-Ressourcentyp
description: Stellt eine Bedingung in einem Sortiervorgang dar.
localization_priority: Normal
ms.openlocfilehash: fc93f33f7e1c6f366986cd5d1ca82ea186ad44b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894278"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="6ae29-103">SortField-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ae29-103">SortField resource type</span></span>

> <span data-ttu-id="6ae29-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ae29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ae29-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ae29-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ae29-106">Stellt eine Bedingung in einem Sortiervorgang dar.</span><span class="sxs-lookup"><span data-stu-id="6ae29-106">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="6ae29-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ae29-107">Properties</span></span>
| <span data-ttu-id="6ae29-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ae29-108">Property</span></span>     | <span data-ttu-id="6ae29-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6ae29-109">Type</span></span>   |<span data-ttu-id="6ae29-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ae29-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ae29-111">ascending</span><span class="sxs-lookup"><span data-stu-id="6ae29-111">ascending</span></span>|<span data-ttu-id="6ae29-112">boolean</span><span class="sxs-lookup"><span data-stu-id="6ae29-112">boolean</span></span>|<span data-ttu-id="6ae29-113">Stellt dar, ob die Sortierung in aufsteigender Reihenfolge ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="6ae29-113">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="6ae29-114">color</span><span class="sxs-lookup"><span data-stu-id="6ae29-114">color</span></span>|<span data-ttu-id="6ae29-115">string</span><span class="sxs-lookup"><span data-stu-id="6ae29-115">string</span></span>|<span data-ttu-id="6ae29-116">Stellt die Farbe dar, die das Ziel der Bedingung ist, wenn die Sortierung für die Schrift- oder Zellenfarbe gilt.</span><span class="sxs-lookup"><span data-stu-id="6ae29-116">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="6ae29-117">dataOption</span><span class="sxs-lookup"><span data-stu-id="6ae29-117">dataOption</span></span>|<span data-ttu-id="6ae29-118">string</span><span class="sxs-lookup"><span data-stu-id="6ae29-118">string</span></span>|<span data-ttu-id="6ae29-p102">Stellt weitere Sortieroptionen für dieses Feld dar. Die folgenden Werte sind möglich: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="6ae29-p102">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="6ae29-121">Key</span><span class="sxs-lookup"><span data-stu-id="6ae29-121">key</span></span>|<span data-ttu-id="6ae29-122">int</span><span class="sxs-lookup"><span data-stu-id="6ae29-122">int</span></span>|<span data-ttu-id="6ae29-p103">Stellt die Spalte (oder Zeile, je nach Sortierausrichtung) dar, für die die Bedingung gilt. Wird als Offset von der ersten Spalte (oder Zeile) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="6ae29-p103">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="6ae29-125">sortOn</span><span class="sxs-lookup"><span data-stu-id="6ae29-125">sortOn</span></span>|<span data-ttu-id="6ae29-126">string</span><span class="sxs-lookup"><span data-stu-id="6ae29-126">string</span></span>|<span data-ttu-id="6ae29-p104">Stellt den Typ der Sortierung dieser Bedingung dar. Die folgenden Werte sind möglich: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="6ae29-p104">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ae29-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ae29-129">Relationships</span></span>
| <span data-ttu-id="6ae29-130">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6ae29-130">Relationship</span></span> | <span data-ttu-id="6ae29-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6ae29-131">Type</span></span>   |<span data-ttu-id="6ae29-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ae29-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ae29-133">Symbol</span><span class="sxs-lookup"><span data-stu-id="6ae29-133">icon</span></span>|[<span data-ttu-id="6ae29-134">Icon</span><span class="sxs-lookup"><span data-stu-id="6ae29-134">Icon</span></span>](icon.md)|<span data-ttu-id="6ae29-135">Stellt das Symbol dar, das das Ziel der Bedingung ist, wenn die Sortierung für das Symbol der Zelle gilt.</span><span class="sxs-lookup"><span data-stu-id="6ae29-135">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ae29-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ae29-136">JSON representation</span></span>

<span data-ttu-id="6ae29-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ae29-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
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
