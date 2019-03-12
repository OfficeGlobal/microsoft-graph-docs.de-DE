---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Miniaturansicht
localization_priority: Normal
ms.openlocfilehash: d11f9eead6faf885bee579c634267e038f8a8ee4
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482259"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="966c2-102">Thumbnail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="966c2-102">Thumbnail resource type</span></span>

<span data-ttu-id="966c2-103">Der **thumbnail**-Ressourcentyp stellt eine Miniaturansicht für ein Bild, ein Video, ein Dokument oder ein beliebiges Element dar, das über eine Bitmapdarstellung verfügt.</span><span class="sxs-lookup"><span data-stu-id="966c2-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="966c2-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="966c2-104">JSON representation</span></span>

<span data-ttu-id="966c2-105">Es folgt eine JSON-Darstellung der **thumbnail**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="966c2-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="966c2-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="966c2-106">Properties</span></span>

| <span data-ttu-id="966c2-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="966c2-107">Property</span></span>     | <span data-ttu-id="966c2-108">Typ</span><span class="sxs-lookup"><span data-stu-id="966c2-108">Type</span></span>   | <span data-ttu-id="966c2-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="966c2-109">Description</span></span>
| :----------- | :----- | :----------------------------------------------------
| <span data-ttu-id="966c2-110">height</span><span class="sxs-lookup"><span data-stu-id="966c2-110">height</span></span>       | <span data-ttu-id="966c2-111">Int32</span><span class="sxs-lookup"><span data-stu-id="966c2-111">Int32</span></span>  | <span data-ttu-id="966c2-112">Die Höhe der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="966c2-112">The height of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="966c2-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="966c2-113">sourceItemId</span></span> | <span data-ttu-id="966c2-114">String</span><span class="sxs-lookup"><span data-stu-id="966c2-114">String</span></span> | <span data-ttu-id="966c2-p101">Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="966c2-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span>
| <span data-ttu-id="966c2-117">url</span><span class="sxs-lookup"><span data-stu-id="966c2-117">url</span></span>          | <span data-ttu-id="966c2-118">String</span><span class="sxs-lookup"><span data-stu-id="966c2-118">String</span></span> | <span data-ttu-id="966c2-119">Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="966c2-119">The URL used to fetch the thumbnail content.</span></span>
| <span data-ttu-id="966c2-120">width</span><span class="sxs-lookup"><span data-stu-id="966c2-120">width</span></span>        | <span data-ttu-id="966c2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="966c2-121">Int32</span></span>  | <span data-ttu-id="966c2-122">Die Breite der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="966c2-122">The width of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="966c2-123">content</span><span class="sxs-lookup"><span data-stu-id="966c2-123">content</span></span>      | <span data-ttu-id="966c2-124">Stream</span><span class="sxs-lookup"><span data-stu-id="966c2-124">Stream</span></span> | <span data-ttu-id="966c2-125">Der Inhaltsdatenstrom für die Miniaturansicht.</span><span class="sxs-lookup"><span data-stu-id="966c2-125">The content stream for the thumbnail.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
