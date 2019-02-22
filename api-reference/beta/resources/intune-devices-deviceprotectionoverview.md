---
title: deviceProtectionOverview-Ressourcentyp
description: Hardware Informationen eines bestimmten Geräts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d6cd5cc1eef939476a6fa3b5c46a7cfa315607b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154089"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="16896-103">deviceProtectionOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16896-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="16896-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16896-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16896-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="16896-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16896-106">Hardware Informationen eines bestimmten Geräts.</span><span class="sxs-lookup"><span data-stu-id="16896-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="16896-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16896-107">Properties</span></span>
|<span data-ttu-id="16896-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16896-108">Property</span></span>|<span data-ttu-id="16896-109">Typ</span><span class="sxs-lookup"><span data-stu-id="16896-109">Type</span></span>|<span data-ttu-id="16896-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16896-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16896-111">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="16896-112">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-112">Int32</span></span>|<span data-ttu-id="16896-113">Gesamtanzahl der Geräte.</span><span class="sxs-lookup"><span data-stu-id="16896-113">Total device count.</span></span>|
|<span data-ttu-id="16896-114">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="16896-115">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-115">Int32</span></span>|<span data-ttu-id="16896-116">Geräte mit Anzahl der inaktiven Bedrohungen</span><span class="sxs-lookup"><span data-stu-id="16896-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="16896-117">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="16896-118">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-118">Int32</span></span>|<span data-ttu-id="16896-119">Gerät mit dem Status des Bedrohungs-Agents als unbekannte Anzahl.</span><span class="sxs-lookup"><span data-stu-id="16896-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="16896-120">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="16896-121">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-121">Int32</span></span>|<span data-ttu-id="16896-122">Gerät mit Alter Signatur Anzahl.</span><span class="sxs-lookup"><span data-stu-id="16896-122">Device with old signature count.</span></span>|
|<span data-ttu-id="16896-123">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-123">cleanDeviceCount</span></span>|<span data-ttu-id="16896-124">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-124">Int32</span></span>|<span data-ttu-id="16896-125">Geräteanzahl wird bereinigt.</span><span class="sxs-lookup"><span data-stu-id="16896-125">Clean device count.</span></span>|
|<span data-ttu-id="16896-126">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="16896-127">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-127">Int32</span></span>|<span data-ttu-id="16896-128">Anzahl der ausStehenden vollständigen Scans.</span><span class="sxs-lookup"><span data-stu-id="16896-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="16896-129">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="16896-130">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-130">Int32</span></span>|<span data-ttu-id="16896-131">Anzahl der ausStehenden Neustart Geräte.</span><span class="sxs-lookup"><span data-stu-id="16896-131">Pending restart device count.</span></span>|
|<span data-ttu-id="16896-132">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="16896-133">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-133">Int32</span></span>|<span data-ttu-id="16896-134">AusStehende manuelle Schritte Geräteanzahl.</span><span class="sxs-lookup"><span data-stu-id="16896-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="16896-135">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="16896-136">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-136">Int32</span></span>|<span data-ttu-id="16896-137">Anzahl der ausStehenden Offline Scangeräte.</span><span class="sxs-lookup"><span data-stu-id="16896-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="16896-138">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16896-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="16896-139">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-139">Int32</span></span>|<span data-ttu-id="16896-140">Geräteanzahl für kritische Fehler.</span><span class="sxs-lookup"><span data-stu-id="16896-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16896-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16896-141">Relationships</span></span>
<span data-ttu-id="16896-142">Keine</span><span class="sxs-lookup"><span data-stu-id="16896-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16896-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16896-143">JSON Representation</span></span>
<span data-ttu-id="16896-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16896-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




