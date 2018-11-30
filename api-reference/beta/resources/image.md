---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
ms.openlocfilehash: c9e647ef630e8822d835aec1bd72b9f3c18f2e3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063197"
---
# <a name="image-resource-type"></a><span data-ttu-id="cedc8-102">Image-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cedc8-102">Image resource type</span></span>

> <span data-ttu-id="cedc8-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cedc8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cedc8-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cedc8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cedc8-p102">Die **Image**-Ressourc gruppiert bildbezogene Eigenschaften in einer einzelnen Struktur. Wenn ein [**DriveItem**](driveitem.md) ein **image**-Facet ungleich Null aufweist, stellt das Element eine Bitmapdatei dar.</span><span class="sxs-lookup"><span data-stu-id="cedc8-p102">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="cedc8-107">**Hinweis:** Wenn der Dienst die Breite und Höhe des Bilds nicht bestimmen kann, ist die **Image**-Ressource möglicherweise leer.</span><span class="sxs-lookup"><span data-stu-id="cedc8-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cedc8-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cedc8-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="cedc8-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cedc8-109">Properties</span></span>

| <span data-ttu-id="cedc8-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cedc8-110">Property</span></span>   | <span data-ttu-id="cedc8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="cedc8-111">Type</span></span>  | <span data-ttu-id="cedc8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cedc8-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="cedc8-113">**height**</span><span class="sxs-lookup"><span data-stu-id="cedc8-113">**height**</span></span> | <span data-ttu-id="cedc8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="cedc8-114">Int32</span></span> | <span data-ttu-id="cedc8-p103">Optional. Die Höhe des Bilds in Pixel. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cedc8-p103">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="cedc8-118">**width**</span><span class="sxs-lookup"><span data-stu-id="cedc8-118">**width**</span></span>  | <span data-ttu-id="cedc8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cedc8-119">Int32</span></span> | <span data-ttu-id="cedc8-p104">Optional. Die Breite des Bilds in Pixel. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cedc8-p104">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="cedc8-123">Hinweise</span><span class="sxs-lookup"><span data-stu-id="cedc8-123">Remarks</span></span>

<span data-ttu-id="cedc8-124">In OneDrive for Business wird diese Ressource für Elemente zurückgegeben, von denen basierend auf der Dateierweiterung davon ausgegangen wird, dass es sich um Bilder handelt.</span><span class="sxs-lookup"><span data-stu-id="cedc8-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="cedc8-125">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="cedc8-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
