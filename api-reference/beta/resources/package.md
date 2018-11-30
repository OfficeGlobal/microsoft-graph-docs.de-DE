---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Paket
ms.openlocfilehash: fe26cf0dc5de00673d5c3c2ae4a90ac80a62897f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064480"
---
# <a name="package-resource-type"></a><span data-ttu-id="c0be4-102">Package-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c0be4-102">Package resource type</span></span>

> <span data-ttu-id="c0be4-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0be4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0be4-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0be4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0be4-105">Die **Package**-Ressource gibt an, dass ein DriveItem das Element der obersten Ebene in einem „Paket“ oder einer Sammlung von Elementen ist, die als eine Sammlung und nicht als einzelne Elemente behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="c0be4-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="c0be4-106">Ein Beispiel für ein Paket ist ein OneNote-Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="c0be4-106">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="c0be4-107">Während das Notizbuch aus Dateien und Ordnern besteht, die die Inhalte des Notizbuchs darstellen, weist das Element der obersten Ebene, das das Notizbuch darstellt, ein **package**-Facet auf, um für Clients anzugeben, dass es sich dabei um eine Sammlung von Daten handelt, die auf besondere Weise behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="c0be4-107">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="c0be4-108">DriveItems mit dem **package**-Facet enthalten keine **folder**- oder **file**-Facets, sie ähneln jedoch Elementen mit einem **folder**-Facet.</span><span class="sxs-lookup"><span data-stu-id="c0be4-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0be4-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c0be4-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="c0be4-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="c0be4-110">Property Name</span></span> | <span data-ttu-id="c0be4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c0be4-111">Type</span></span>   | <span data-ttu-id="c0be4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0be4-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c0be4-113">**type**</span><span class="sxs-lookup"><span data-stu-id="c0be4-113">**type**</span></span>      | <span data-ttu-id="c0be4-114">string</span><span class="sxs-lookup"><span data-stu-id="c0be4-114">string</span></span> | <span data-ttu-id="c0be4-p103">Eine Zeichenfolge, die den Typ des Pakets angibt. Obwohl `oneNote` der einzige derzeit definierte Wert ist, sollten Sie davon ausgehen, dass andere Paketarten zurückgegeben werden, die entsprechend behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="c0be4-p103">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c0be4-117">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="c0be4-117">Remarks</span></span> 

<span data-ttu-id="c0be4-118">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c0be4-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation"
} -->
