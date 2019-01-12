---
title: RangeFill-Ressourcentyp
description: Stellt den Hintergrund eines Bereichsobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4043122f4c35c3e7f1c6f9d3919687833d35b9b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974343"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="889ed-103">RangeFill-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="889ed-103">RangeFill resource type</span></span>

> <span data-ttu-id="889ed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="889ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="889ed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="889ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="889ed-106">Stellt den Hintergrund eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="889ed-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="889ed-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="889ed-107">Methods</span></span>

| <span data-ttu-id="889ed-108">Methode</span><span class="sxs-lookup"><span data-stu-id="889ed-108">Method</span></span>           | <span data-ttu-id="889ed-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="889ed-109">Return Type</span></span>    |<span data-ttu-id="889ed-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="889ed-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="889ed-111">RangeFill abrufen</span><span class="sxs-lookup"><span data-stu-id="889ed-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="889ed-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="889ed-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="889ed-113">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="889ed-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="889ed-114">Update</span><span class="sxs-lookup"><span data-stu-id="889ed-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="889ed-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="889ed-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="889ed-116">Dient zum Aktualisieren des RangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="889ed-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="889ed-117">Clear</span><span class="sxs-lookup"><span data-stu-id="889ed-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="889ed-118">Keine</span><span class="sxs-lookup"><span data-stu-id="889ed-118">None</span></span>|<span data-ttu-id="889ed-119">Setzt den Hintergrund des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="889ed-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="889ed-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="889ed-120">Properties</span></span>
| <span data-ttu-id="889ed-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="889ed-121">Property</span></span>     | <span data-ttu-id="889ed-122">Typ</span><span class="sxs-lookup"><span data-stu-id="889ed-122">Type</span></span>   |<span data-ttu-id="889ed-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="889ed-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="889ed-124">color</span><span class="sxs-lookup"><span data-stu-id="889ed-124">color</span></span>|<span data-ttu-id="889ed-125">string</span><span class="sxs-lookup"><span data-stu-id="889ed-125">string</span></span>|<span data-ttu-id="889ed-126">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.</span><span class="sxs-lookup"><span data-stu-id="889ed-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="889ed-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="889ed-127">Relationships</span></span>
<span data-ttu-id="889ed-128">Keine</span><span class="sxs-lookup"><span data-stu-id="889ed-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="889ed-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="889ed-129">JSON representation</span></span>

<span data-ttu-id="889ed-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="889ed-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
