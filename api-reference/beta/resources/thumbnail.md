---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
ms.openlocfilehash: 22602d534c3fd1f308a5e2bb67992bd76086c4fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863224"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="17a2e-102">Thumbnail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="17a2e-102">Thumbnail resource type</span></span>

> <span data-ttu-id="17a2e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="17a2e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17a2e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17a2e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17a2e-105">Der **thumbnail**-Ressourcentyp stellt eine Miniaturansicht für ein Bild, ein Video, ein Dokument oder ein beliebiges Element dar, das über eine Bitmapdarstellung verfügt.</span><span class="sxs-lookup"><span data-stu-id="17a2e-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17a2e-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17a2e-106">JSON representation</span></span>

<span data-ttu-id="17a2e-107">Es folgt eine JSON-Darstellung der **thumbnail**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="17a2e-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="17a2e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17a2e-108">Properties</span></span>

| <span data-ttu-id="17a2e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17a2e-109">Property</span></span>     | <span data-ttu-id="17a2e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="17a2e-110">Type</span></span>   | <span data-ttu-id="17a2e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17a2e-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="17a2e-112">height</span><span class="sxs-lookup"><span data-stu-id="17a2e-112">height</span></span>       | <span data-ttu-id="17a2e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="17a2e-113">Int32</span></span>  | <span data-ttu-id="17a2e-114">Die Höhe der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="17a2e-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="17a2e-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="17a2e-115">sourceItemId</span></span> | <span data-ttu-id="17a2e-116">String</span><span class="sxs-lookup"><span data-stu-id="17a2e-116">String</span></span> | <span data-ttu-id="17a2e-p102">Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="17a2e-p102">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="17a2e-119">url</span><span class="sxs-lookup"><span data-stu-id="17a2e-119">url</span></span>          | <span data-ttu-id="17a2e-120">String</span><span class="sxs-lookup"><span data-stu-id="17a2e-120">String</span></span> | <span data-ttu-id="17a2e-121">Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="17a2e-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="17a2e-122">width</span><span class="sxs-lookup"><span data-stu-id="17a2e-122">width</span></span>        | <span data-ttu-id="17a2e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="17a2e-123">Int32</span></span>  | <span data-ttu-id="17a2e-124">Die Breite der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="17a2e-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="17a2e-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="17a2e-125">Relationships</span></span>

| <span data-ttu-id="17a2e-126">Name</span><span class="sxs-lookup"><span data-stu-id="17a2e-126">Name</span></span>    | <span data-ttu-id="17a2e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="17a2e-127">Type</span></span>   | <span data-ttu-id="17a2e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17a2e-128">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="17a2e-129">Inhalt</span><span class="sxs-lookup"><span data-stu-id="17a2e-129">content</span></span> | <span data-ttu-id="17a2e-130">Stream</span><span class="sxs-lookup"><span data-stu-id="17a2e-130">Stream</span></span> | <span data-ttu-id="17a2e-131">Der Inhaltsdatenstrom für die Miniaturansicht.</span><span class="sxs-lookup"><span data-stu-id="17a2e-131">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
