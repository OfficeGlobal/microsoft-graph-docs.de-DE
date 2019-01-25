---
title: SortField-Ressourcentyp
description: Stellt eine Bedingung in einem Sortiervorgang dar.
localization_priority: Normal
ms.openlocfilehash: 52817df89ed130b6984ae3a76da775e0e000dee5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521635"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="2a905-103">SortField-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2a905-103">SortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a905-104">Stellt eine Bedingung in einem Sortiervorgang dar.</span><span class="sxs-lookup"><span data-stu-id="2a905-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="2a905-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a905-105">Properties</span></span>
| <span data-ttu-id="2a905-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a905-106">Property</span></span>     | <span data-ttu-id="2a905-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2a905-107">Type</span></span>   |<span data-ttu-id="2a905-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a905-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a905-109">ascending</span><span class="sxs-lookup"><span data-stu-id="2a905-109">ascending</span></span>|<span data-ttu-id="2a905-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a905-110">boolean</span></span>|<span data-ttu-id="2a905-111">Stellt dar, ob die Sortierung in aufsteigender Reihenfolge ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="2a905-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="2a905-112">color</span><span class="sxs-lookup"><span data-stu-id="2a905-112">color</span></span>|<span data-ttu-id="2a905-113">string</span><span class="sxs-lookup"><span data-stu-id="2a905-113">string</span></span>|<span data-ttu-id="2a905-114">Stellt die Farbe dar, die das Ziel der Bedingung ist, wenn die Sortierung für die Schrift- oder Zellenfarbe gilt.</span><span class="sxs-lookup"><span data-stu-id="2a905-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="2a905-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="2a905-115">dataOption</span></span>|<span data-ttu-id="2a905-116">string</span><span class="sxs-lookup"><span data-stu-id="2a905-116">string</span></span>|<span data-ttu-id="2a905-p101">Stellt weitere Sortieroptionen für dieses Feld dar. Die folgenden Werte sind möglich: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="2a905-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="2a905-119">Key</span><span class="sxs-lookup"><span data-stu-id="2a905-119">key</span></span>|<span data-ttu-id="2a905-120">int</span><span class="sxs-lookup"><span data-stu-id="2a905-120">int</span></span>|<span data-ttu-id="2a905-p102">Stellt die Spalte (oder Zeile, je nach Sortierausrichtung) dar, für die die Bedingung gilt. Wird als Offset von der ersten Spalte (oder Zeile) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="2a905-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="2a905-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="2a905-123">sortOn</span></span>|<span data-ttu-id="2a905-124">string</span><span class="sxs-lookup"><span data-stu-id="2a905-124">string</span></span>|<span data-ttu-id="2a905-p103">Stellt den Typ der Sortierung dieser Bedingung dar. Die folgenden Werte sind möglich: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="2a905-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a905-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2a905-127">Relationships</span></span>
| <span data-ttu-id="2a905-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2a905-128">Relationship</span></span> | <span data-ttu-id="2a905-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2a905-129">Type</span></span>   |<span data-ttu-id="2a905-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a905-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a905-131">Symbol</span><span class="sxs-lookup"><span data-stu-id="2a905-131">icon</span></span>|[<span data-ttu-id="2a905-132">Icon</span><span class="sxs-lookup"><span data-stu-id="2a905-132">Icon</span></span>](icon.md)|<span data-ttu-id="2a905-133">Stellt das Symbol dar, das das Ziel der Bedingung ist, wenn die Sortierung für das Symbol der Zelle gilt.</span><span class="sxs-lookup"><span data-stu-id="2a905-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a905-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a905-134">JSON representation</span></span>

<span data-ttu-id="2a905-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a905-135">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sortfield.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
