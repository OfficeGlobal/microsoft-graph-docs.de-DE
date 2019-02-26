---
title: deliveryOptimizationBandwidthAbsolute-Ressourcentyp
description: Bandbreitenbegrenzungen in Kilobyte pro Sekunde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eca95ad33ced19e437e760663a73158aacc25d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178269"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="b8835-103">deliveryOptimizationBandwidthAbsolute-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8835-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

> <span data-ttu-id="b8835-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8835-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8835-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8835-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8835-106">Bandbreitenbegrenzungen in Kilobyte pro Sekunde.</span><span class="sxs-lookup"><span data-stu-id="b8835-106">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="b8835-107">Erbt von [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="b8835-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8835-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8835-108">Properties</span></span>
|<span data-ttu-id="b8835-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8835-109">Property</span></span>|<span data-ttu-id="b8835-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b8835-110">Type</span></span>|<span data-ttu-id="b8835-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8835-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8835-112">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="b8835-112">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="b8835-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b8835-113">Int64</span></span>|<span data-ttu-id="b8835-114">Gibt die maximale Download Bandbreite in KiloByte/Sekunde an, die das Gerät für alle gleichzeitigen Download Aktivitäten mithilfe der Übermittlungs Optimierung verwenden kann.</span><span class="sxs-lookup"><span data-stu-id="b8835-114">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="b8835-115">Gültige Werte 0 bis 4294967295</span><span class="sxs-lookup"><span data-stu-id="b8835-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="b8835-116">Der Wert 0 (null) bewirkt, dass die zuStellungsOptimierung dynamisch angepasst wird, um die verfügbare Bandbreite für Downloads zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="b8835-116">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="b8835-117">Gültige Werte 0 bis 4294967295</span><span class="sxs-lookup"><span data-stu-id="b8835-117">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="b8835-118">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="b8835-118">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="b8835-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b8835-119">Int64</span></span>|<span data-ttu-id="b8835-120">Gibt die maximale Upload-Bandbreite in KiloByte/Sekunde an, die ein Gerät für alle gleichzeitigen Upload-Aktivitäten mithilfe der Übermittlungs Optimierung verwendet (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="b8835-120">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="b8835-121">Gültige Werte 0 bis 4 Millionen</span><span class="sxs-lookup"><span data-stu-id="b8835-121">Valid values 0 to 4000000</span></span>
<span data-ttu-id="b8835-122">Der Standardwert ist 0, was eine unbegrenzte Bandbreite erlaubt (optimiert für minimale Auslastung der Upload-Bandbreite).</span><span class="sxs-lookup"><span data-stu-id="b8835-122">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="b8835-123">Gültige Werte 0 bis 4 Millionen</span><span class="sxs-lookup"><span data-stu-id="b8835-123">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8835-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8835-124">Relationships</span></span>
<span data-ttu-id="b8835-125">Keine</span><span class="sxs-lookup"><span data-stu-id="b8835-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8835-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8835-126">JSON Representation</span></span>
<span data-ttu-id="b8835-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8835-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```




