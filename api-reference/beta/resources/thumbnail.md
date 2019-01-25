---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
ms.openlocfilehash: 05fcb6ec4b0821a4243692aab9c15419eb2f630d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529754"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="191b8-102">Thumbnail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="191b8-102">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="191b8-103">Der **thumbnail**-Ressourcentyp stellt eine Miniaturansicht für ein Bild, ein Video, ein Dokument oder ein beliebiges Element dar, das über eine Bitmapdarstellung verfügt.</span><span class="sxs-lookup"><span data-stu-id="191b8-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="191b8-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="191b8-104">JSON representation</span></span>

<span data-ttu-id="191b8-105">Es folgt eine JSON-Darstellung der **thumbnail**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="191b8-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="191b8-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="191b8-106">Properties</span></span>

| <span data-ttu-id="191b8-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="191b8-107">Property</span></span>     | <span data-ttu-id="191b8-108">Typ</span><span class="sxs-lookup"><span data-stu-id="191b8-108">Type</span></span>   | <span data-ttu-id="191b8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="191b8-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="191b8-110">height</span><span class="sxs-lookup"><span data-stu-id="191b8-110">height</span></span>       | <span data-ttu-id="191b8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="191b8-111">Int32</span></span>  | <span data-ttu-id="191b8-112">Die Höhe der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="191b8-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="191b8-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="191b8-113">sourceItemId</span></span> | <span data-ttu-id="191b8-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="191b8-114">String</span></span> | <span data-ttu-id="191b8-p101">Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="191b8-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="191b8-117">url</span><span class="sxs-lookup"><span data-stu-id="191b8-117">url</span></span>          | <span data-ttu-id="191b8-118">String</span><span class="sxs-lookup"><span data-stu-id="191b8-118">String</span></span> | <span data-ttu-id="191b8-119">Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="191b8-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="191b8-120">width</span><span class="sxs-lookup"><span data-stu-id="191b8-120">width</span></span>        | <span data-ttu-id="191b8-121">Int32</span><span class="sxs-lookup"><span data-stu-id="191b8-121">Int32</span></span>  | <span data-ttu-id="191b8-122">Die Breite der Miniaturansicht in Pixel.</span><span class="sxs-lookup"><span data-stu-id="191b8-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="191b8-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="191b8-123">Relationships</span></span>

| <span data-ttu-id="191b8-124">Name</span><span class="sxs-lookup"><span data-stu-id="191b8-124">Name</span></span>    | <span data-ttu-id="191b8-125">Typ</span><span class="sxs-lookup"><span data-stu-id="191b8-125">Type</span></span>   | <span data-ttu-id="191b8-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="191b8-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="191b8-127">Inhalt</span><span class="sxs-lookup"><span data-stu-id="191b8-127">content</span></span> | <span data-ttu-id="191b8-128">Stream</span><span class="sxs-lookup"><span data-stu-id="191b8-128">Stream</span></span> | <span data-ttu-id="191b8-129">Der Inhaltsdatenstrom für die Miniaturansicht.</span><span class="sxs-lookup"><span data-stu-id="191b8-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
