---
title: Icon-Ressourcentyp
description: Stellt ein Zellensymbol dar.
ms.openlocfilehash: fd3e0682a7eb73dd4e3286e11d9f9680755db265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060170"
---
# <a name="icon-resource-type"></a><span data-ttu-id="fec9a-103">Icon-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fec9a-103">Icon resource type</span></span>

> <span data-ttu-id="fec9a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fec9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fec9a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fec9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fec9a-106">Stellt ein Zellensymbol dar.</span><span class="sxs-lookup"><span data-stu-id="fec9a-106">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="fec9a-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="fec9a-107">Methods</span></span>

| <span data-ttu-id="fec9a-108">Methode</span><span class="sxs-lookup"><span data-stu-id="fec9a-108">Method</span></span>           | <span data-ttu-id="fec9a-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fec9a-109">Return Type</span></span>    |<span data-ttu-id="fec9a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fec9a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fec9a-111">Symbol abrufen</span><span class="sxs-lookup"><span data-stu-id="fec9a-111">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="fec9a-112">Icon</span><span class="sxs-lookup"><span data-stu-id="fec9a-112">Icon</span></span>](icon.md) |<span data-ttu-id="fec9a-113">Dient zum Lesen der Eigenschaften und der Beziehungen des icon-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fec9a-113">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="fec9a-114">Update</span><span class="sxs-lookup"><span data-stu-id="fec9a-114">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="fec9a-115">Icon</span><span class="sxs-lookup"><span data-stu-id="fec9a-115">Icon</span></span>](icon.md)  |<span data-ttu-id="fec9a-116">Dient zum Aktualisieren des icon-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fec9a-116">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fec9a-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fec9a-117">Properties</span></span>
| <span data-ttu-id="fec9a-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fec9a-118">Property</span></span>     | <span data-ttu-id="fec9a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fec9a-119">Type</span></span>   |<span data-ttu-id="fec9a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fec9a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fec9a-121">Index</span><span class="sxs-lookup"><span data-stu-id="fec9a-121">index</span></span>|<span data-ttu-id="fec9a-122">int</span><span class="sxs-lookup"><span data-stu-id="fec9a-122">int</span></span>|<span data-ttu-id="fec9a-123">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="fec9a-123">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="fec9a-124">set</span><span class="sxs-lookup"><span data-stu-id="fec9a-124">set</span></span>|<span data-ttu-id="fec9a-125">string</span><span class="sxs-lookup"><span data-stu-id="fec9a-125">string</span></span>|<span data-ttu-id="fec9a-p102">Stellt den Satz dar, zu dem das Symbol gehört. Mögliche Werte: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="fec9a-p102">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fec9a-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fec9a-128">Relationships</span></span>
<span data-ttu-id="fec9a-129">Keine</span><span class="sxs-lookup"><span data-stu-id="fec9a-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fec9a-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fec9a-130">JSON representation</span></span>

<span data-ttu-id="fec9a-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fec9a-131">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->