---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 4526b8d475b36521ee08829b50931438999ca249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830415"
---
# <a name="image-resource-type"></a><span data-ttu-id="99a17-102">Image-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="99a17-102">Image resource type</span></span>

<span data-ttu-id="99a17-p101">Die **Image**-Ressourc gruppiert bildbezogene Eigenschaften in einer einzelnen Struktur. Wenn ein [**DriveItem**](driveitem.md) ein **image**-Facet ungleich Null aufweist, stellt das Element eine Bitmapdatei dar.</span><span class="sxs-lookup"><span data-stu-id="99a17-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="99a17-105">**Hinweis:** Wenn der Dienst die Breite und Höhe des Bilds nicht bestimmen kann, ist die **Image**-Ressource möglicherweise leer.</span><span class="sxs-lookup"><span data-stu-id="99a17-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99a17-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="99a17-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="99a17-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="99a17-107">Properties</span></span>

| <span data-ttu-id="99a17-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99a17-108">Property</span></span>   | <span data-ttu-id="99a17-109">Typ</span><span class="sxs-lookup"><span data-stu-id="99a17-109">Type</span></span>  | <span data-ttu-id="99a17-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99a17-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="99a17-111">**height**</span><span class="sxs-lookup"><span data-stu-id="99a17-111">**height**</span></span> | <span data-ttu-id="99a17-112">Int32</span><span class="sxs-lookup"><span data-stu-id="99a17-112">Int32</span></span> | <span data-ttu-id="99a17-p102">Optional. Die Höhe des Bilds in Pixel. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="99a17-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="99a17-116">**width**</span><span class="sxs-lookup"><span data-stu-id="99a17-116">**width**</span></span>  | <span data-ttu-id="99a17-117">Int32</span><span class="sxs-lookup"><span data-stu-id="99a17-117">Int32</span></span> | <span data-ttu-id="99a17-p103">Optional. Die Breite des Bilds in Pixel. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="99a17-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="99a17-121">Hinweise</span><span class="sxs-lookup"><span data-stu-id="99a17-121">Remarks</span></span>

<span data-ttu-id="99a17-122">In OneDrive for Business wird diese Ressource für Elemente zurückgegeben, von denen basierend auf der Dateierweiterung davon ausgegangen wird, dass es sich um Bilder handelt.</span><span class="sxs-lookup"><span data-stu-id="99a17-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="99a17-123">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="99a17-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
