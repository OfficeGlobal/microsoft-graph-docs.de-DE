---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Ordner
localization_priority: Normal
ms.openlocfilehash: b78e6038a8f8f9a91883dd29faeebe3d5db3ca04
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481216"
---
# <a name="folder-resource-type"></a><span data-ttu-id="28d2a-102">Folder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="28d2a-102">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28d2a-p101">Die **Folder**-Ressource gruppiert ordnerbezogene Daten für ein Element in einer einzelnen Struktur. [**DriveItems**](driveitem.md) mit einem **Ordner**-Facet, das nicht Null ist, sind Container für andere DriveItems.</span><span class="sxs-lookup"><span data-stu-id="28d2a-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28d2a-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28d2a-105">JSON representation</span></span>

<span data-ttu-id="28d2a-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="28d2a-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a><span data-ttu-id="28d2a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28d2a-107">Properties</span></span>

| <span data-ttu-id="28d2a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28d2a-108">Property</span></span>       | <span data-ttu-id="28d2a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="28d2a-109">Type</span></span>           | <span data-ttu-id="28d2a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28d2a-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="28d2a-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="28d2a-111">**childCount**</span></span> | <span data-ttu-id="28d2a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="28d2a-112">Int64</span></span>          | <span data-ttu-id="28d2a-113">Die Anzahl von direkt in dem jeweiligen Container enthaltenen untergeordneten Elementen.</span><span class="sxs-lookup"><span data-stu-id="28d2a-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="28d2a-114">**view**</span><span class="sxs-lookup"><span data-stu-id="28d2a-114">**view**</span></span>       | <span data-ttu-id="28d2a-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="28d2a-115">[folderView][]</span></span> | <span data-ttu-id="28d2a-116">Eine Sammlung von Eigenschaften, welche die empfohlene Ansicht für den Ordner definieren.</span><span class="sxs-lookup"><span data-stu-id="28d2a-116">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="28d2a-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="28d2a-117">Remarks</span></span> 

<span data-ttu-id="28d2a-118">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="28d2a-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
