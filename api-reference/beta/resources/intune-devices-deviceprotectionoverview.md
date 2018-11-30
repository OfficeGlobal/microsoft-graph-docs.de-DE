---
title: Ressourcentyp deviceProtectionOverview
description: Hardwareinformationen für ein bestimmtes Gerät.
ms.openlocfilehash: 81252fdf60c1de129a615b075968e0e6f1eca943
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063482"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="9097f-103">Ressourcentyp deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="9097f-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="9097f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9097f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9097f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9097f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9097f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9097f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9097f-107">Hardwareinformationen für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="9097f-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="9097f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9097f-108">Properties</span></span>
|<span data-ttu-id="9097f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9097f-109">Property</span></span>|<span data-ttu-id="9097f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9097f-110">Type</span></span>|<span data-ttu-id="9097f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9097f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9097f-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="9097f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-113">Int32</span></span>|<span data-ttu-id="9097f-114">Anzahl der insgesamt Geräte.</span><span class="sxs-lookup"><span data-stu-id="9097f-114">Total device count.</span></span>|
|<span data-ttu-id="9097f-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="9097f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-116">Int32</span></span>|<span data-ttu-id="9097f-117">Gerät mit inaktiven Threat Agent count</span><span class="sxs-lookup"><span data-stu-id="9097f-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="9097f-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="9097f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-119">Int32</span></span>|<span data-ttu-id="9097f-120">Gerät Threat Agent Zustand wie unbekannte Count.</span><span class="sxs-lookup"><span data-stu-id="9097f-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="9097f-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="9097f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-122">Int32</span></span>|<span data-ttu-id="9097f-123">Das Gerät mit alten Signatur Count.</span><span class="sxs-lookup"><span data-stu-id="9097f-123">Device with old signature count.</span></span>|
|<span data-ttu-id="9097f-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-124">cleanDeviceCount</span></span>|<span data-ttu-id="9097f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-125">Int32</span></span>|<span data-ttu-id="9097f-126">Bereinigen Sie die Anzahl der Geräte.</span><span class="sxs-lookup"><span data-stu-id="9097f-126">Clean device count.</span></span>|
|<span data-ttu-id="9097f-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="9097f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-128">Int32</span></span>|<span data-ttu-id="9097f-129">Anzahl der ausstehenden vollständigen Scan Geräte.</span><span class="sxs-lookup"><span data-stu-id="9097f-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="9097f-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="9097f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-131">Int32</span></span>|<span data-ttu-id="9097f-132">Anzahl ausstehender Neustart-Geräte.</span><span class="sxs-lookup"><span data-stu-id="9097f-132">Pending restart device count.</span></span>|
|<span data-ttu-id="9097f-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="9097f-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-134">Int32</span></span>|<span data-ttu-id="9097f-135">Anzahl der ausstehenden manuelle Schritte Geräte.</span><span class="sxs-lookup"><span data-stu-id="9097f-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="9097f-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="9097f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-137">Int32</span></span>|<span data-ttu-id="9097f-138">Anzahl der ausstehenden offline Scan Geräte.</span><span class="sxs-lookup"><span data-stu-id="9097f-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="9097f-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9097f-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="9097f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9097f-140">Int32</span></span>|<span data-ttu-id="9097f-141">Anzahl der Geräte kritische Fehler.</span><span class="sxs-lookup"><span data-stu-id="9097f-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9097f-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9097f-142">Relationships</span></span>
<span data-ttu-id="9097f-143">Keine</span><span class="sxs-lookup"><span data-stu-id="9097f-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9097f-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9097f-144">JSON Representation</span></span>
<span data-ttu-id="9097f-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9097f-145">Here is a JSON representation of the resource.</span></span>
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





