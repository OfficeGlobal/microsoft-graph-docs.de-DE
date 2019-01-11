---
title: Ressourcentyp skypeForBusinessDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858380"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="ad102-103">Ressourcentyp skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ad102-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ad102-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad102-104">Properties</span></span>

| <span data-ttu-id="ad102-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad102-105">Property</span></span>          | <span data-ttu-id="ad102-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ad102-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="ad102-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ad102-107">reportRefreshDate</span></span> | <span data-ttu-id="ad102-108">Datum</span><span class="sxs-lookup"><span data-stu-id="ad102-108">Date</span></span>    |
| <span data-ttu-id="ad102-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ad102-109">userPrincipalName</span></span> | <span data-ttu-id="ad102-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad102-110">String</span></span>  |
| <span data-ttu-id="ad102-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ad102-111">lastActivityDate</span></span>  | <span data-ttu-id="ad102-112">Datum</span><span class="sxs-lookup"><span data-stu-id="ad102-112">Date</span></span>    |
| <span data-ttu-id="ad102-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="ad102-113">usedWindows</span></span>       | <span data-ttu-id="ad102-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ad102-114">Boolean</span></span> |
| <span data-ttu-id="ad102-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="ad102-115">usedWindowsPhone</span></span>  | <span data-ttu-id="ad102-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ad102-116">Boolean</span></span> |
| <span data-ttu-id="ad102-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="ad102-117">usedAndroidPhone</span></span>  | <span data-ttu-id="ad102-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ad102-118">Boolean</span></span> |
| <span data-ttu-id="ad102-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="ad102-119">usediPhone</span></span>        | <span data-ttu-id="ad102-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ad102-120">Boolean</span></span> |
| <span data-ttu-id="ad102-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="ad102-121">usediPad</span></span>          | <span data-ttu-id="ad102-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ad102-122">Boolean</span></span> |
| <span data-ttu-id="ad102-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ad102-123">reportPeriod</span></span>      | <span data-ttu-id="ad102-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad102-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ad102-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad102-125">JSON representation</span></span>

<span data-ttu-id="ad102-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad102-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
