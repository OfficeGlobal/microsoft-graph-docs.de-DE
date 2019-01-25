---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: de832eb4ecdf36081b00b94679dcafe9b94fe007
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529439"
---
# <a name="deleted-facet"></a><span data-ttu-id="6b94e-102">Facet „Deleted“</span><span class="sxs-lookup"><span data-stu-id="6b94e-102">Deleted facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b94e-p101">Die Deleted-Ressource gibt an, dass das Element gelöscht wurde. In dieser Version der API gibt das Vorhandensein (nicht Null) des Ressourcenwerts an, dass die Datei gelöscht wurde. Ein NULL-Werte (oder ein fehlender Wert) gibt an, dass die Datei nicht gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="6b94e-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="6b94e-106">Unter [Änderungen für ein Element anzeigen](../api/driveitem-delta.md) finden Sie weitere Informationen zum Nachverfolgen von Änderungen und zum Suchen gelöschter Elemente.</span><span class="sxs-lookup"><span data-stu-id="6b94e-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b94e-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b94e-107">JSON representation</span></span>

<span data-ttu-id="6b94e-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b94e-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6b94e-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b94e-109">Properties</span></span>

| <span data-ttu-id="6b94e-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b94e-110">Property</span></span> | <span data-ttu-id="6b94e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6b94e-111">Type</span></span>   | <span data-ttu-id="6b94e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b94e-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="6b94e-113">state</span><span class="sxs-lookup"><span data-stu-id="6b94e-113">state</span></span>    | <span data-ttu-id="6b94e-114">String</span><span class="sxs-lookup"><span data-stu-id="6b94e-114">String</span></span> | <span data-ttu-id="6b94e-115">Stellt den Status des gelöschten Elements dar.</span><span class="sxs-lookup"><span data-stu-id="6b94e-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="6b94e-116">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="6b94e-116">Remarks</span></span> 

<span data-ttu-id="6b94e-117">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6b94e-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleted.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
