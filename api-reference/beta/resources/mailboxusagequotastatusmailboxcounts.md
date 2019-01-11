---
title: Ressourcentyp mailboxUsageQuotaStatusMailboxCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835222"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="357ce-103">Ressourcentyp mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="357ce-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="357ce-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="357ce-104">Properties</span></span>

| <span data-ttu-id="357ce-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="357ce-105">Property</span></span>              | <span data-ttu-id="357ce-106">Typ</span><span class="sxs-lookup"><span data-stu-id="357ce-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="357ce-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="357ce-107">reportRefreshDate</span></span>     | <span data-ttu-id="357ce-108">Datum</span><span class="sxs-lookup"><span data-stu-id="357ce-108">Date</span></span>   |
| <span data-ttu-id="357ce-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="357ce-109">underLimit</span></span>            | <span data-ttu-id="357ce-110">Int64</span><span class="sxs-lookup"><span data-stu-id="357ce-110">Int64</span></span>  |
| <span data-ttu-id="357ce-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="357ce-111">warningIssued</span></span>         | <span data-ttu-id="357ce-112">Int64</span><span class="sxs-lookup"><span data-stu-id="357ce-112">Int64</span></span>  |
| <span data-ttu-id="357ce-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="357ce-113">sendProhibited</span></span>        | <span data-ttu-id="357ce-114">Int64</span><span class="sxs-lookup"><span data-stu-id="357ce-114">Int64</span></span>  |
| <span data-ttu-id="357ce-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="357ce-115">sendReceiveProhibited</span></span> | <span data-ttu-id="357ce-116">Int64</span><span class="sxs-lookup"><span data-stu-id="357ce-116">Int64</span></span>  |
| <span data-ttu-id="357ce-117">unbestimmten</span><span class="sxs-lookup"><span data-stu-id="357ce-117">indeterminate</span></span>         | <span data-ttu-id="357ce-118">Int64</span><span class="sxs-lookup"><span data-stu-id="357ce-118">Int64</span></span>  |
| <span data-ttu-id="357ce-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="357ce-119">reportDate</span></span>            | <span data-ttu-id="357ce-120">Datum</span><span class="sxs-lookup"><span data-stu-id="357ce-120">Date</span></span>   |
| <span data-ttu-id="357ce-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="357ce-121">reportPeriod</span></span>          | <span data-ttu-id="357ce-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="357ce-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="357ce-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="357ce-123">JSON representation</span></span>

<span data-ttu-id="357ce-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="357ce-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
