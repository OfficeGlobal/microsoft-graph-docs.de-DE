---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
ms.openlocfilehash: 1d45219b2ef26bdc96c46e386d66d91874f9bc0b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="deleted-facet"></a><span data-ttu-id="2f3d5-102">Deleted-Facet</span><span class="sxs-lookup"><span data-stu-id="2f3d5-102">Deleted facet</span></span>

<span data-ttu-id="2f3d5-103">Die **Deleted**-Ressource gibt an, dass das Element gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="2f3d5-103">The **Deleted** resource indicates that the item has been deleted.</span></span>
<span data-ttu-id="2f3d5-104">In dieser Version der API gibt das Vorhandensein (nicht Null) des Ressourcenwerts an, dass die Datei gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="2f3d5-104">The Deleted resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>
<span data-ttu-id="2f3d5-105">Ein NULL-Werte (oder ein fehlender Wert) gibt an, dass die Datei nicht gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="2f3d5-105">A null (or missing) value indicates the driveItem is not the root..</span></span>

<span data-ttu-id="2f3d5-106">Unter [Anzeigen von Änderungen für ein Element](../api/driveitem_delta.md) finden Sie weitere Informationen zum Nachverfolgen von Änderungen und zum Suchen gelöschter Elemente.</span><span class="sxs-lookup"><span data-stu-id="2f3d5-106">See [view changes for an item](../api/driveitem_delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f3d5-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2f3d5-107">JSON representation</span></span>

<span data-ttu-id="2f3d5-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2f3d5-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a><span data-ttu-id="2f3d5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2f3d5-109">Properties</span></span>

| <span data-ttu-id="2f3d5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f3d5-110">Property</span></span> | <span data-ttu-id="2f3d5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="2f3d5-111">Type</span></span>   | <span data-ttu-id="2f3d5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f3d5-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="2f3d5-113">state</span><span class="sxs-lookup"><span data-stu-id="2f3d5-113">state</span></span>    | <span data-ttu-id="2f3d5-114">String</span><span class="sxs-lookup"><span data-stu-id="2f3d5-114">String</span></span> | <span data-ttu-id="2f3d5-115">Stellt den Status des gelöschten Elements dar.</span><span class="sxs-lookup"><span data-stu-id="2f3d5-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="2f3d5-116">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="2f3d5-116">Remarks</span></span> 

<span data-ttu-id="2f3d5-117">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2f3d5-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
