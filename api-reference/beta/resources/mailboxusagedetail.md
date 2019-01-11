---
title: Ressourcentyp mailboxUsageDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 25cb41e38138a677bfc6636b035003bb8fc5858c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818011"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="8584a-103">Ressourcentyp mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="8584a-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8584a-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8584a-104">Properties</span></span>

| <span data-ttu-id="8584a-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8584a-105">Property</span></span>                        | <span data-ttu-id="8584a-106">Typ</span><span class="sxs-lookup"><span data-stu-id="8584a-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="8584a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8584a-107">reportRefreshDate</span></span>               | <span data-ttu-id="8584a-108">Datum</span><span class="sxs-lookup"><span data-stu-id="8584a-108">Date</span></span>    |
| <span data-ttu-id="8584a-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8584a-109">userPrincipalName</span></span>               | <span data-ttu-id="8584a-110">String</span><span class="sxs-lookup"><span data-stu-id="8584a-110">String</span></span>  |
| <span data-ttu-id="8584a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8584a-111">displayName</span></span>                     | <span data-ttu-id="8584a-112">String</span><span class="sxs-lookup"><span data-stu-id="8584a-112">String</span></span>  |
| <span data-ttu-id="8584a-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8584a-113">isDeleted</span></span>                       | <span data-ttu-id="8584a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8584a-114">Boolean</span></span> |
| <span data-ttu-id="8584a-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8584a-115">deletedDate</span></span>                     | <span data-ttu-id="8584a-116">Datum</span><span class="sxs-lookup"><span data-stu-id="8584a-116">Date</span></span>    |
| <span data-ttu-id="8584a-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="8584a-117">createdDate</span></span>                     | <span data-ttu-id="8584a-118">Datum</span><span class="sxs-lookup"><span data-stu-id="8584a-118">Date</span></span>    |
| <span data-ttu-id="8584a-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8584a-119">lastActivityDate</span></span>                | <span data-ttu-id="8584a-120">Datum</span><span class="sxs-lookup"><span data-stu-id="8584a-120">Date</span></span>    |
| <span data-ttu-id="8584a-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="8584a-121">itemCount</span></span>                       | <span data-ttu-id="8584a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8584a-122">Int64</span></span>   |
| <span data-ttu-id="8584a-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="8584a-123">storageUsedInBytes</span></span>              | <span data-ttu-id="8584a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8584a-124">Int64</span></span>   |
| <span data-ttu-id="8584a-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="8584a-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="8584a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8584a-126">Int64</span></span>   |
| <span data-ttu-id="8584a-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="8584a-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="8584a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="8584a-128">Int64</span></span>   |
| <span data-ttu-id="8584a-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="8584a-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="8584a-130">Int64</span><span class="sxs-lookup"><span data-stu-id="8584a-130">Int64</span></span>   |
| <span data-ttu-id="8584a-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8584a-131">reportPeriod</span></span>                    | <span data-ttu-id="8584a-132">String</span><span class="sxs-lookup"><span data-stu-id="8584a-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8584a-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8584a-133">JSON representation</span></span>

<span data-ttu-id="8584a-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8584a-134">The following is a JSON representation of the resource.</span></span>

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
