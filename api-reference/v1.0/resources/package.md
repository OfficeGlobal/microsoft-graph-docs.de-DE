---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Paket
ms.openlocfilehash: 12ae750a0f4fbe0e951554308d4041928c31a16d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018928"
---
# <a name="package-resource-type"></a><span data-ttu-id="844ba-102">Package-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="844ba-102">Package resource type</span></span>

<span data-ttu-id="844ba-103">Die **Package**-Ressource gibt an, dass ein DriveItem das Element der obersten Ebene in einem „Paket“ oder einer Sammlung von Elementen ist, die als eine Sammlung und nicht als einzelne Elemente behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="844ba-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="844ba-104">Ein Beispiel für ein Paket ist ein OneNote-Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="844ba-104">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="844ba-105">Während das Notizbuch aus Dateien und Ordnern besteht, die die Inhalte des Notizbuchs darstellen, weist das Element der obersten Ebene, das das Notizbuch darstellt, ein **package**-Facet auf, um für Clients anzugeben, dass es sich dabei um eine Sammlung von Daten handelt, die auf besondere Weise behandelt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="844ba-105">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="844ba-106">DriveItems mit dem **package**-Facet enthalten keine **folder**- oder **file**-Facets, sie ähneln jedoch Elementen mit einem **folder**-Facet.</span><span class="sxs-lookup"><span data-stu-id="844ba-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="844ba-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="844ba-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="844ba-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="844ba-108">Properties</span></span>

| <span data-ttu-id="844ba-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="844ba-109">Property Name</span></span> | <span data-ttu-id="844ba-110">Typ</span><span class="sxs-lookup"><span data-stu-id="844ba-110">Type</span></span>   | <span data-ttu-id="844ba-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="844ba-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="844ba-112">Typ</span><span class="sxs-lookup"><span data-stu-id="844ba-112">type</span></span>          | <span data-ttu-id="844ba-113">string</span><span class="sxs-lookup"><span data-stu-id="844ba-113">string</span></span> | <span data-ttu-id="844ba-114">Eine Zeichenfolge, die den Typ des Pakets angibt.</span><span class="sxs-lookup"><span data-stu-id="844ba-114">A string indicating the type of package.</span></span> <span data-ttu-id="844ba-115">Während `oneNote` ist der einzige Wert derzeit definiert sind, sollten Sie erwarten, andere Pakettypen zurückgegeben werden, und sie entsprechend behandelt.</span><span class="sxs-lookup"><span data-stu-id="844ba-115">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="844ba-116">Hinweise</span><span class="sxs-lookup"><span data-stu-id="844ba-116">Remarks</span></span> 

<span data-ttu-id="844ba-117">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="844ba-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
