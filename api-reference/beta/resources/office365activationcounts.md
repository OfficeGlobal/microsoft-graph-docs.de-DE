---
title: Ressourcentyp office365ActivationCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: e53a979ac627735ef63a24e1823d83f4c9fe9f7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064760"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="2e9e6-103">Ressourcentyp office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="2e9e6-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2e9e6-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e9e6-104">Properties</span></span>

| <span data-ttu-id="2e9e6-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e9e6-105">Property</span></span>          | <span data-ttu-id="2e9e6-106">Typ</span><span class="sxs-lookup"><span data-stu-id="2e9e6-106">Type</span></span>   | <span data-ttu-id="2e9e6-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e9e6-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2e9e6-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2e9e6-108">reportRefreshDate</span></span> | <span data-ttu-id="2e9e6-109">Datum</span><span class="sxs-lookup"><span data-stu-id="2e9e6-109">Date</span></span>   | <span data-ttu-id="2e9e6-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2e9e6-111">productType</span><span class="sxs-lookup"><span data-stu-id="2e9e6-111">productType</span></span>       | <span data-ttu-id="2e9e6-112">String</span><span class="sxs-lookup"><span data-stu-id="2e9e6-112">String</span></span> | <span data-ttu-id="2e9e6-113">Produkttyp, beispielsweise "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365".</span><span class="sxs-lookup"><span data-stu-id="2e9e6-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="2e9e6-114">Windows</span><span class="sxs-lookup"><span data-stu-id="2e9e6-114">windows</span></span>           | <span data-ttu-id="2e9e6-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2e9e6-115">Int64</span></span>  | <span data-ttu-id="2e9e6-116">Die Anzahl der Aktivierung auf Windows.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-116">The activation count on Windows.</span></span> <span data-ttu-id="2e9e6-117">Dieser Wert schließt alle Aktivierung auf einem beliebigen Windows-Computer.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="2e9e6-118">mac</span><span class="sxs-lookup"><span data-stu-id="2e9e6-118">mac</span></span>               | <span data-ttu-id="2e9e6-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2e9e6-119">Int64</span></span>  | <span data-ttu-id="2e9e6-120">Die Anzahl der Aktivierung auf Mac OS.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="2e9e6-121">Android (engl.)</span><span class="sxs-lookup"><span data-stu-id="2e9e6-121">android</span></span>           | <span data-ttu-id="2e9e6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2e9e6-122">Int64</span></span>  | <span data-ttu-id="2e9e6-123">Die Anzahl der Aktivierung auf einer Android-Gerät.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="2e9e6-124">IOS</span><span class="sxs-lookup"><span data-stu-id="2e9e6-124">ios</span></span>               | <span data-ttu-id="2e9e6-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2e9e6-125">Int64</span></span>  | <span data-ttu-id="2e9e6-126">Die Anzahl der Aktivierung auf iOS.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="2e9e6-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="2e9e6-127">windows10Mobile</span></span>   | <span data-ttu-id="2e9e6-128">Int64</span><span class="sxs-lookup"><span data-stu-id="2e9e6-128">Int64</span></span>  | <span data-ttu-id="2e9e6-129">Die Aktivierung zählen auf 10 für Windows mobile.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e9e6-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e9e6-130">JSON representation</span></span>

<span data-ttu-id="2e9e6-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e9e6-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
