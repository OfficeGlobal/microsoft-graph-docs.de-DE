---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: 6316f31d41e9d8e7264a671ac0317ebf9b32173f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804767"
---
# <a name="deleted-facet"></a><span data-ttu-id="b6271-102">Facet „Deleted“</span><span class="sxs-lookup"><span data-stu-id="b6271-102">Deleted facet</span></span>

> <span data-ttu-id="b6271-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b6271-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6271-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6271-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6271-p102">Die **Deleted**-Ressource gibt an, dass das Element gelöscht wurde. In dieser Version der API gibt das Vorhandensein (nicht Null) des Ressourcenwerts an, dass die Datei gelöscht wurde. Ein NULL-Werte (oder ein fehlender Wert) gibt an, dass die Datei nicht gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="b6271-p102">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="b6271-108">Unter [Änderungen für ein Element anzeigen](../api/driveitem-delta.md) finden Sie weitere Informationen zum Nachverfolgen von Änderungen und zum Suchen gelöschter Elemente.</span><span class="sxs-lookup"><span data-stu-id="b6271-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6271-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b6271-109">JSON representation</span></span>

<span data-ttu-id="b6271-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b6271-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b6271-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b6271-111">Properties</span></span>

| <span data-ttu-id="b6271-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b6271-112">Property</span></span> | <span data-ttu-id="b6271-113">Typ</span><span class="sxs-lookup"><span data-stu-id="b6271-113">Type</span></span>   | <span data-ttu-id="b6271-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6271-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="b6271-115">state</span><span class="sxs-lookup"><span data-stu-id="b6271-115">state</span></span>    | <span data-ttu-id="b6271-116">String</span><span class="sxs-lookup"><span data-stu-id="b6271-116">String</span></span> | <span data-ttu-id="b6271-117">Stellt den Status des gelöschten Elements dar.</span><span class="sxs-lookup"><span data-stu-id="b6271-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="b6271-118">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="b6271-118">Remarks</span></span> 

<span data-ttu-id="b6271-119">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b6271-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
