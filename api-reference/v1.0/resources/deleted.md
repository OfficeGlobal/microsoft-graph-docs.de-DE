---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
ms.openlocfilehash: 6a51d858f529e65820d7bc55bb7ec8fec80186d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016435"
---
# <a name="deleted-facet"></a><span data-ttu-id="7369a-102">Facet „Deleted“</span><span class="sxs-lookup"><span data-stu-id="7369a-102">Deleted facet</span></span>

<span data-ttu-id="7369a-p101">Die **Deleted**-Ressource gibt an, dass das Element gelöscht wurde. In dieser Version der API gibt das Vorhandensein (nicht Null) des Ressourcenwerts an, dass die Datei gelöscht wurde. Ein NULL-Werte (oder ein fehlender Wert) gibt an, dass die Datei nicht gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="7369a-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="7369a-106">Unter [Änderungen für ein Element anzeigen](../api/driveitem-delta.md) finden Sie weitere Informationen zum Nachverfolgen von Änderungen und zum Suchen gelöschter Elemente.</span><span class="sxs-lookup"><span data-stu-id="7369a-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7369a-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7369a-107">JSON representation</span></span>

<span data-ttu-id="7369a-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7369a-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7369a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7369a-109">Properties</span></span>

| <span data-ttu-id="7369a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7369a-110">Property</span></span> | <span data-ttu-id="7369a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7369a-111">Type</span></span>   | <span data-ttu-id="7369a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7369a-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="7369a-113">state</span><span class="sxs-lookup"><span data-stu-id="7369a-113">state</span></span>    | <span data-ttu-id="7369a-114">String</span><span class="sxs-lookup"><span data-stu-id="7369a-114">String</span></span> | <span data-ttu-id="7369a-115">Stellt den Status des gelöschten Elements dar.</span><span class="sxs-lookup"><span data-stu-id="7369a-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="7369a-116">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="7369a-116">Remarks</span></span> 

<span data-ttu-id="7369a-117">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7369a-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
