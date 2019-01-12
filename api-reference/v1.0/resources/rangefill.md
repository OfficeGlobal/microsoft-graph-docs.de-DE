---
title: RangeFill-Ressourcentyp
description: Stellt den Hintergrund eines Bereichsobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 75aa4bd91ad6f1038fdc42460c6a3c9ab928a09d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911819"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="74b8e-103">RangeFill-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="74b8e-103">RangeFill resource type</span></span>

<span data-ttu-id="74b8e-104">Stellt den Hintergrund eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="74b8e-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="74b8e-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="74b8e-105">Methods</span></span>

| <span data-ttu-id="74b8e-106">Methode</span><span class="sxs-lookup"><span data-stu-id="74b8e-106">Method</span></span>           | <span data-ttu-id="74b8e-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="74b8e-107">Return Type</span></span>    |<span data-ttu-id="74b8e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74b8e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74b8e-109">RangeFill abrufen</span><span class="sxs-lookup"><span data-stu-id="74b8e-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="74b8e-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="74b8e-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="74b8e-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="74b8e-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="74b8e-112">Update</span><span class="sxs-lookup"><span data-stu-id="74b8e-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="74b8e-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="74b8e-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="74b8e-114">Dient zum Aktualisieren des RangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="74b8e-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="74b8e-115">Clear</span><span class="sxs-lookup"><span data-stu-id="74b8e-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="74b8e-116">Keine</span><span class="sxs-lookup"><span data-stu-id="74b8e-116">None</span></span>|<span data-ttu-id="74b8e-117">Setzt den Hintergrund des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="74b8e-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="74b8e-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="74b8e-118">Properties</span></span>
| <span data-ttu-id="74b8e-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74b8e-119">Property</span></span>     | <span data-ttu-id="74b8e-120">Typ</span><span class="sxs-lookup"><span data-stu-id="74b8e-120">Type</span></span>   |<span data-ttu-id="74b8e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74b8e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74b8e-122">color</span><span class="sxs-lookup"><span data-stu-id="74b8e-122">color</span></span>|<span data-ttu-id="74b8e-123">string</span><span class="sxs-lookup"><span data-stu-id="74b8e-123">string</span></span>|<span data-ttu-id="74b8e-124">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.</span><span class="sxs-lookup"><span data-stu-id="74b8e-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="74b8e-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="74b8e-125">Relationships</span></span>
<span data-ttu-id="74b8e-126">Keine</span><span class="sxs-lookup"><span data-stu-id="74b8e-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="74b8e-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="74b8e-127">JSON representation</span></span>

<span data-ttu-id="74b8e-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="74b8e-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
