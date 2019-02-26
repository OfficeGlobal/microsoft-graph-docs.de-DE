---
title: deliveryOptimizationBandwidthPercentage-Ressourcentyp
description: Als Prozentsatz festgelegte Bandbreitengrenzen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fb30ca54911723c619c8199ca32a9542772a6da
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177861"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="3ed00-103">deliveryOptimizationBandwidthPercentage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ed00-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="3ed00-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ed00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ed00-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3ed00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ed00-106">Als Prozentsatz festgelegte Bandbreitengrenzen.</span><span class="sxs-lookup"><span data-stu-id="3ed00-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="3ed00-107">Erbt von [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="3ed00-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ed00-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ed00-108">Properties</span></span>
|<span data-ttu-id="3ed00-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ed00-109">Property</span></span>|<span data-ttu-id="3ed00-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3ed00-110">Type</span></span>|<span data-ttu-id="3ed00-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ed00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ed00-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="3ed00-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="3ed00-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3ed00-113">Int32</span></span>|<span data-ttu-id="3ed00-114">Gibt die maximale Bandbreite des Hintergrund Downloads an, die von der BereitstellungsOptimierung für alle gleichzeitigen Download Aktivitäten als Prozentsatz der verfügbaren Download Bandbreite (0-100) verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="3ed00-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="3ed00-115">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="3ed00-115">Valid values 0 to 100</span></span>
<span data-ttu-id="3ed00-116">Der Standardwert 0 (null) bewirkt, dass die zuStellungsOptimierung dynamisch angepasst wird, um die verfügbare Bandbreite für Hintergrund Downloads zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="3ed00-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="3ed00-117">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="3ed00-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3ed00-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="3ed00-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="3ed00-119">Int32</span><span class="sxs-lookup"><span data-stu-id="3ed00-119">Int32</span></span>|<span data-ttu-id="3ed00-120">Gibt die maximale Bandbreite für den Vordergrund Download an, die von der BereitstellungsOptimierung für alle gleichzeitigen Download Aktivitäten als Prozentsatz der verfügbaren Download Bandbreite verwendet wird (0-100)</span><span class="sxs-lookup"><span data-stu-id="3ed00-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="3ed00-121">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="3ed00-121">Valid values 0 to 100</span></span>
<span data-ttu-id="3ed00-122">Der Standardwert 0 (null) bewirkt, dass die zuStellungsOptimierung dynamisch angepasst wird, um die verfügbare Bandbreite für Vordergrund Downloads zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="3ed00-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="3ed00-123">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="3ed00-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ed00-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3ed00-124">Relationships</span></span>
<span data-ttu-id="3ed00-125">Keine</span><span class="sxs-lookup"><span data-stu-id="3ed00-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ed00-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ed00-126">JSON Representation</span></span>
<span data-ttu-id="3ed00-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ed00-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```




