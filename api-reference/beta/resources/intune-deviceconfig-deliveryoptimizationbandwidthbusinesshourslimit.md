---
title: deliveryOptimizationBandwidthBusinessHoursLimit-Ressourcentyp
description: Bandbreiten-und prozentuale Geschäftszeiten
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba15df46075e5cbea1a2eab8a798c333f4a60ae6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178115"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="dffa9-103">deliveryOptimizationBandwidthBusinessHoursLimit-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dffa9-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="dffa9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dffa9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dffa9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dffa9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dffa9-106">Bandbreiten-und prozentuale Geschäftszeiten</span><span class="sxs-lookup"><span data-stu-id="dffa9-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="dffa9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dffa9-107">Properties</span></span>
|<span data-ttu-id="dffa9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dffa9-108">Property</span></span>|<span data-ttu-id="dffa9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="dffa9-109">Type</span></span>|<span data-ttu-id="dffa9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dffa9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dffa9-111">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="dffa9-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="dffa9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="dffa9-112">Int32</span></span>|<span data-ttu-id="dffa9-113">Gibt den Beginn der Geschäftszeiten mit einer 24-Stunden-Uhr an (0-23).</span><span class="sxs-lookup"><span data-stu-id="dffa9-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="dffa9-114">Gültige Werte 0 bis 23</span><span class="sxs-lookup"><span data-stu-id="dffa9-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="dffa9-115">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="dffa9-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="dffa9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="dffa9-116">Int32</span></span>|<span data-ttu-id="dffa9-117">Gibt das Ende der Geschäftszeiten in einem 24-Stunden-Format an (0-23).</span><span class="sxs-lookup"><span data-stu-id="dffa9-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="dffa9-118">Gültige Werte 0 bis 23</span><span class="sxs-lookup"><span data-stu-id="dffa9-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="dffa9-119">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="dffa9-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="dffa9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="dffa9-120">Int32</span></span>|<span data-ttu-id="dffa9-121">Gibt den Prozentsatz der Bandbreite an, der während der Geschäftszeiten begrenzt werden soll (0-100).</span><span class="sxs-lookup"><span data-stu-id="dffa9-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="dffa9-122">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="dffa9-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="dffa9-123">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="dffa9-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="dffa9-124">Int32</span><span class="sxs-lookup"><span data-stu-id="dffa9-124">Int32</span></span>|<span data-ttu-id="dffa9-125">Gibt den Prozentsatz der Bandbreite an, um die Geschäftszeiten für SIDs zu begrenzen (0-100).</span><span class="sxs-lookup"><span data-stu-id="dffa9-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="dffa9-126">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="dffa9-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="dffa9-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dffa9-127">Relationships</span></span>
<span data-ttu-id="dffa9-128">Keine</span><span class="sxs-lookup"><span data-stu-id="dffa9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dffa9-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dffa9-129">JSON Representation</span></span>
<span data-ttu-id="dffa9-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dffa9-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```




