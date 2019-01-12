---
title: Ressourcentyp mailboxUsageDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63b4b997a0ae559338fffd2acfabaa35dcc306e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938734"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="1f210-103">Ressourcentyp mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="1f210-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1f210-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1f210-104">Properties</span></span>

| <span data-ttu-id="1f210-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f210-105">Property</span></span>                        | <span data-ttu-id="1f210-106">Typ</span><span class="sxs-lookup"><span data-stu-id="1f210-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="1f210-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1f210-107">reportRefreshDate</span></span>               | <span data-ttu-id="1f210-108">Datum</span><span class="sxs-lookup"><span data-stu-id="1f210-108">Date</span></span>    |
| <span data-ttu-id="1f210-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1f210-109">userPrincipalName</span></span>               | <span data-ttu-id="1f210-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f210-110">String</span></span>  |
| <span data-ttu-id="1f210-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1f210-111">displayName</span></span>                     | <span data-ttu-id="1f210-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f210-112">String</span></span>  |
| <span data-ttu-id="1f210-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1f210-113">isDeleted</span></span>                       | <span data-ttu-id="1f210-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1f210-114">Boolean</span></span> |
| <span data-ttu-id="1f210-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="1f210-115">deletedDate</span></span>                     | <span data-ttu-id="1f210-116">Datum</span><span class="sxs-lookup"><span data-stu-id="1f210-116">Date</span></span>    |
| <span data-ttu-id="1f210-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="1f210-117">createdDate</span></span>                     | <span data-ttu-id="1f210-118">Datum</span><span class="sxs-lookup"><span data-stu-id="1f210-118">Date</span></span>    |
| <span data-ttu-id="1f210-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1f210-119">lastActivityDate</span></span>                | <span data-ttu-id="1f210-120">Datum</span><span class="sxs-lookup"><span data-stu-id="1f210-120">Date</span></span>    |
| <span data-ttu-id="1f210-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="1f210-121">itemCount</span></span>                       | <span data-ttu-id="1f210-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1f210-122">Int64</span></span>   |
| <span data-ttu-id="1f210-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="1f210-123">storageUsedInBytes</span></span>              | <span data-ttu-id="1f210-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1f210-124">Int64</span></span>   |
| <span data-ttu-id="1f210-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="1f210-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="1f210-126">Int64</span><span class="sxs-lookup"><span data-stu-id="1f210-126">Int64</span></span>   |
| <span data-ttu-id="1f210-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="1f210-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="1f210-128">Int64</span><span class="sxs-lookup"><span data-stu-id="1f210-128">Int64</span></span>   |
| <span data-ttu-id="1f210-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="1f210-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="1f210-130">Int64</span><span class="sxs-lookup"><span data-stu-id="1f210-130">Int64</span></span>   |
| <span data-ttu-id="1f210-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1f210-131">reportPeriod</span></span>                    | <span data-ttu-id="1f210-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f210-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1f210-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1f210-133">JSON representation</span></span>

<span data-ttu-id="1f210-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1f210-134">The following is a JSON representation of the resource.</span></span>

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
