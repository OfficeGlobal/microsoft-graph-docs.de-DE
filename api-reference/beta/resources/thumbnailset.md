---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: 145134d6a3ad85134ea2d6c4d72e050bc17b31d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830191"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="f18ec-102">ThumbnailSet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f18ec-102">ThumbnailSet resource type</span></span>

> <span data-ttu-id="f18ec-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f18ec-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f18ec-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f18ec-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f18ec-p102">Die **ThumbnailSet**-Ressource ist eine verschlüsselter Sammlung von [thumbnail](thumbnail.md)-Ressourcen. Sie wird zum Darstellen eines Satzes von Miniaturansichten verwendet, die mit einem DriveItem verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="f18ec-p102">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f18ec-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f18ec-107">JSON representation</span></span>

<span data-ttu-id="f18ec-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f18ec-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="f18ec-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f18ec-109">Properties</span></span>

| <span data-ttu-id="f18ec-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f18ec-110">Property</span></span> | <span data-ttu-id="f18ec-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f18ec-111">Type</span></span>                      | <span data-ttu-id="f18ec-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f18ec-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="f18ec-113">id</span><span class="sxs-lookup"><span data-stu-id="f18ec-113">id</span></span>       | <span data-ttu-id="f18ec-114">String</span><span class="sxs-lookup"><span data-stu-id="f18ec-114">String</span></span>                    | <span data-ttu-id="f18ec-p103">Die ID innerhalb des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f18ec-p103">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="f18ec-117">large</span><span class="sxs-lookup"><span data-stu-id="f18ec-117">large</span></span>    | [<span data-ttu-id="f18ec-118">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="f18ec-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ec-119">Eine skalierte Miniaturansicht von 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="f18ec-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="f18ec-120">medium</span><span class="sxs-lookup"><span data-stu-id="f18ec-120">medium</span></span>   | [<span data-ttu-id="f18ec-121">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="f18ec-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ec-122">Eine skalierte Miniaturansicht von 176x176.</span><span class="sxs-lookup"><span data-stu-id="f18ec-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="f18ec-123">small</span><span class="sxs-lookup"><span data-stu-id="f18ec-123">small</span></span>    | [<span data-ttu-id="f18ec-124">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="f18ec-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ec-125">Eine zugeschnittene Miniaturansicht von 48x48.</span><span class="sxs-lookup"><span data-stu-id="f18ec-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="f18ec-126">source</span><span class="sxs-lookup"><span data-stu-id="f18ec-126">source</span></span>   | [<span data-ttu-id="f18ec-127">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="f18ec-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f18ec-128">Eine benutzerdefiniertes Miniaturbild oder das ursprüngliche Bild, das zum Erstellen anderer Miniaturansichten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f18ec-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
