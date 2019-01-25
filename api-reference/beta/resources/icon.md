---
title: Icon-Ressourcentyp
description: Stellt ein Zellensymbol dar.
localization_priority: Normal
ms.openlocfilehash: c15ee02d1c6830cbb5246826665d0353b7e999b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516301"
---
# <a name="icon-resource-type"></a><span data-ttu-id="6407b-103">Icon-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6407b-103">Icon resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6407b-104">Stellt ein Zellensymbol dar.</span><span class="sxs-lookup"><span data-stu-id="6407b-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="6407b-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="6407b-105">Methods</span></span>

| <span data-ttu-id="6407b-106">Methode</span><span class="sxs-lookup"><span data-stu-id="6407b-106">Method</span></span>           | <span data-ttu-id="6407b-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6407b-107">Return Type</span></span>    |<span data-ttu-id="6407b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6407b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6407b-109">Symbol abrufen</span><span class="sxs-lookup"><span data-stu-id="6407b-109">[Get Icon](../api/icon-get.md)</span></span> | [<span data-ttu-id="6407b-110">Icon</span><span class="sxs-lookup"><span data-stu-id="6407b-110">Icon</span></span>](icon.md) |<span data-ttu-id="6407b-111">Dient zum Lesen der Eigenschaften und der Beziehungen des icon-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6407b-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="6407b-112">Update</span><span class="sxs-lookup"><span data-stu-id="6407b-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="6407b-113">Icon</span><span class="sxs-lookup"><span data-stu-id="6407b-113">Icon</span></span>](icon.md)  |<span data-ttu-id="6407b-114">Dient zum Aktualisieren des icon-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6407b-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6407b-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6407b-115">Properties</span></span>
| <span data-ttu-id="6407b-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6407b-116">Property</span></span>     | <span data-ttu-id="6407b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="6407b-117">Type</span></span>   |<span data-ttu-id="6407b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6407b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6407b-119">Index</span><span class="sxs-lookup"><span data-stu-id="6407b-119">index</span></span>|<span data-ttu-id="6407b-120">int</span><span class="sxs-lookup"><span data-stu-id="6407b-120">int</span></span>|<span data-ttu-id="6407b-121">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="6407b-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="6407b-122">set</span><span class="sxs-lookup"><span data-stu-id="6407b-122">set</span></span>|<span data-ttu-id="6407b-123">string</span><span class="sxs-lookup"><span data-stu-id="6407b-123">string</span></span>|<span data-ttu-id="6407b-p101">Stellt den Satz dar, zu dem das Symbol gehört. Mögliche Werte: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="6407b-p101">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6407b-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6407b-126">Relationships</span></span>
<span data-ttu-id="6407b-127">Keine</span><span class="sxs-lookup"><span data-stu-id="6407b-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6407b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6407b-128">JSON representation</span></span>

<span data-ttu-id="6407b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6407b-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.icon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/icon.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
