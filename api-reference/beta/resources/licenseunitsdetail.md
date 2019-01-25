---
title: licenseUnitsDetail-Ressourcentyp
description: Die prepaidUnits-Eigenschaft der subscribedSku-Entität ist vom Typ licenseUnitsDetail.
localization_priority: Normal
ms.openlocfilehash: a5eacb79dfca97b992e2f8584761aaa45beccd76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511317"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="4d7a3-103">licenseUnitsDetail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4d7a3-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d7a3-104">Die **prepaidUnits**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist vom Typ **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="4d7a3-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="4d7a3-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4d7a3-105">Properties</span></span>
| <span data-ttu-id="4d7a3-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d7a3-106">Property</span></span>     | <span data-ttu-id="4d7a3-107">Typ</span><span class="sxs-lookup"><span data-stu-id="4d7a3-107">Type</span></span>   |<span data-ttu-id="4d7a3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d7a3-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="4d7a3-109">aktiviert</span><span class="sxs-lookup"><span data-stu-id="4d7a3-109">enabled</span></span>|<span data-ttu-id="4d7a3-110">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7a3-110">Int32</span></span>| <span data-ttu-id="4d7a3-111">Die Anzahl der Einheiten, die aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="4d7a3-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="4d7a3-112">suspended</span><span class="sxs-lookup"><span data-stu-id="4d7a3-112">suspended</span></span>|<span data-ttu-id="4d7a3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7a3-113">Int32</span></span>| <span data-ttu-id="4d7a3-114">Die Anzahl der Einheiten, die angehalten werden.</span><span class="sxs-lookup"><span data-stu-id="4d7a3-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="4d7a3-115">warning</span><span class="sxs-lookup"><span data-stu-id="4d7a3-115">warning</span></span>|<span data-ttu-id="4d7a3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7a3-116">Int32</span></span>| <span data-ttu-id="4d7a3-117">Die Anzahl der Einheiten, für die eine Warnung vorliegt.</span><span class="sxs-lookup"><span data-stu-id="4d7a3-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d7a3-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4d7a3-118">JSON representation</span></span>

<span data-ttu-id="4d7a3-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d7a3-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseunitsdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
