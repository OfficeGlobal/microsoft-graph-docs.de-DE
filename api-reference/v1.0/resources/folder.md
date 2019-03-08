---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Ordner
localization_priority: Normal
ms.openlocfilehash: 2c98cb57bfd860b568b1cba95ed7f6fcf455eea1
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480817"
---
# <a name="folder-resource-type"></a><span data-ttu-id="67a0f-102">Folder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="67a0f-102">Folder resource type</span></span>

<span data-ttu-id="67a0f-p101">Die **Folder**-Ressource gruppiert ordnerbezogene Daten für ein Element in einer einzelnen Struktur. [**DriveItems**](driveitem.md) mit einem **Ordner**-Facet, das nicht Null ist, sind Container für andere DriveItems.</span><span class="sxs-lookup"><span data-stu-id="67a0f-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67a0f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="67a0f-105">JSON representation</span></span>

<span data-ttu-id="67a0f-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="67a0f-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="67a0f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="67a0f-107">Properties</span></span>

| <span data-ttu-id="67a0f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67a0f-108">Property</span></span>       | <span data-ttu-id="67a0f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="67a0f-109">Type</span></span>           | <span data-ttu-id="67a0f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67a0f-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="67a0f-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="67a0f-111">**childCount**</span></span> | <span data-ttu-id="67a0f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="67a0f-112">Int32</span></span>          | <span data-ttu-id="67a0f-113">Die Anzahl von direkt in dem jeweiligen Container enthaltenen untergeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="67a0f-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="67a0f-114">**view**</span><span class="sxs-lookup"><span data-stu-id="67a0f-114">**view**</span></span>       | <span data-ttu-id="67a0f-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="67a0f-115">[folderView][]</span></span> | <span data-ttu-id="67a0f-116">Eine Sammlung von Eigenschaften, welche die empfohlene Ansicht für den Ordner definieren.</span><span class="sxs-lookup"><span data-stu-id="67a0f-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="67a0f-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="67a0f-117">Remarks</span></span> 

<span data-ttu-id="67a0f-118">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="67a0f-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
