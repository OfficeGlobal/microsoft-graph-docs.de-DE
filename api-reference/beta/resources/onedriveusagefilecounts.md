---
title: Ressourcentyp oneDriveUsageFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 98e387b97687a4aab55e8d94e72fdbfa585a0e84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059050"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="7bfad-103">Ressourcentyp oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="7bfad-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7bfad-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7bfad-104">Properties</span></span>

| <span data-ttu-id="7bfad-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7bfad-105">Property</span></span>          | <span data-ttu-id="7bfad-106">Typ</span><span class="sxs-lookup"><span data-stu-id="7bfad-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7bfad-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7bfad-107">reportRefreshDate</span></span> | <span data-ttu-id="7bfad-108">Datum</span><span class="sxs-lookup"><span data-stu-id="7bfad-108">Date</span></span>   |
| <span data-ttu-id="7bfad-109">Standorttyp</span><span class="sxs-lookup"><span data-stu-id="7bfad-109">siteType</span></span>          | <span data-ttu-id="7bfad-110">String</span><span class="sxs-lookup"><span data-stu-id="7bfad-110">String</span></span> |
| <span data-ttu-id="7bfad-111">gesamt</span><span class="sxs-lookup"><span data-stu-id="7bfad-111">total</span></span>             | <span data-ttu-id="7bfad-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7bfad-112">Int64</span></span>  |
| <span data-ttu-id="7bfad-113">aktive</span><span class="sxs-lookup"><span data-stu-id="7bfad-113">active</span></span>            | <span data-ttu-id="7bfad-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7bfad-114">Int64</span></span>  |
| <span data-ttu-id="7bfad-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="7bfad-115">reportDate</span></span>        | <span data-ttu-id="7bfad-116">Datum</span><span class="sxs-lookup"><span data-stu-id="7bfad-116">Date</span></span>   |
| <span data-ttu-id="7bfad-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7bfad-117">reportPeriod</span></span>      | <span data-ttu-id="7bfad-118">String</span><span class="sxs-lookup"><span data-stu-id="7bfad-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7bfad-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7bfad-119">JSON representation</span></span>

<span data-ttu-id="7bfad-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7bfad-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
