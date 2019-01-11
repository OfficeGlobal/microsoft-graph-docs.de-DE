---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: a35bc781555486603c0319c819aa019704e362d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886142"
---
# <a name="deleted-facet"></a><span data-ttu-id="300a3-102">Facet „Deleted“</span><span class="sxs-lookup"><span data-stu-id="300a3-102">Deleted facet</span></span>

<span data-ttu-id="300a3-p101">Die **Deleted**-Ressource gibt an, dass das Element gelöscht wurde. In dieser Version der API gibt das Vorhandensein (nicht Null) des Ressourcenwerts an, dass die Datei gelöscht wurde. Ein NULL-Werte (oder ein fehlender Wert) gibt an, dass die Datei nicht gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="300a3-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="300a3-106">Unter [Änderungen für ein Element anzeigen](../api/driveitem-delta.md) finden Sie weitere Informationen zum Nachverfolgen von Änderungen und zum Suchen gelöschter Elemente.</span><span class="sxs-lookup"><span data-stu-id="300a3-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="300a3-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="300a3-107">JSON representation</span></span>

<span data-ttu-id="300a3-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="300a3-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="300a3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="300a3-109">Properties</span></span>

| <span data-ttu-id="300a3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="300a3-110">Property</span></span> | <span data-ttu-id="300a3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="300a3-111">Type</span></span>   | <span data-ttu-id="300a3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="300a3-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="300a3-113">state</span><span class="sxs-lookup"><span data-stu-id="300a3-113">state</span></span>    | <span data-ttu-id="300a3-114">String</span><span class="sxs-lookup"><span data-stu-id="300a3-114">String</span></span> | <span data-ttu-id="300a3-115">Stellt den Status des gelöschten Elements dar.</span><span class="sxs-lookup"><span data-stu-id="300a3-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="300a3-116">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="300a3-116">Remarks</span></span> 

<span data-ttu-id="300a3-117">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="300a3-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
