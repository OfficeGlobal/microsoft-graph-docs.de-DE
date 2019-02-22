---
title: deliveryOptimizationMaxCacheSizePercentage-Ressourcentyp
description: Maximale Anzahl von Cachegrößen für die Verteilungs Optimierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7579b95d0adefb09c9312596f4604fe9d5b05548
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177833"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="aff55-103">deliveryOptimizationMaxCacheSizePercentage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aff55-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

> <span data-ttu-id="aff55-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aff55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aff55-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="aff55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aff55-106">Maximale Anzahl von Cachegrößen für die Verteilungs Optimierung.</span><span class="sxs-lookup"><span data-stu-id="aff55-106">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="aff55-107">Erbt von [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="aff55-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aff55-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aff55-108">Properties</span></span>
|<span data-ttu-id="aff55-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aff55-109">Property</span></span>|<span data-ttu-id="aff55-110">Typ</span><span class="sxs-lookup"><span data-stu-id="aff55-110">Type</span></span>|<span data-ttu-id="aff55-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aff55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff55-112">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="aff55-112">maximumCacheSizePercentage</span></span>|<span data-ttu-id="aff55-113">Int32</span><span class="sxs-lookup"><span data-stu-id="aff55-113">Int32</span></span>|<span data-ttu-id="aff55-114">Gibt die maximale Cachegröße, die von der BereitstellungsOptimierung verwendet werden kann, als Prozentsatz der Datenträgergröße an (1-100).</span><span class="sxs-lookup"><span data-stu-id="aff55-114">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="aff55-115">Gültige Werte 1 bis 100</span><span class="sxs-lookup"><span data-stu-id="aff55-115">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="aff55-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aff55-116">Relationships</span></span>
<span data-ttu-id="aff55-117">Keine</span><span class="sxs-lookup"><span data-stu-id="aff55-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aff55-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aff55-118">JSON Representation</span></span>
<span data-ttu-id="aff55-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aff55-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```




