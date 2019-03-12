---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Paket
localization_priority: Normal
ms.openlocfilehash: c64dfce910456ef9b9415e3332c099d7814a71f2
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482203"
---
# <a name="package-resource-type"></a><span data-ttu-id="f3a82-102">Package-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f3a82-102">Package resource type</span></span>

<span data-ttu-id="f3a82-103">Die **Package**-Ressource gibt an, dass ein DriveItem das Element der obersten Ebene in einem „Paket“ oder einer Sammlung von Elementen ist, die als eine Sammlung und nicht als einzelne Elemente behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f3a82-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="f3a82-p101">Ein Beispiel für ein Paket ist ein OneNote-Notizbuch. Während das Notizbuch aus Dateien und Ordnern besteht, die die Inhalte des Notizbuchs darstellen, weist das Element der obersten Ebene, das das Notizbuch darstellt, ein **package**-Facet auf, um für Clients anzugeben, dass es sich dabei um eine Sammlung von Daten handelt, die auf besondere Weise behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f3a82-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="f3a82-106">DriveItems mit dem **package**-Facet enthalten keine **folder**- oder **file**-Facets, sie ähneln jedoch Elementen mit einem **folder**-Facet.</span><span class="sxs-lookup"><span data-stu-id="f3a82-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3a82-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f3a82-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="f3a82-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f3a82-108">Properties</span></span>

| <span data-ttu-id="f3a82-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="f3a82-109">Property Name</span></span> | <span data-ttu-id="f3a82-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f3a82-110">Type</span></span>   | <span data-ttu-id="f3a82-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3a82-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f3a82-112">type</span><span class="sxs-lookup"><span data-stu-id="f3a82-112">type</span></span>          | <span data-ttu-id="f3a82-113">string</span><span class="sxs-lookup"><span data-stu-id="f3a82-113">string</span></span> | <span data-ttu-id="f3a82-114">Eine Zeichenfolge, die den Typ des Pakets angibt.</span><span class="sxs-lookup"><span data-stu-id="f3a82-114">A string indicating the type of package.</span></span> <span data-ttu-id="f3a82-115">Obwohl `oneNote` der einzige derzeit definierte Wert ist, sollten Sie davon ausgehen, dass andere Paketarten zurückgegeben werden, die entsprechend behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f3a82-115">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="f3a82-116">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="f3a82-116">Remarks</span></span> 

<span data-ttu-id="f3a82-117">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f3a82-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
