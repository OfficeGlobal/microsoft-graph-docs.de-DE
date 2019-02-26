---
title: deliveryOptimizationBandwidthHoursWithPercentage-Ressourcentyp
description: Bandbreiten Grenzwert als Prozentsatz der Geschäftszeiten.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fb4fa251e9f1cb936da0ada158050df42e0aab6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178241"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="507b4-103">deliveryOptimizationBandwidthHoursWithPercentage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="507b4-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="507b4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="507b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="507b4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="507b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="507b4-106">Bandbreiten Grenzwert als Prozentsatz der Geschäftszeiten.</span><span class="sxs-lookup"><span data-stu-id="507b4-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="507b4-107">Erbt von [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="507b4-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="507b4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="507b4-108">Properties</span></span>
|<span data-ttu-id="507b4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="507b4-109">Property</span></span>|<span data-ttu-id="507b4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="507b4-110">Type</span></span>|<span data-ttu-id="507b4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="507b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="507b4-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="507b4-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="507b4-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="507b4-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="507b4-114">Prozentuale Anzahl der Hintergrund Downloads.</span><span class="sxs-lookup"><span data-stu-id="507b4-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="507b4-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="507b4-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="507b4-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="507b4-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="507b4-117">Vordergrund Download prozentuale Stunden.</span><span class="sxs-lookup"><span data-stu-id="507b4-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="507b4-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="507b4-118">Relationships</span></span>
<span data-ttu-id="507b4-119">Keine</span><span class="sxs-lookup"><span data-stu-id="507b4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="507b4-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="507b4-120">JSON Representation</span></span>
<span data-ttu-id="507b4-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="507b4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  }
}
```




