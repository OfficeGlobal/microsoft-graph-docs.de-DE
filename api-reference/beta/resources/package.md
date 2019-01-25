---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Paket
localization_priority: Normal
ms.openlocfilehash: 67e82faa3f51eeae71c2dcb22ecb7a973e2070bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516602"
---
# <a name="package-resource-type"></a><span data-ttu-id="ff9c1-102">Package-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ff9c1-102">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff9c1-103">Die **Package**-Ressource gibt an, dass ein DriveItem das Element der obersten Ebene in einem „Paket“ oder einer Sammlung von Elementen ist, die als eine Sammlung und nicht als einzelne Elemente behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="ff9c1-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="ff9c1-p101">Ein Beispiel für ein Paket ist ein OneNote-Notizbuch. Während das Notizbuch aus Dateien und Ordnern besteht, die die Inhalte des Notizbuchs darstellen, weist das Element der obersten Ebene, das das Notizbuch darstellt, ein **Package**-Facet auf, um für Clients anzugeben, dass es sich dabei um eine Sammlung von Daten handelt, die auf besondere Weise behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="ff9c1-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="ff9c1-106">DriveItems mit dem **package**-Facet enthalten keine **folder**- oder **file**-Facets, sie ähneln jedoch Elementen mit einem **folder**-Facet.</span><span class="sxs-lookup"><span data-stu-id="ff9c1-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff9c1-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff9c1-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="ff9c1-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ff9c1-108">Property Name</span></span> | <span data-ttu-id="ff9c1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ff9c1-109">Type</span></span>   | <span data-ttu-id="ff9c1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff9c1-110">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ff9c1-111">**type**</span><span class="sxs-lookup"><span data-stu-id="ff9c1-111">**type**</span></span>      | <span data-ttu-id="ff9c1-112">string</span><span class="sxs-lookup"><span data-stu-id="ff9c1-112">string</span></span> | <span data-ttu-id="ff9c1-p102">Eine Zeichenfolge, die den Typ des Pakets angibt. Obwohl `oneNote` der einzige derzeit definierte Wert ist, sollten Sie davon ausgehen, dass andere Paketarten zurückgegeben werden, die entsprechend behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="ff9c1-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="ff9c1-115">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="ff9c1-115">Remarks</span></span> 

<span data-ttu-id="ff9c1-116">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ff9c1-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/package.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
