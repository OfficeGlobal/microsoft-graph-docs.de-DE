---
title: Ressourcentyp userActivationCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: cae194545f13d312ee78b572659017752e43a6a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845290"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="96461-103">Ressourcentyp userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="96461-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="96461-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96461-104">Properties</span></span>

| <span data-ttu-id="96461-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96461-105">Property</span></span>          | <span data-ttu-id="96461-106">Typ</span><span class="sxs-lookup"><span data-stu-id="96461-106">Type</span></span>   | <span data-ttu-id="96461-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96461-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="96461-108">productType</span><span class="sxs-lookup"><span data-stu-id="96461-108">productType</span></span>       | <span data-ttu-id="96461-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96461-109">String</span></span> | <span data-ttu-id="96461-110">Produkttyp, beispielsweise "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365".</span><span class="sxs-lookup"><span data-stu-id="96461-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="96461-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="96461-111">lastActivatedDate</span></span> | <span data-ttu-id="96461-112">Datum</span><span class="sxs-lookup"><span data-stu-id="96461-112">Date</span></span>   | <span data-ttu-id="96461-113">Das Datum der neuesten Aktivierung.</span><span class="sxs-lookup"><span data-stu-id="96461-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="96461-114">Windows</span><span class="sxs-lookup"><span data-stu-id="96461-114">windows</span></span>           | <span data-ttu-id="96461-115">Int64</span><span class="sxs-lookup"><span data-stu-id="96461-115">Int64</span></span>  | <span data-ttu-id="96461-116">Die Anzahl der Aktivierung auf Windows.</span><span class="sxs-lookup"><span data-stu-id="96461-116">The activation count on Windows.</span></span> <span data-ttu-id="96461-117">Dieser Wert schließt alle Aktivierung auf einem beliebigen Windows-Computer.</span><span class="sxs-lookup"><span data-stu-id="96461-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="96461-118">mac</span><span class="sxs-lookup"><span data-stu-id="96461-118">mac</span></span>               | <span data-ttu-id="96461-119">Int64</span><span class="sxs-lookup"><span data-stu-id="96461-119">Int64</span></span>  | <span data-ttu-id="96461-120">Die Anzahl der Aktivierung auf Mac OS.</span><span class="sxs-lookup"><span data-stu-id="96461-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="96461-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="96461-121">windows10Mobile</span></span>   | <span data-ttu-id="96461-122">Int64</span><span class="sxs-lookup"><span data-stu-id="96461-122">Int64</span></span>  | <span data-ttu-id="96461-123">Die Aktivierung zählen auf 10 für Windows mobile.</span><span class="sxs-lookup"><span data-stu-id="96461-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="96461-124">IOS</span><span class="sxs-lookup"><span data-stu-id="96461-124">ios</span></span>               | <span data-ttu-id="96461-125">Int64</span><span class="sxs-lookup"><span data-stu-id="96461-125">Int64</span></span>  | <span data-ttu-id="96461-126">Die Anzahl der Aktivierung auf iOS.</span><span class="sxs-lookup"><span data-stu-id="96461-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="96461-127">Android (engl.)</span><span class="sxs-lookup"><span data-stu-id="96461-127">android</span></span>           | <span data-ttu-id="96461-128">Int64</span><span class="sxs-lookup"><span data-stu-id="96461-128">Int64</span></span>  | <span data-ttu-id="96461-129">Die Anzahl der Aktivierung auf einer Android-Gerät.</span><span class="sxs-lookup"><span data-stu-id="96461-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="96461-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="96461-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="96461-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="96461-131">Boolean</span></span> | <span data-ttu-id="96461-132">True, wenn der Benutzer das Produkt auf einem freigegebenen Computer vor verwendet.</span><span class="sxs-lookup"><span data-stu-id="96461-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96461-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96461-133">JSON representation</span></span>

<span data-ttu-id="96461-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96461-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```
