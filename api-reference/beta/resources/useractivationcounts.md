---
title: Ressourcentyp userActivationCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 022b73310a54877889efebabbb6e8fc4ab71fb65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061139"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="9094b-103">Ressourcentyp userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="9094b-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9094b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9094b-104">Properties</span></span>

| <span data-ttu-id="9094b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9094b-105">Property</span></span>          | <span data-ttu-id="9094b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="9094b-106">Type</span></span>   | <span data-ttu-id="9094b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9094b-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="9094b-108">productType</span><span class="sxs-lookup"><span data-stu-id="9094b-108">productType</span></span>       | <span data-ttu-id="9094b-109">String</span><span class="sxs-lookup"><span data-stu-id="9094b-109">String</span></span> | <span data-ttu-id="9094b-110">Produkttyp, beispielsweise "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365".</span><span class="sxs-lookup"><span data-stu-id="9094b-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="9094b-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="9094b-111">lastActivatedDate</span></span> | <span data-ttu-id="9094b-112">Datum</span><span class="sxs-lookup"><span data-stu-id="9094b-112">Date</span></span>   | <span data-ttu-id="9094b-113">Das Datum der neuesten Aktivierung.</span><span class="sxs-lookup"><span data-stu-id="9094b-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="9094b-114">Windows</span><span class="sxs-lookup"><span data-stu-id="9094b-114">windows</span></span>           | <span data-ttu-id="9094b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9094b-115">Int64</span></span>  | <span data-ttu-id="9094b-116">Die Anzahl der Aktivierung auf Windows.</span><span class="sxs-lookup"><span data-stu-id="9094b-116">The activation count on Windows.</span></span> <span data-ttu-id="9094b-117">Dieser Wert schließt alle Aktivierung auf einem beliebigen Windows-Computer.</span><span class="sxs-lookup"><span data-stu-id="9094b-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="9094b-118">mac</span><span class="sxs-lookup"><span data-stu-id="9094b-118">mac</span></span>               | <span data-ttu-id="9094b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="9094b-119">Int64</span></span>  | <span data-ttu-id="9094b-120">Die Anzahl der Aktivierung auf Mac OS.</span><span class="sxs-lookup"><span data-stu-id="9094b-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="9094b-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="9094b-121">windows10Mobile</span></span>   | <span data-ttu-id="9094b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9094b-122">Int64</span></span>  | <span data-ttu-id="9094b-123">Die Aktivierung zählen auf 10 für Windows mobile.</span><span class="sxs-lookup"><span data-stu-id="9094b-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="9094b-124">IOS</span><span class="sxs-lookup"><span data-stu-id="9094b-124">ios</span></span>               | <span data-ttu-id="9094b-125">Int64</span><span class="sxs-lookup"><span data-stu-id="9094b-125">Int64</span></span>  | <span data-ttu-id="9094b-126">Die Anzahl der Aktivierung auf iOS.</span><span class="sxs-lookup"><span data-stu-id="9094b-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="9094b-127">Android (engl.)</span><span class="sxs-lookup"><span data-stu-id="9094b-127">android</span></span>           | <span data-ttu-id="9094b-128">Int64</span><span class="sxs-lookup"><span data-stu-id="9094b-128">Int64</span></span>  | <span data-ttu-id="9094b-129">Die Anzahl der Aktivierung auf einer Android-Gerät.</span><span class="sxs-lookup"><span data-stu-id="9094b-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="9094b-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="9094b-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="9094b-131">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9094b-131">Boolean</span></span> | <span data-ttu-id="9094b-132">True, wenn der Benutzer das Produkt auf einem freigegebenen Computer vor verwendet.</span><span class="sxs-lookup"><span data-stu-id="9094b-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9094b-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9094b-133">JSON representation</span></span>

<span data-ttu-id="9094b-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9094b-134">The following is a JSON representation of the resource.</span></span>

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
