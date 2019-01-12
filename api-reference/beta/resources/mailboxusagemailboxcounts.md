---
title: Ressourcentyp mailboxUsageMailboxCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e9da6a72c3c2d79323041e683702a7af2e4699c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941310"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="7de32-103">Ressourcentyp mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="7de32-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7de32-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7de32-104">Properties</span></span>

| <span data-ttu-id="7de32-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7de32-105">Property</span></span>          | <span data-ttu-id="7de32-106">Typ</span><span class="sxs-lookup"><span data-stu-id="7de32-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7de32-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7de32-107">reportRefreshDate</span></span> | <span data-ttu-id="7de32-108">Datum</span><span class="sxs-lookup"><span data-stu-id="7de32-108">Date</span></span>   |
| <span data-ttu-id="7de32-109">gesamt</span><span class="sxs-lookup"><span data-stu-id="7de32-109">total</span></span>             | <span data-ttu-id="7de32-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7de32-110">Int64</span></span>  |
| <span data-ttu-id="7de32-111">aktive</span><span class="sxs-lookup"><span data-stu-id="7de32-111">active</span></span>            | <span data-ttu-id="7de32-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7de32-112">Int64</span></span>  |
| <span data-ttu-id="7de32-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="7de32-113">reportDate</span></span>        | <span data-ttu-id="7de32-114">Datum</span><span class="sxs-lookup"><span data-stu-id="7de32-114">Date</span></span>   |
| <span data-ttu-id="7de32-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7de32-115">reportPeriod</span></span>      | <span data-ttu-id="7de32-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7de32-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7de32-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7de32-117">JSON representation</span></span>

<span data-ttu-id="7de32-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7de32-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
