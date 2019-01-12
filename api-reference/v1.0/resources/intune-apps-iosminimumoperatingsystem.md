---
title: iosMinimumOperatingSystem-Ressourcentyp
description: Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a80de09abe7e5fb513c95006f6b2c2fe719a4f39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925938"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="681b4-103">iosMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="681b4-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="681b4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="681b4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="681b4-105">Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="681b4-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="681b4-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="681b4-106">Properties</span></span>
|<span data-ttu-id="681b4-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="681b4-107">Property</span></span>|<span data-ttu-id="681b4-108">Typ</span><span class="sxs-lookup"><span data-stu-id="681b4-108">Type</span></span>|<span data-ttu-id="681b4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="681b4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="681b4-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="681b4-110">v8_0</span></span>|<span data-ttu-id="681b4-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="681b4-111">Boolean</span></span>|<span data-ttu-id="681b4-112">Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="681b4-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="681b4-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="681b4-113">v9_0</span></span>|<span data-ttu-id="681b4-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="681b4-114">Boolean</span></span>|<span data-ttu-id="681b4-115">Version 9.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="681b4-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="681b4-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="681b4-116">v10_0</span></span>|<span data-ttu-id="681b4-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="681b4-117">Boolean</span></span>|<span data-ttu-id="681b4-118">Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="681b4-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="681b4-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="681b4-119">v11_0</span></span>|<span data-ttu-id="681b4-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="681b4-120">Boolean</span></span>|<span data-ttu-id="681b4-121">Version 11.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="681b4-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="681b4-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="681b4-122">v12_0</span></span>|<span data-ttu-id="681b4-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="681b4-123">Boolean</span></span>|<span data-ttu-id="681b4-124">Version 12.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="681b4-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="681b4-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="681b4-125">Relationships</span></span>
<span data-ttu-id="681b4-126">Keine</span><span class="sxs-lookup"><span data-stu-id="681b4-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="681b4-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="681b4-127">JSON Representation</span></span>
<span data-ttu-id="681b4-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="681b4-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



