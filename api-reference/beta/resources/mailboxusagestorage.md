---
title: Ressourcentyp mailboxUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: dcabfab0e8a64f2d74442f7d7464708501a59b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840740"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="a60e1-103">Ressourcentyp mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="a60e1-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a60e1-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a60e1-104">Properties</span></span>

| <span data-ttu-id="a60e1-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a60e1-105">Property</span></span>           | <span data-ttu-id="a60e1-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a60e1-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="a60e1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a60e1-107">reportRefreshDate</span></span>  | <span data-ttu-id="a60e1-108">Datum</span><span class="sxs-lookup"><span data-stu-id="a60e1-108">Date</span></span>   |
| <span data-ttu-id="a60e1-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="a60e1-109">storageUsedInBytes</span></span> | <span data-ttu-id="a60e1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a60e1-110">Int64</span></span>  |
| <span data-ttu-id="a60e1-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="a60e1-111">reportDate</span></span>         | <span data-ttu-id="a60e1-112">Datum</span><span class="sxs-lookup"><span data-stu-id="a60e1-112">Date</span></span>   |
| <span data-ttu-id="a60e1-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a60e1-113">reportPeriod</span></span>       | <span data-ttu-id="a60e1-114">String</span><span class="sxs-lookup"><span data-stu-id="a60e1-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a60e1-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a60e1-115">JSON representation</span></span>

<span data-ttu-id="a60e1-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a60e1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
