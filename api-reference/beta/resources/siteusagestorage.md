---
title: Ressourcentyp siteUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 1fdfa6cb2690d6dbacf5e534792061b6e64025d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059386"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="5564d-103">Ressourcentyp siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="5564d-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5564d-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5564d-104">Properties</span></span>

| <span data-ttu-id="5564d-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5564d-105">Property</span></span>           | <span data-ttu-id="5564d-106">Typ</span><span class="sxs-lookup"><span data-stu-id="5564d-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="5564d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5564d-107">reportRefreshDate</span></span>  | <span data-ttu-id="5564d-108">Datum</span><span class="sxs-lookup"><span data-stu-id="5564d-108">Date</span></span>   |
| <span data-ttu-id="5564d-109">Standorttyp</span><span class="sxs-lookup"><span data-stu-id="5564d-109">siteType</span></span>           | <span data-ttu-id="5564d-110">String</span><span class="sxs-lookup"><span data-stu-id="5564d-110">String</span></span> |
| <span data-ttu-id="5564d-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="5564d-111">storageUsedInBytes</span></span> | <span data-ttu-id="5564d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5564d-112">Int64</span></span>  |
| <span data-ttu-id="5564d-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="5564d-113">reportDate</span></span>         | <span data-ttu-id="5564d-114">Datum</span><span class="sxs-lookup"><span data-stu-id="5564d-114">Date</span></span>   |
| <span data-ttu-id="5564d-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5564d-115">reportPeriod</span></span>       | <span data-ttu-id="5564d-116">String</span><span class="sxs-lookup"><span data-stu-id="5564d-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5564d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5564d-117">JSON representation</span></span>

<span data-ttu-id="5564d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5564d-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
