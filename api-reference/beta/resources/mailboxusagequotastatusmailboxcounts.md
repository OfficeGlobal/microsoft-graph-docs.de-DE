---
title: Ressourcentyp mailboxUsageQuotaStatusMailboxCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921234"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="c9372-103">Ressourcentyp mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="c9372-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c9372-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9372-104">Properties</span></span>

| <span data-ttu-id="c9372-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9372-105">Property</span></span>              | <span data-ttu-id="c9372-106">Typ</span><span class="sxs-lookup"><span data-stu-id="c9372-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="c9372-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c9372-107">reportRefreshDate</span></span>     | <span data-ttu-id="c9372-108">Datum</span><span class="sxs-lookup"><span data-stu-id="c9372-108">Date</span></span>   |
| <span data-ttu-id="c9372-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="c9372-109">underLimit</span></span>            | <span data-ttu-id="c9372-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c9372-110">Int64</span></span>  |
| <span data-ttu-id="c9372-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="c9372-111">warningIssued</span></span>         | <span data-ttu-id="c9372-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c9372-112">Int64</span></span>  |
| <span data-ttu-id="c9372-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="c9372-113">sendProhibited</span></span>        | <span data-ttu-id="c9372-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c9372-114">Int64</span></span>  |
| <span data-ttu-id="c9372-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="c9372-115">sendReceiveProhibited</span></span> | <span data-ttu-id="c9372-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c9372-116">Int64</span></span>  |
| <span data-ttu-id="c9372-117">unbestimmten</span><span class="sxs-lookup"><span data-stu-id="c9372-117">indeterminate</span></span>         | <span data-ttu-id="c9372-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c9372-118">Int64</span></span>  |
| <span data-ttu-id="c9372-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="c9372-119">reportDate</span></span>            | <span data-ttu-id="c9372-120">Datum</span><span class="sxs-lookup"><span data-stu-id="c9372-120">Date</span></span>   |
| <span data-ttu-id="c9372-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c9372-121">reportPeriod</span></span>          | <span data-ttu-id="c9372-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9372-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9372-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9372-123">JSON representation</span></span>

<span data-ttu-id="c9372-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9372-124">The following is a JSON representation of the resource.</span></span>

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
