---
title: Ressourcentyp mailboxUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 8cc26c5d3cc30529857ed3273f8ee66c7373327a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059837"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="53913-103">Ressourcentyp mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="53913-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="53913-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="53913-104">Properties</span></span>

| <span data-ttu-id="53913-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53913-105">Property</span></span>           | <span data-ttu-id="53913-106">Typ</span><span class="sxs-lookup"><span data-stu-id="53913-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="53913-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="53913-107">reportRefreshDate</span></span>  | <span data-ttu-id="53913-108">Datum</span><span class="sxs-lookup"><span data-stu-id="53913-108">Date</span></span>   |
| <span data-ttu-id="53913-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="53913-109">storageUsedInBytes</span></span> | <span data-ttu-id="53913-110">Int64</span><span class="sxs-lookup"><span data-stu-id="53913-110">Int64</span></span>  |
| <span data-ttu-id="53913-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="53913-111">reportDate</span></span>         | <span data-ttu-id="53913-112">Datum</span><span class="sxs-lookup"><span data-stu-id="53913-112">Date</span></span>   |
| <span data-ttu-id="53913-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="53913-113">reportPeriod</span></span>       | <span data-ttu-id="53913-114">String</span><span class="sxs-lookup"><span data-stu-id="53913-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53913-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="53913-115">JSON representation</span></span>

<span data-ttu-id="53913-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="53913-116">The following is a JSON representation of the resource.</span></span>

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
