---
title: licenseUnitsDetail-Ressourcentyp
description: Die **prepaidUnits**-Eigenschaft der subscribedSku-Entität ist vom Typ **licenseUnitsDetail**.
ms.openlocfilehash: 5f3d62c39248739746923195945efbc3322d5686
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058206"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="36d01-103">licenseUnitsDetail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="36d01-103">licenseUnitsDetail resource type</span></span>

> <span data-ttu-id="36d01-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="36d01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36d01-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36d01-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36d01-106">Die **prepaidUnits**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist vom Typ **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="36d01-106">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="36d01-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36d01-107">Properties</span></span>
| <span data-ttu-id="36d01-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36d01-108">Property</span></span>     | <span data-ttu-id="36d01-109">Typ</span><span class="sxs-lookup"><span data-stu-id="36d01-109">Type</span></span>   |<span data-ttu-id="36d01-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36d01-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="36d01-111">aktiviert</span><span class="sxs-lookup"><span data-stu-id="36d01-111">enabled</span></span>|<span data-ttu-id="36d01-112">Int32</span><span class="sxs-lookup"><span data-stu-id="36d01-112">Int32</span></span>| <span data-ttu-id="36d01-113">Die Anzahl der Einheiten, die aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="36d01-113">The number of units that are enabled.</span></span> |
|<span data-ttu-id="36d01-114">suspended</span><span class="sxs-lookup"><span data-stu-id="36d01-114">suspended</span></span>|<span data-ttu-id="36d01-115">Int32</span><span class="sxs-lookup"><span data-stu-id="36d01-115">Int32</span></span>| <span data-ttu-id="36d01-116">Die Anzahl der Einheiten, die angehalten werden.</span><span class="sxs-lookup"><span data-stu-id="36d01-116">The number of units that are suspended.</span></span> |
|<span data-ttu-id="36d01-117">warning</span><span class="sxs-lookup"><span data-stu-id="36d01-117">warning</span></span>|<span data-ttu-id="36d01-118">Int32</span><span class="sxs-lookup"><span data-stu-id="36d01-118">Int32</span></span>| <span data-ttu-id="36d01-119">Die Anzahl der Einheiten, für die eine Warnung vorliegt.</span><span class="sxs-lookup"><span data-stu-id="36d01-119">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="36d01-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="36d01-120">JSON representation</span></span>

<span data-ttu-id="36d01-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="36d01-121">Here is a JSON representation of the resource</span></span>

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
