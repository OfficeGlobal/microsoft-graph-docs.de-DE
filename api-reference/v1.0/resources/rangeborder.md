---
title: RangeBorder-Ressourcentyp
description: Stellt den Rahmen eines Objekts dar.
ms.openlocfilehash: 30d5548ba867dc652c700985d65a6db01ce8bc99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017052"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="30fc5-103">RangeBorder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="30fc5-103">RangeBorder resource type</span></span>

<span data-ttu-id="30fc5-104">Stellt den Rahmen eines Objekts dar.</span><span class="sxs-lookup"><span data-stu-id="30fc5-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="30fc5-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="30fc5-105">Methods</span></span>

| <span data-ttu-id="30fc5-106">Methode</span><span class="sxs-lookup"><span data-stu-id="30fc5-106">Method</span></span>           | <span data-ttu-id="30fc5-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="30fc5-107">Return Type</span></span>    |<span data-ttu-id="30fc5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30fc5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30fc5-109">RangeBorder abrufen</span><span class="sxs-lookup"><span data-stu-id="30fc5-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="30fc5-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="30fc5-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="30fc5-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeBorder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="30fc5-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="30fc5-112">Update</span><span class="sxs-lookup"><span data-stu-id="30fc5-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="30fc5-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="30fc5-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="30fc5-114">Dient zum Aktualisieren des RangeBorder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="30fc5-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="30fc5-115">List</span><span class="sxs-lookup"><span data-stu-id="30fc5-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="30fc5-116">[WorkbookRangeBorder](rangeborder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="30fc5-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="30fc5-117">Dient zum Abrufen der RangeBorder-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="30fc5-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="30fc5-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="30fc5-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="30fc5-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="30fc5-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="30fc5-120">Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.</span><span class="sxs-lookup"><span data-stu-id="30fc5-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="30fc5-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30fc5-121">Properties</span></span>
| <span data-ttu-id="30fc5-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30fc5-122">Property</span></span>     | <span data-ttu-id="30fc5-123">Typ</span><span class="sxs-lookup"><span data-stu-id="30fc5-123">Type</span></span>   |<span data-ttu-id="30fc5-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30fc5-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30fc5-125">color</span><span class="sxs-lookup"><span data-stu-id="30fc5-125">color</span></span>|<span data-ttu-id="30fc5-126">string</span><span class="sxs-lookup"><span data-stu-id="30fc5-126">string</span></span>|<span data-ttu-id="30fc5-127">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="30fc5-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="30fc5-128">id</span><span class="sxs-lookup"><span data-stu-id="30fc5-128">id</span></span>|<span data-ttu-id="30fc5-129">string</span><span class="sxs-lookup"><span data-stu-id="30fc5-129">string</span></span>|<span data-ttu-id="30fc5-130">Stellt Rahmen Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="30fc5-130">Represents border identifier.</span></span> <span data-ttu-id="30fc5-131">Die möglichen Werte sind: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="30fc5-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="30fc5-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30fc5-132">Read-only.</span></span>|
|<span data-ttu-id="30fc5-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="30fc5-133">sideIndex</span></span>|<span data-ttu-id="30fc5-134">string</span><span class="sxs-lookup"><span data-stu-id="30fc5-134">string</span></span>|<span data-ttu-id="30fc5-135">Konstanter Wert, der angibt, die bestimmte Seiten des Rahmens.</span><span class="sxs-lookup"><span data-stu-id="30fc5-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="30fc5-136">Die möglichen Werte sind: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="30fc5-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="30fc5-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30fc5-137">Read-only.</span></span>|
|<span data-ttu-id="30fc5-138">style</span><span class="sxs-lookup"><span data-stu-id="30fc5-138">style</span></span>|<span data-ttu-id="30fc5-139">string</span><span class="sxs-lookup"><span data-stu-id="30fc5-139">string</span></span>|<span data-ttu-id="30fc5-140">Eine der Konstanten der Linienart die Linienart für den Rahmen angeben.</span><span class="sxs-lookup"><span data-stu-id="30fc5-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="30fc5-141">Die möglichen Werte sind: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="30fc5-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="30fc5-142">weight</span><span class="sxs-lookup"><span data-stu-id="30fc5-142">weight</span></span>|<span data-ttu-id="30fc5-143">string</span><span class="sxs-lookup"><span data-stu-id="30fc5-143">string</span></span>|<span data-ttu-id="30fc5-144">Gibt die Stärke des Rahmens um einen Bereich an.</span><span class="sxs-lookup"><span data-stu-id="30fc5-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="30fc5-145">Die möglichen Werte sind: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="30fc5-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30fc5-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="30fc5-146">Relationships</span></span>
<span data-ttu-id="30fc5-147">Keine</span><span class="sxs-lookup"><span data-stu-id="30fc5-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="30fc5-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30fc5-148">JSON representation</span></span>

<span data-ttu-id="30fc5-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="30fc5-149">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->