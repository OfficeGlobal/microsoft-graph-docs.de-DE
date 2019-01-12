---
title: Ressourcentyp oneDriveUsageFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7e3a52d082d1acdd2e685008d60e6594615f57a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941023"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="5a041-103">Ressourcentyp oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="5a041-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5a041-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5a041-104">Properties</span></span>

| <span data-ttu-id="5a041-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a041-105">Property</span></span>          | <span data-ttu-id="5a041-106">Typ</span><span class="sxs-lookup"><span data-stu-id="5a041-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5a041-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5a041-107">reportRefreshDate</span></span> | <span data-ttu-id="5a041-108">Datum</span><span class="sxs-lookup"><span data-stu-id="5a041-108">Date</span></span>   |
| <span data-ttu-id="5a041-109">Standorttyp</span><span class="sxs-lookup"><span data-stu-id="5a041-109">siteType</span></span>          | <span data-ttu-id="5a041-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a041-110">String</span></span> |
| <span data-ttu-id="5a041-111">gesamt</span><span class="sxs-lookup"><span data-stu-id="5a041-111">total</span></span>             | <span data-ttu-id="5a041-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5a041-112">Int64</span></span>  |
| <span data-ttu-id="5a041-113">aktive</span><span class="sxs-lookup"><span data-stu-id="5a041-113">active</span></span>            | <span data-ttu-id="5a041-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5a041-114">Int64</span></span>  |
| <span data-ttu-id="5a041-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="5a041-115">reportDate</span></span>        | <span data-ttu-id="5a041-116">Datum</span><span class="sxs-lookup"><span data-stu-id="5a041-116">Date</span></span>   |
| <span data-ttu-id="5a041-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5a041-117">reportPeriod</span></span>      | <span data-ttu-id="5a041-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a041-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a041-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5a041-119">JSON representation</span></span>

<span data-ttu-id="5a041-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5a041-120">The following is a JSON representation of the resource.</span></span>

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
