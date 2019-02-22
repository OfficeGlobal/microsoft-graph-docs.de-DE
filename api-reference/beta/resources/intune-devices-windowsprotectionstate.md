---
title: Windowsprotectionstate wurde-Ressourcentyp
description: Geräteschutz Status-Entität.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eebf798a41e5cbab27fab849cdead8a288a782e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148314"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="4b76d-103">Windowsprotectionstate wurde-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4b76d-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="4b76d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b76d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b76d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4b76d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b76d-106">Geräteschutz Status-Entität.</span><span class="sxs-lookup"><span data-stu-id="4b76d-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="4b76d-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="4b76d-107">Methods</span></span>
|<span data-ttu-id="4b76d-108">Methode</span><span class="sxs-lookup"><span data-stu-id="4b76d-108">Method</span></span>|<span data-ttu-id="4b76d-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4b76d-109">Return Type</span></span>|<span data-ttu-id="4b76d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b76d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b76d-111">Windowsprotectionstate wurde abrufen</span><span class="sxs-lookup"><span data-stu-id="4b76d-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="4b76d-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="4b76d-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="4b76d-113">Lesen von Eigenschaften und Beziehungen des [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b76d-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="4b76d-114">Windowsprotectionstate wurde aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4b76d-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="4b76d-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="4b76d-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="4b76d-116">Aktualisieren der Eigenschaften eines [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b76d-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b76d-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b76d-117">Properties</span></span>
|<span data-ttu-id="4b76d-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b76d-118">Property</span></span>|<span data-ttu-id="4b76d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="4b76d-119">Type</span></span>|<span data-ttu-id="4b76d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b76d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b76d-121">id</span><span class="sxs-lookup"><span data-stu-id="4b76d-121">id</span></span>|<span data-ttu-id="4b76d-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b76d-122">String</span></span>|<span data-ttu-id="4b76d-123">Der eindeutige Bezeichner für das Statusobjekt des Geräteschutzes.</span><span class="sxs-lookup"><span data-stu-id="4b76d-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="4b76d-124">Dies ist die Geräte-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4b76d-124">This is device id of the device</span></span>|
|<span data-ttu-id="4b76d-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4b76d-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="4b76d-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-126">Boolean</span></span>|<span data-ttu-id="4b76d-127">Antischadsoftware ist aktiviert oder nicht</span><span class="sxs-lookup"><span data-stu-id="4b76d-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="4b76d-128">deviceState</span><span class="sxs-lookup"><span data-stu-id="4b76d-128">deviceState</span></span>|[<span data-ttu-id="4b76d-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="4b76d-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="4b76d-130">Status des Computers (wie Clean oder ausstehender vollständiger Scan oder ausstehender Neustart usw.).</span><span class="sxs-lookup"><span data-stu-id="4b76d-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="4b76d-131">Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.</span><span class="sxs-lookup"><span data-stu-id="4b76d-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="4b76d-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4b76d-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="4b76d-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-133">Boolean</span></span>|<span data-ttu-id="4b76d-134">Echtzeitschutz ist aktiviert oder nicht?</span><span class="sxs-lookup"><span data-stu-id="4b76d-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="4b76d-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="4b76d-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="4b76d-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-136">Boolean</span></span>|<span data-ttu-id="4b76d-137">Netzwerk Inspektionssystem aktiviert oder nicht?</span><span class="sxs-lookup"><span data-stu-id="4b76d-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="4b76d-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="4b76d-138">quickScanOverdue</span></span>|<span data-ttu-id="4b76d-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-139">Boolean</span></span>|<span data-ttu-id="4b76d-140">Schnellscan überfällig oder nicht?</span><span class="sxs-lookup"><span data-stu-id="4b76d-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="4b76d-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="4b76d-141">fullScanOverdue</span></span>|<span data-ttu-id="4b76d-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-142">Boolean</span></span>|<span data-ttu-id="4b76d-143">Vollständiger Scan überfällig oder nicht?</span><span class="sxs-lookup"><span data-stu-id="4b76d-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="4b76d-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="4b76d-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="4b76d-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-145">Boolean</span></span>|<span data-ttu-id="4b76d-146">Signatur veraltet oder nicht?</span><span class="sxs-lookup"><span data-stu-id="4b76d-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="4b76d-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="4b76d-147">rebootRequired</span></span>|<span data-ttu-id="4b76d-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-148">Boolean</span></span>|<span data-ttu-id="4b76d-149">Neustart erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="4b76d-149">Reboot required or not?</span></span>|
|<span data-ttu-id="4b76d-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="4b76d-150">fullScanRequired</span></span>|<span data-ttu-id="4b76d-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b76d-151">Boolean</span></span>|<span data-ttu-id="4b76d-152">Vollständige Überprüfung erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="4b76d-152">Full scan required or not?</span></span>|
|<span data-ttu-id="4b76d-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="4b76d-153">engineVersion</span></span>|<span data-ttu-id="4b76d-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b76d-154">String</span></span>|<span data-ttu-id="4b76d-155">Version des aktuellen Endpoint Protection-Moduls</span><span class="sxs-lookup"><span data-stu-id="4b76d-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="4b76d-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="4b76d-156">signatureVersion</span></span>|<span data-ttu-id="4b76d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b76d-157">String</span></span>|<span data-ttu-id="4b76d-158">Aktuelle Version der Malware-Definitionen</span><span class="sxs-lookup"><span data-stu-id="4b76d-158">Current malware definitions version</span></span>|
|<span data-ttu-id="4b76d-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="4b76d-159">antiMalwareVersion</span></span>|<span data-ttu-id="4b76d-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b76d-160">String</span></span>|<span data-ttu-id="4b76d-161">Aktuelle Antischadsoftware-Version</span><span class="sxs-lookup"><span data-stu-id="4b76d-161">Current anti malware version</span></span>|
|<span data-ttu-id="4b76d-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="4b76d-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="4b76d-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b76d-163">DateTimeOffset</span></span>|<span data-ttu-id="4b76d-164">Datum der letzten Schnellüberprüfung</span><span class="sxs-lookup"><span data-stu-id="4b76d-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="4b76d-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="4b76d-165">lastFullScanDateTime</span></span>|<span data-ttu-id="4b76d-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b76d-166">DateTimeOffset</span></span>|<span data-ttu-id="4b76d-167">Datum der letzten Schnellüberprüfung</span><span class="sxs-lookup"><span data-stu-id="4b76d-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="4b76d-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="4b76d-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="4b76d-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b76d-169">String</span></span>|<span data-ttu-id="4b76d-170">Letzte Schnellscan-Signaturversion</span><span class="sxs-lookup"><span data-stu-id="4b76d-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="4b76d-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="4b76d-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="4b76d-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b76d-172">String</span></span>|<span data-ttu-id="4b76d-173">Letzte vollständige Scan-Signaturversion</span><span class="sxs-lookup"><span data-stu-id="4b76d-173">Last full scan signature version</span></span>|
|<span data-ttu-id="4b76d-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b76d-174">lastReportedDateTime</span></span>|<span data-ttu-id="4b76d-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b76d-175">DateTimeOffset</span></span>|<span data-ttu-id="4b76d-176">Zeitpunkt des letzten Geräte Integritätsstatus</span><span class="sxs-lookup"><span data-stu-id="4b76d-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b76d-177">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4b76d-177">Relationships</span></span>
|<span data-ttu-id="4b76d-178">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4b76d-178">Relationship</span></span>|<span data-ttu-id="4b76d-179">Typ</span><span class="sxs-lookup"><span data-stu-id="4b76d-179">Type</span></span>|<span data-ttu-id="4b76d-180">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b76d-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b76d-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="4b76d-181">detectedMalwareState</span></span>|<span data-ttu-id="4b76d-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="4b76d-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="4b76d-183">Liste der Geräte Schadsoftware</span><span class="sxs-lookup"><span data-stu-id="4b76d-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b76d-184">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b76d-184">JSON Representation</span></span>
<span data-ttu-id="4b76d-185">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b76d-185">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```




