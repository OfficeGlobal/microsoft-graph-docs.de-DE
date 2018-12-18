---
title: deviceCompliancePolicyDeviceStateSummary-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 229a03830fec065cbed9861ad1db07418c3fbfa8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329015"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="e02a9-103">deviceCompliancePolicyDeviceStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e02a9-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="e02a9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e02a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e02a9-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e02a9-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="e02a9-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="e02a9-106">Methods</span></span>
|<span data-ttu-id="e02a9-107">Methode</span><span class="sxs-lookup"><span data-stu-id="e02a9-107">Method</span></span>|<span data-ttu-id="e02a9-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e02a9-108">Return Type</span></span>|<span data-ttu-id="e02a9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e02a9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e02a9-110">deviceCompliancePolicyDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="e02a9-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="e02a9-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e02a9-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e02a9-112">Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e02a9-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="e02a9-113">deviceCompliancePolicyDeviceStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e02a9-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="e02a9-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e02a9-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e02a9-115">Aktualisieren der Eigenschaften eines [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e02a9-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e02a9-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e02a9-116">Properties</span></span>
|<span data-ttu-id="e02a9-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e02a9-117">Property</span></span>|<span data-ttu-id="e02a9-118">Typ</span><span class="sxs-lookup"><span data-stu-id="e02a9-118">Type</span></span>|<span data-ttu-id="e02a9-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e02a9-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e02a9-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-120">inGracePeriodCount</span></span>|<span data-ttu-id="e02a9-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-121">Int32</span></span>|<span data-ttu-id="e02a9-122">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="e02a9-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e02a9-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-123">configManagerCount</span></span>|<span data-ttu-id="e02a9-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-124">Int32</span></span>|<span data-ttu-id="e02a9-125">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e02a9-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e02a9-126">id</span><span class="sxs-lookup"><span data-stu-id="e02a9-126">id</span></span>|<span data-ttu-id="e02a9-127">String</span><span class="sxs-lookup"><span data-stu-id="e02a9-127">String</span></span>|<span data-ttu-id="e02a9-128">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e02a9-128">Key of the entity.</span></span>|
|<span data-ttu-id="e02a9-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-129">unknownDeviceCount</span></span>|<span data-ttu-id="e02a9-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-130">Int32</span></span>|<span data-ttu-id="e02a9-131">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="e02a9-131">Number of unknown devices</span></span>|
|<span data-ttu-id="e02a9-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="e02a9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-133">Int32</span></span>|<span data-ttu-id="e02a9-134">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="e02a9-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="e02a9-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-135">compliantDeviceCount</span></span>|<span data-ttu-id="e02a9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-136">Int32</span></span>|<span data-ttu-id="e02a9-137">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="e02a9-137">Number of compliant devices</span></span>|
|<span data-ttu-id="e02a9-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-138">remediatedDeviceCount</span></span>|<span data-ttu-id="e02a9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-139">Int32</span></span>|<span data-ttu-id="e02a9-140">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="e02a9-140">Number of remediated devices</span></span>|
|<span data-ttu-id="e02a9-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e02a9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-142">Int32</span></span>|<span data-ttu-id="e02a9-143">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="e02a9-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e02a9-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-144">errorDeviceCount</span></span>|<span data-ttu-id="e02a9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-145">Int32</span></span>|<span data-ttu-id="e02a9-146">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="e02a9-146">Number of error devices</span></span>|
|<span data-ttu-id="e02a9-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e02a9-147">conflictDeviceCount</span></span>|<span data-ttu-id="e02a9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e02a9-148">Int32</span></span>|<span data-ttu-id="e02a9-149">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="e02a9-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e02a9-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e02a9-150">Relationships</span></span>
<span data-ttu-id="e02a9-151">Keine</span><span class="sxs-lookup"><span data-stu-id="e02a9-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e02a9-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e02a9-152">JSON Representation</span></span>
<span data-ttu-id="e02a9-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e02a9-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



