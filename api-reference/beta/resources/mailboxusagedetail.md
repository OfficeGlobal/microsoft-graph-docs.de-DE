---
title: Ressourcentyp mailboxUsageDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: af49fac7c6286c7e9f9ce1e6d7ffdede225b4072
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059795"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="383e2-103">Ressourcentyp mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="383e2-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="383e2-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="383e2-104">Properties</span></span>

| <span data-ttu-id="383e2-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="383e2-105">Property</span></span>                        | <span data-ttu-id="383e2-106">Typ</span><span class="sxs-lookup"><span data-stu-id="383e2-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="383e2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="383e2-107">reportRefreshDate</span></span>               | <span data-ttu-id="383e2-108">Datum</span><span class="sxs-lookup"><span data-stu-id="383e2-108">Date</span></span>    |
| <span data-ttu-id="383e2-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="383e2-109">userPrincipalName</span></span>               | <span data-ttu-id="383e2-110">String</span><span class="sxs-lookup"><span data-stu-id="383e2-110">String</span></span>  |
| <span data-ttu-id="383e2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="383e2-111">displayName</span></span>                     | <span data-ttu-id="383e2-112">String</span><span class="sxs-lookup"><span data-stu-id="383e2-112">String</span></span>  |
| <span data-ttu-id="383e2-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="383e2-113">isDeleted</span></span>                       | <span data-ttu-id="383e2-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="383e2-114">Boolean</span></span> |
| <span data-ttu-id="383e2-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="383e2-115">deletedDate</span></span>                     | <span data-ttu-id="383e2-116">Datum</span><span class="sxs-lookup"><span data-stu-id="383e2-116">Date</span></span>    |
| <span data-ttu-id="383e2-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="383e2-117">createdDate</span></span>                     | <span data-ttu-id="383e2-118">Datum</span><span class="sxs-lookup"><span data-stu-id="383e2-118">Date</span></span>    |
| <span data-ttu-id="383e2-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="383e2-119">lastActivityDate</span></span>                | <span data-ttu-id="383e2-120">Datum</span><span class="sxs-lookup"><span data-stu-id="383e2-120">Date</span></span>    |
| <span data-ttu-id="383e2-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="383e2-121">itemCount</span></span>                       | <span data-ttu-id="383e2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="383e2-122">Int64</span></span>   |
| <span data-ttu-id="383e2-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="383e2-123">storageUsedInBytes</span></span>              | <span data-ttu-id="383e2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="383e2-124">Int64</span></span>   |
| <span data-ttu-id="383e2-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="383e2-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="383e2-126">Int64</span><span class="sxs-lookup"><span data-stu-id="383e2-126">Int64</span></span>   |
| <span data-ttu-id="383e2-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="383e2-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="383e2-128">Int64</span><span class="sxs-lookup"><span data-stu-id="383e2-128">Int64</span></span>   |
| <span data-ttu-id="383e2-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="383e2-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="383e2-130">Int64</span><span class="sxs-lookup"><span data-stu-id="383e2-130">Int64</span></span>   |
| <span data-ttu-id="383e2-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="383e2-131">reportPeriod</span></span>                    | <span data-ttu-id="383e2-132">String</span><span class="sxs-lookup"><span data-stu-id="383e2-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="383e2-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="383e2-133">JSON representation</span></span>

<span data-ttu-id="383e2-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="383e2-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
