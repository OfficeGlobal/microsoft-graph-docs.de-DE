---
title: iosMinimumOperatingSystem-Ressourcentyp
description: Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7243b337a53cca31054f99ae807e5c17cdd3e372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876268"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="70602-103">iosMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="70602-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="70602-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="70602-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70602-105">Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="70602-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="70602-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70602-106">Properties</span></span>
|<span data-ttu-id="70602-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70602-107">Property</span></span>|<span data-ttu-id="70602-108">Typ</span><span class="sxs-lookup"><span data-stu-id="70602-108">Type</span></span>|<span data-ttu-id="70602-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70602-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70602-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="70602-110">v8_0</span></span>|<span data-ttu-id="70602-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="70602-111">Boolean</span></span>|<span data-ttu-id="70602-112">Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="70602-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="70602-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="70602-113">v9_0</span></span>|<span data-ttu-id="70602-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="70602-114">Boolean</span></span>|<span data-ttu-id="70602-115">Version 9.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="70602-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="70602-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="70602-116">v10_0</span></span>|<span data-ttu-id="70602-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="70602-117">Boolean</span></span>|<span data-ttu-id="70602-118">Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="70602-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="70602-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="70602-119">v11_0</span></span>|<span data-ttu-id="70602-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="70602-120">Boolean</span></span>|<span data-ttu-id="70602-121">Version 11.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="70602-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="70602-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="70602-122">v12_0</span></span>|<span data-ttu-id="70602-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="70602-123">Boolean</span></span>|<span data-ttu-id="70602-124">Version 12.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="70602-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70602-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="70602-125">Relationships</span></span>
<span data-ttu-id="70602-126">Keine</span><span class="sxs-lookup"><span data-stu-id="70602-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70602-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70602-127">JSON Representation</span></span>
<span data-ttu-id="70602-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70602-128">Here is a JSON representation of the resource.</span></span>
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



