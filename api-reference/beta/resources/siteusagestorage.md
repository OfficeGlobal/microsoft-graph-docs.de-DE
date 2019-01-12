---
title: Ressourcentyp siteUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928101"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="80243-103">Ressourcentyp siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="80243-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="80243-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80243-104">Properties</span></span>

| <span data-ttu-id="80243-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80243-105">Property</span></span>           | <span data-ttu-id="80243-106">Typ</span><span class="sxs-lookup"><span data-stu-id="80243-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="80243-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="80243-107">reportRefreshDate</span></span>  | <span data-ttu-id="80243-108">Datum</span><span class="sxs-lookup"><span data-stu-id="80243-108">Date</span></span>   |
| <span data-ttu-id="80243-109">Standorttyp</span><span class="sxs-lookup"><span data-stu-id="80243-109">siteType</span></span>           | <span data-ttu-id="80243-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80243-110">String</span></span> |
| <span data-ttu-id="80243-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="80243-111">storageUsedInBytes</span></span> | <span data-ttu-id="80243-112">Int64</span><span class="sxs-lookup"><span data-stu-id="80243-112">Int64</span></span>  |
| <span data-ttu-id="80243-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="80243-113">reportDate</span></span>         | <span data-ttu-id="80243-114">Datum</span><span class="sxs-lookup"><span data-stu-id="80243-114">Date</span></span>   |
| <span data-ttu-id="80243-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="80243-115">reportPeriod</span></span>       | <span data-ttu-id="80243-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80243-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80243-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80243-117">JSON representation</span></span>

<span data-ttu-id="80243-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80243-118">The following is a JSON representation of the resource.</span></span>

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
