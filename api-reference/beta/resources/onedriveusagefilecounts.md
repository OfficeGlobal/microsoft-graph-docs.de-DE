---
title: Ressourcentyp oneDriveUsageFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: ec428179cb35755e545aded70929eccd9d558fec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829533"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="d3508-103">Ressourcentyp oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="d3508-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d3508-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3508-104">Properties</span></span>

| <span data-ttu-id="d3508-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3508-105">Property</span></span>          | <span data-ttu-id="d3508-106">Typ</span><span class="sxs-lookup"><span data-stu-id="d3508-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d3508-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d3508-107">reportRefreshDate</span></span> | <span data-ttu-id="d3508-108">Datum</span><span class="sxs-lookup"><span data-stu-id="d3508-108">Date</span></span>   |
| <span data-ttu-id="d3508-109">Standorttyp</span><span class="sxs-lookup"><span data-stu-id="d3508-109">siteType</span></span>          | <span data-ttu-id="d3508-110">String</span><span class="sxs-lookup"><span data-stu-id="d3508-110">String</span></span> |
| <span data-ttu-id="d3508-111">gesamt</span><span class="sxs-lookup"><span data-stu-id="d3508-111">total</span></span>             | <span data-ttu-id="d3508-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d3508-112">Int64</span></span>  |
| <span data-ttu-id="d3508-113">aktive</span><span class="sxs-lookup"><span data-stu-id="d3508-113">active</span></span>            | <span data-ttu-id="d3508-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d3508-114">Int64</span></span>  |
| <span data-ttu-id="d3508-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="d3508-115">reportDate</span></span>        | <span data-ttu-id="d3508-116">Datum</span><span class="sxs-lookup"><span data-stu-id="d3508-116">Date</span></span>   |
| <span data-ttu-id="d3508-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d3508-117">reportPeriod</span></span>      | <span data-ttu-id="d3508-118">String</span><span class="sxs-lookup"><span data-stu-id="d3508-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3508-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d3508-119">JSON representation</span></span>

<span data-ttu-id="d3508-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d3508-120">The following is a JSON representation of the resource.</span></span>

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
