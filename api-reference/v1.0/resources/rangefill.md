---
title: RangeFill-Ressourcentyp
description: Stellt den Hintergrund eines Bereichsobjekts dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d1dc1bda19d725999f9a49644bee1e4cb1126ec2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877189"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="02fad-103">RangeFill-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="02fad-103">RangeFill resource type</span></span>

<span data-ttu-id="02fad-104">Stellt den Hintergrund eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="02fad-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="02fad-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="02fad-105">Methods</span></span>

| <span data-ttu-id="02fad-106">Methode</span><span class="sxs-lookup"><span data-stu-id="02fad-106">Method</span></span>           | <span data-ttu-id="02fad-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="02fad-107">Return Type</span></span>    |<span data-ttu-id="02fad-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02fad-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02fad-109">RangeFill abrufen</span><span class="sxs-lookup"><span data-stu-id="02fad-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="02fad-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="02fad-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="02fad-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="02fad-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="02fad-112">Update</span><span class="sxs-lookup"><span data-stu-id="02fad-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="02fad-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="02fad-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="02fad-114">Dient zum Aktualisieren des RangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="02fad-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="02fad-115">Clear</span><span class="sxs-lookup"><span data-stu-id="02fad-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="02fad-116">Keine</span><span class="sxs-lookup"><span data-stu-id="02fad-116">None</span></span>|<span data-ttu-id="02fad-117">Setzt den Hintergrund des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="02fad-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="02fad-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02fad-118">Properties</span></span>
| <span data-ttu-id="02fad-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02fad-119">Property</span></span>     | <span data-ttu-id="02fad-120">Typ</span><span class="sxs-lookup"><span data-stu-id="02fad-120">Type</span></span>   |<span data-ttu-id="02fad-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02fad-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02fad-122">color</span><span class="sxs-lookup"><span data-stu-id="02fad-122">color</span></span>|<span data-ttu-id="02fad-123">string</span><span class="sxs-lookup"><span data-stu-id="02fad-123">string</span></span>|<span data-ttu-id="02fad-124">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.</span><span class="sxs-lookup"><span data-stu-id="02fad-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="02fad-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="02fad-125">Relationships</span></span>
<span data-ttu-id="02fad-126">Keine</span><span class="sxs-lookup"><span data-stu-id="02fad-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="02fad-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02fad-127">JSON representation</span></span>

<span data-ttu-id="02fad-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02fad-128">Here is a JSON representation of the resource.</span></span>

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
