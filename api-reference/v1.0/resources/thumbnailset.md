---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: a9d92d84c8495b8c138c34f752700ccd0aad64fd
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480131"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="2c53b-102">ThumbnailSet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2c53b-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="2c53b-p101">Die **ThumbnailSet**-Ressource ist eine verschlüsselter Sammlung von [thumbnail](thumbnail.md)-Ressourcen. Sie wird zum Darstellen eines Satzes von Miniaturansichten verwendet, die mit einem DriveItem verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="2c53b-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c53b-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2c53b-105">JSON representation</span></span>

<span data-ttu-id="2c53b-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2c53b-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "source",
    "small",
    "medium",
    "large"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "openType": true
}-->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="2c53b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2c53b-107">Properties</span></span>

| <span data-ttu-id="2c53b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c53b-108">Property</span></span> | <span data-ttu-id="2c53b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2c53b-109">Type</span></span>                      | <span data-ttu-id="2c53b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c53b-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="2c53b-111">id</span><span class="sxs-lookup"><span data-stu-id="2c53b-111">id</span></span>       | <span data-ttu-id="2c53b-112">String</span><span class="sxs-lookup"><span data-stu-id="2c53b-112">String</span></span>                    | <span data-ttu-id="2c53b-p102">Die ID innerhalb des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2c53b-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="2c53b-115">large</span><span class="sxs-lookup"><span data-stu-id="2c53b-115">large</span></span>    | [<span data-ttu-id="2c53b-116">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="2c53b-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="2c53b-117">Eine skalierte Miniaturansicht von 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="2c53b-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="2c53b-118">medium</span><span class="sxs-lookup"><span data-stu-id="2c53b-118">medium</span></span>   | [<span data-ttu-id="2c53b-119">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="2c53b-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="2c53b-120">Eine skalierte Miniaturansicht von 176x176.</span><span class="sxs-lookup"><span data-stu-id="2c53b-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="2c53b-121">small</span><span class="sxs-lookup"><span data-stu-id="2c53b-121">small</span></span>    | [<span data-ttu-id="2c53b-122">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="2c53b-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="2c53b-123">Eine zugeschnittene Miniaturansicht von 48x48.</span><span class="sxs-lookup"><span data-stu-id="2c53b-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="2c53b-124">source</span><span class="sxs-lookup"><span data-stu-id="2c53b-124">source</span></span>   | [<span data-ttu-id="2c53b-125">Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="2c53b-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="2c53b-126">Eine benutzerdefiniertes Miniaturbild oder das ursprüngliche Bild, das zum Erstellen anderer Miniaturansichten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="2c53b-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
