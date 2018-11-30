---
title: Ressourcentyp mailboxUsageQuotaStatusMailboxCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: ac6c597cad9d28f985da97d6f55a5726ebbf491e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061040"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="0bcf3-103">Ressourcentyp mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="0bcf3-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0bcf3-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0bcf3-104">Properties</span></span>

| <span data-ttu-id="0bcf3-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0bcf3-105">Property</span></span>              | <span data-ttu-id="0bcf3-106">Typ</span><span class="sxs-lookup"><span data-stu-id="0bcf3-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="0bcf3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0bcf3-107">reportRefreshDate</span></span>     | <span data-ttu-id="0bcf3-108">Datum</span><span class="sxs-lookup"><span data-stu-id="0bcf3-108">Date</span></span>   |
| <span data-ttu-id="0bcf3-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="0bcf3-109">underLimit</span></span>            | <span data-ttu-id="0bcf3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="0bcf3-110">Int64</span></span>  |
| <span data-ttu-id="0bcf3-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="0bcf3-111">warningIssued</span></span>         | <span data-ttu-id="0bcf3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0bcf3-112">Int64</span></span>  |
| <span data-ttu-id="0bcf3-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="0bcf3-113">sendProhibited</span></span>        | <span data-ttu-id="0bcf3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0bcf3-114">Int64</span></span>  |
| <span data-ttu-id="0bcf3-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="0bcf3-115">sendReceiveProhibited</span></span> | <span data-ttu-id="0bcf3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0bcf3-116">Int64</span></span>  |
| <span data-ttu-id="0bcf3-117">unbestimmten</span><span class="sxs-lookup"><span data-stu-id="0bcf3-117">indeterminate</span></span>         | <span data-ttu-id="0bcf3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0bcf3-118">Int64</span></span>  |
| <span data-ttu-id="0bcf3-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="0bcf3-119">reportDate</span></span>            | <span data-ttu-id="0bcf3-120">Datum</span><span class="sxs-lookup"><span data-stu-id="0bcf3-120">Date</span></span>   |
| <span data-ttu-id="0bcf3-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0bcf3-121">reportPeriod</span></span>          | <span data-ttu-id="0bcf3-122">String</span><span class="sxs-lookup"><span data-stu-id="0bcf3-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0bcf3-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0bcf3-123">JSON representation</span></span>

<span data-ttu-id="0bcf3-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0bcf3-124">The following is a JSON representation of the resource.</span></span>

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
