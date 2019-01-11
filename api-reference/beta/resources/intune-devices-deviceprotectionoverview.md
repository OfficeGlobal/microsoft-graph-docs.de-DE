---
title: Ressourcentyp deviceProtectionOverview
description: Hardwareinformationen für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 12066877e380c022a1cd1ec49322ab51b8e59d65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811529"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="7ec5d-103">Ressourcentyp deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="7ec5d-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="7ec5d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ec5d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ec5d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ec5d-107">Hardwareinformationen für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="7ec5d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7ec5d-108">Properties</span></span>
|<span data-ttu-id="7ec5d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ec5d-109">Property</span></span>|<span data-ttu-id="7ec5d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7ec5d-110">Type</span></span>|<span data-ttu-id="7ec5d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ec5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ec5d-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="7ec5d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-113">Int32</span></span>|<span data-ttu-id="7ec5d-114">Anzahl der insgesamt Geräte.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-114">Total device count.</span></span>|
|<span data-ttu-id="7ec5d-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="7ec5d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-116">Int32</span></span>|<span data-ttu-id="7ec5d-117">Gerät mit inaktiven Threat Agent count</span><span class="sxs-lookup"><span data-stu-id="7ec5d-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="7ec5d-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="7ec5d-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-119">Int32</span></span>|<span data-ttu-id="7ec5d-120">Gerät Threat Agent Zustand wie unbekannte Count.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="7ec5d-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="7ec5d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-122">Int32</span></span>|<span data-ttu-id="7ec5d-123">Das Gerät mit alten Signatur Count.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-123">Device with old signature count.</span></span>|
|<span data-ttu-id="7ec5d-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-124">cleanDeviceCount</span></span>|<span data-ttu-id="7ec5d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-125">Int32</span></span>|<span data-ttu-id="7ec5d-126">Bereinigen Sie die Anzahl der Geräte.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-126">Clean device count.</span></span>|
|<span data-ttu-id="7ec5d-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="7ec5d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-128">Int32</span></span>|<span data-ttu-id="7ec5d-129">Anzahl der ausstehenden vollständigen Scan Geräte.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="7ec5d-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="7ec5d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-131">Int32</span></span>|<span data-ttu-id="7ec5d-132">Anzahl ausstehender Neustart-Geräte.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-132">Pending restart device count.</span></span>|
|<span data-ttu-id="7ec5d-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="7ec5d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-134">Int32</span></span>|<span data-ttu-id="7ec5d-135">Anzahl der ausstehenden manuelle Schritte Geräte.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="7ec5d-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="7ec5d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-137">Int32</span></span>|<span data-ttu-id="7ec5d-138">Anzahl der ausstehenden offline Scan Geräte.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="7ec5d-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec5d-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="7ec5d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec5d-140">Int32</span></span>|<span data-ttu-id="7ec5d-141">Anzahl der Geräte kritische Fehler.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ec5d-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7ec5d-142">Relationships</span></span>
<span data-ttu-id="7ec5d-143">Keine</span><span class="sxs-lookup"><span data-stu-id="7ec5d-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ec5d-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7ec5d-144">JSON Representation</span></span>
<span data-ttu-id="7ec5d-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7ec5d-145">Here is a JSON representation of the resource.</span></span>
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





