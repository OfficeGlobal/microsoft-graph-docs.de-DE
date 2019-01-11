---
title: licenseUnitsDetail-Ressourcentyp
description: Die **prepaidUnits**-Eigenschaft der subscribedSku-Entität ist vom Typ **licenseUnitsDetail**.
localization_priority: Normal
ms.openlocfilehash: 8c2a4e995c7e1afa63b7f9daea6b61cbaf974958
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810696"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="185ed-103">licenseUnitsDetail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="185ed-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="185ed-104">Die **prepaidUnits**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist vom Typ **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="185ed-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="185ed-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="185ed-105">Properties</span></span>
| <span data-ttu-id="185ed-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="185ed-106">Property</span></span>     | <span data-ttu-id="185ed-107">Typ</span><span class="sxs-lookup"><span data-stu-id="185ed-107">Type</span></span>   |<span data-ttu-id="185ed-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="185ed-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="185ed-109">aktiviert</span><span class="sxs-lookup"><span data-stu-id="185ed-109">enabled</span></span>|<span data-ttu-id="185ed-110">Int32</span><span class="sxs-lookup"><span data-stu-id="185ed-110">Int32</span></span>| <span data-ttu-id="185ed-111">Die Anzahl der Einheiten, die aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="185ed-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="185ed-112">suspended</span><span class="sxs-lookup"><span data-stu-id="185ed-112">suspended</span></span>|<span data-ttu-id="185ed-113">Int32</span><span class="sxs-lookup"><span data-stu-id="185ed-113">Int32</span></span>| <span data-ttu-id="185ed-114">Die Anzahl der Einheiten, die angehalten werden.</span><span class="sxs-lookup"><span data-stu-id="185ed-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="185ed-115">warning</span><span class="sxs-lookup"><span data-stu-id="185ed-115">warning</span></span>|<span data-ttu-id="185ed-116">Int32</span><span class="sxs-lookup"><span data-stu-id="185ed-116">Int32</span></span>| <span data-ttu-id="185ed-117">Die Anzahl der Einheiten, für die eine Warnung vorliegt.</span><span class="sxs-lookup"><span data-stu-id="185ed-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="185ed-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="185ed-118">JSON representation</span></span>

<span data-ttu-id="185ed-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="185ed-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
