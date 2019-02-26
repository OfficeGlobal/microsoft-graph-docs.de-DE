---
title: iosMinimumOperatingSystem-Ressourcentyp
description: Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7490ad7b27d55fa6f2b7c6de12083025e7b4ac93
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254569"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="138a3-103">iosMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="138a3-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="138a3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="138a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="138a3-105">Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="138a3-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="138a3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="138a3-106">Properties</span></span>
|<span data-ttu-id="138a3-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="138a3-107">Property</span></span>|<span data-ttu-id="138a3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="138a3-108">Type</span></span>|<span data-ttu-id="138a3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="138a3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="138a3-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="138a3-110">v8_0</span></span>|<span data-ttu-id="138a3-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="138a3-111">Boolean</span></span>|<span data-ttu-id="138a3-112">Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="138a3-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="138a3-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="138a3-113">v9_0</span></span>|<span data-ttu-id="138a3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="138a3-114">Boolean</span></span>|<span data-ttu-id="138a3-115">Version 9.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="138a3-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="138a3-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="138a3-116">v10_0</span></span>|<span data-ttu-id="138a3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="138a3-117">Boolean</span></span>|<span data-ttu-id="138a3-118">Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="138a3-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="138a3-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="138a3-119">v11_0</span></span>|<span data-ttu-id="138a3-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="138a3-120">Boolean</span></span>|<span data-ttu-id="138a3-121">Version 11.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="138a3-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="138a3-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="138a3-122">v12_0</span></span>|<span data-ttu-id="138a3-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="138a3-123">Boolean</span></span>|<span data-ttu-id="138a3-124">Version 12,0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="138a3-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="138a3-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="138a3-125">Relationships</span></span>
<span data-ttu-id="138a3-126">Keine</span><span class="sxs-lookup"><span data-stu-id="138a3-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="138a3-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="138a3-127">JSON Representation</span></span>
<span data-ttu-id="138a3-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="138a3-128">Here is a JSON representation of the resource.</span></span>
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



