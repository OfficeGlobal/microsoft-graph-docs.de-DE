---
title: Ressourcentyp siteUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 1f656feacdbba3418049bd9f3072270aa04af798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879926"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="7fdc6-103">Ressourcentyp siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="7fdc6-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7fdc6-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7fdc6-104">Properties</span></span>

| <span data-ttu-id="7fdc6-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7fdc6-105">Property</span></span>           | <span data-ttu-id="7fdc6-106">Typ</span><span class="sxs-lookup"><span data-stu-id="7fdc6-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="7fdc6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7fdc6-107">reportRefreshDate</span></span>  | <span data-ttu-id="7fdc6-108">Datum</span><span class="sxs-lookup"><span data-stu-id="7fdc6-108">Date</span></span>   |
| <span data-ttu-id="7fdc6-109">Standorttyp</span><span class="sxs-lookup"><span data-stu-id="7fdc6-109">siteType</span></span>           | <span data-ttu-id="7fdc6-110">String</span><span class="sxs-lookup"><span data-stu-id="7fdc6-110">String</span></span> |
| <span data-ttu-id="7fdc6-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="7fdc6-111">storageUsedInBytes</span></span> | <span data-ttu-id="7fdc6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7fdc6-112">Int64</span></span>  |
| <span data-ttu-id="7fdc6-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="7fdc6-113">reportDate</span></span>         | <span data-ttu-id="7fdc6-114">Datum</span><span class="sxs-lookup"><span data-stu-id="7fdc6-114">Date</span></span>   |
| <span data-ttu-id="7fdc6-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7fdc6-115">reportPeriod</span></span>       | <span data-ttu-id="7fdc6-116">String</span><span class="sxs-lookup"><span data-stu-id="7fdc6-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7fdc6-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7fdc6-117">JSON representation</span></span>

<span data-ttu-id="7fdc6-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7fdc6-118">The following is a JSON representation of the resource.</span></span>

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
