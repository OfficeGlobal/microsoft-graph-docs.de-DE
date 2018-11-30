---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Ordner
ms.openlocfilehash: 834b2cd7c81a947ca1e6d4619f39a8533677e6c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064205"
---
# <a name="folder-resource-type"></a><span data-ttu-id="7ec24-102">Folder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7ec24-102">Folder resource type</span></span>

> <span data-ttu-id="7ec24-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ec24-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ec24-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ec24-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ec24-p102">Die **Folder**-Ressource gruppiert ordnerbezogene Daten für ein Element in einer einzelnen Struktur. [**DriveItems**](driveitem.md) mit einem **Ordner**-Facet, das nicht Null ist, sind Container für andere DriveItems.</span><span class="sxs-lookup"><span data-stu-id="7ec24-p102">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ec24-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7ec24-107">JSON representation</span></span>

<span data-ttu-id="7ec24-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7ec24-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7ec24-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7ec24-109">Properties</span></span>

| <span data-ttu-id="7ec24-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ec24-110">Property</span></span>       | <span data-ttu-id="7ec24-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7ec24-111">Type</span></span>           | <span data-ttu-id="7ec24-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ec24-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="7ec24-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="7ec24-113">**childCount**</span></span> | <span data-ttu-id="7ec24-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7ec24-114">Int64</span></span>          | <span data-ttu-id="7ec24-115">Die Anzahl von direkt in dem jeweiligen Container enthaltenen untergeordneten Elementen.</span><span class="sxs-lookup"><span data-stu-id="7ec24-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="7ec24-116">**view**</span><span class="sxs-lookup"><span data-stu-id="7ec24-116">**view**</span></span>       | <span data-ttu-id="7ec24-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="7ec24-117">[folderView][]</span></span> | <span data-ttu-id="7ec24-118">Eine Sammlung von Eigenschaften, welche die empfohlene Ansicht für den Ordner definieren.</span><span class="sxs-lookup"><span data-stu-id="7ec24-118">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="7ec24-119">Hinweise</span><span class="sxs-lookup"><span data-stu-id="7ec24-119">Remarks</span></span> 

<span data-ttu-id="7ec24-120">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="7ec24-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
