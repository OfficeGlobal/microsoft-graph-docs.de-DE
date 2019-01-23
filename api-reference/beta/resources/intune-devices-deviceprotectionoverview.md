---
title: Ressourcentyp deviceProtectionOverview
description: Hardwareinformationen für ein bestimmtes Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418988"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="cad54-103">Ressourcentyp deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="cad54-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="cad54-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cad54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cad54-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cad54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cad54-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cad54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cad54-107">Hardwareinformationen für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="cad54-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="cad54-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cad54-108">Properties</span></span>
|<span data-ttu-id="cad54-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cad54-109">Property</span></span>|<span data-ttu-id="cad54-110">Typ</span><span class="sxs-lookup"><span data-stu-id="cad54-110">Type</span></span>|<span data-ttu-id="cad54-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cad54-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cad54-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="cad54-113">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-113">Int32</span></span>|<span data-ttu-id="cad54-114">Anzahl der insgesamt Geräte.</span><span class="sxs-lookup"><span data-stu-id="cad54-114">Total device count.</span></span>|
|<span data-ttu-id="cad54-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="cad54-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-116">Int32</span></span>|<span data-ttu-id="cad54-117">Gerät mit inaktiven Threat Agent count</span><span class="sxs-lookup"><span data-stu-id="cad54-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="cad54-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="cad54-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-119">Int32</span></span>|<span data-ttu-id="cad54-120">Gerät Threat Agent Zustand wie unbekannte Count.</span><span class="sxs-lookup"><span data-stu-id="cad54-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="cad54-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="cad54-122">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-122">Int32</span></span>|<span data-ttu-id="cad54-123">Das Gerät mit alten Signatur Count.</span><span class="sxs-lookup"><span data-stu-id="cad54-123">Device with old signature count.</span></span>|
|<span data-ttu-id="cad54-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-124">cleanDeviceCount</span></span>|<span data-ttu-id="cad54-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-125">Int32</span></span>|<span data-ttu-id="cad54-126">Bereinigen Sie die Anzahl der Geräte.</span><span class="sxs-lookup"><span data-stu-id="cad54-126">Clean device count.</span></span>|
|<span data-ttu-id="cad54-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="cad54-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-128">Int32</span></span>|<span data-ttu-id="cad54-129">Anzahl der ausstehenden vollständigen Scan Geräte.</span><span class="sxs-lookup"><span data-stu-id="cad54-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="cad54-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="cad54-131">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-131">Int32</span></span>|<span data-ttu-id="cad54-132">Anzahl ausstehender Neustart-Geräte.</span><span class="sxs-lookup"><span data-stu-id="cad54-132">Pending restart device count.</span></span>|
|<span data-ttu-id="cad54-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="cad54-134">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-134">Int32</span></span>|<span data-ttu-id="cad54-135">Anzahl der ausstehenden manuelle Schritte Geräte.</span><span class="sxs-lookup"><span data-stu-id="cad54-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="cad54-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="cad54-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-137">Int32</span></span>|<span data-ttu-id="cad54-138">Anzahl der ausstehenden offline Scan Geräte.</span><span class="sxs-lookup"><span data-stu-id="cad54-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="cad54-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cad54-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="cad54-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cad54-140">Int32</span></span>|<span data-ttu-id="cad54-141">Anzahl der Geräte kritische Fehler.</span><span class="sxs-lookup"><span data-stu-id="cad54-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cad54-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cad54-142">Relationships</span></span>
<span data-ttu-id="cad54-143">Keine</span><span class="sxs-lookup"><span data-stu-id="cad54-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cad54-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cad54-144">JSON Representation</span></span>
<span data-ttu-id="cad54-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cad54-145">Here is a JSON representation of the resource.</span></span>
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




