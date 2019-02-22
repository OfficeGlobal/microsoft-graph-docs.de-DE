---
title: deliveryOptimizationMaxCacheSizeAbsolute-Ressourcentyp
description: Verteilungs Optimierung maximale Cachegröße.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e1ff180136804d6a98e2ebbb292acc358d908d6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178129"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="4a4c3-103">deliveryOptimizationMaxCacheSizeAbsolute-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4a4c3-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

> <span data-ttu-id="4a4c3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a4c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a4c3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4a4c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a4c3-106">Verteilungs Optimierung maximale Cachegröße.</span><span class="sxs-lookup"><span data-stu-id="4a4c3-106">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="4a4c3-107">Erbt von [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="4a4c3-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a4c3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4a4c3-108">Properties</span></span>
|<span data-ttu-id="4a4c3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a4c3-109">Property</span></span>|<span data-ttu-id="4a4c3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4a4c3-110">Type</span></span>|<span data-ttu-id="4a4c3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a4c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a4c3-112">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="4a4c3-112">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="4a4c3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="4a4c3-113">Int64</span></span>|<span data-ttu-id="4a4c3-114">Gibt die maximale Größe des Caches für die Verteilungs Optimierung in GB an.</span><span class="sxs-lookup"><span data-stu-id="4a4c3-114">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="4a4c3-115">Gültige Werte 0 bis 4294967295</span><span class="sxs-lookup"><span data-stu-id="4a4c3-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="4a4c3-116">Der Wert 0 (null) steht für "unbegrenzten" Cache.</span><span class="sxs-lookup"><span data-stu-id="4a4c3-116">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="4a4c3-117">Durch die BereitstellungsOptimierung wird der Cache gelöscht, wenn auf dem Gerät wenig Speicherplatz zur Verfügung steht.</span><span class="sxs-lookup"><span data-stu-id="4a4c3-117">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="4a4c3-118">Gültige Werte 0 bis 4294967295</span><span class="sxs-lookup"><span data-stu-id="4a4c3-118">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a4c3-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4a4c3-119">Relationships</span></span>
<span data-ttu-id="4a4c3-120">Keine</span><span class="sxs-lookup"><span data-stu-id="4a4c3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a4c3-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4a4c3-121">JSON Representation</span></span>
<span data-ttu-id="4a4c3-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4a4c3-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```




