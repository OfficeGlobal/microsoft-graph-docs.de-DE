---
title: Ressourcentyp windowsProtectionState
description: Gerät Protection Status Entität.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423587"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="aa36a-103">Ressourcentyp windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="aa36a-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="aa36a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="aa36a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa36a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa36a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa36a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa36a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa36a-107">Gerät Protection Status Entität.</span><span class="sxs-lookup"><span data-stu-id="aa36a-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="aa36a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="aa36a-108">Methods</span></span>
|<span data-ttu-id="aa36a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="aa36a-109">Method</span></span>|<span data-ttu-id="aa36a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aa36a-110">Return Type</span></span>|<span data-ttu-id="aa36a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa36a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa36a-112">Abrufen von windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="aa36a-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="aa36a-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="aa36a-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="aa36a-114">Lesen Sie Eigenschaften und Beziehungen des [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa36a-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="aa36a-115">WindowsProtectionState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aa36a-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="aa36a-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="aa36a-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="aa36a-117">Aktualisieren Sie die Eigenschaften eines [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa36a-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa36a-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa36a-118">Properties</span></span>
|<span data-ttu-id="aa36a-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa36a-119">Property</span></span>|<span data-ttu-id="aa36a-120">Typ</span><span class="sxs-lookup"><span data-stu-id="aa36a-120">Type</span></span>|<span data-ttu-id="aa36a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa36a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa36a-122">id</span><span class="sxs-lookup"><span data-stu-id="aa36a-122">id</span></span>|<span data-ttu-id="aa36a-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa36a-123">String</span></span>|<span data-ttu-id="aa36a-124">Der eindeutige Bezeichner für das Gerät Protection Status-Objekt.</span><span class="sxs-lookup"><span data-stu-id="aa36a-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="aa36a-125">Dies ist die Geräte-Id des Geräts</span><span class="sxs-lookup"><span data-stu-id="aa36a-125">This is device id of the device</span></span>|
|<span data-ttu-id="aa36a-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="aa36a-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="aa36a-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-127">Boolean</span></span>|<span data-ttu-id="aa36a-128">Anti-Malware ist oder nicht aktiviert</span><span class="sxs-lookup"><span data-stu-id="aa36a-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="aa36a-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="aa36a-129">deviceState</span></span>|[<span data-ttu-id="aa36a-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="aa36a-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="aa36a-131">Zustand des Computers (wie bereinigen oder ausstehende vollständigen Scan oder Ausstehender Neustart usw.).</span><span class="sxs-lookup"><span data-stu-id="aa36a-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="aa36a-132">Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.</span><span class="sxs-lookup"><span data-stu-id="aa36a-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="aa36a-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="aa36a-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="aa36a-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-134">Boolean</span></span>|<span data-ttu-id="aa36a-135">Echtzeit-Schutz ist oder nicht aktiviert?</span><span class="sxs-lookup"><span data-stu-id="aa36a-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="aa36a-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="aa36a-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="aa36a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-137">Boolean</span></span>|<span data-ttu-id="aa36a-138">Netzwerk-Prüfung System aktiviert ist oder nicht?</span><span class="sxs-lookup"><span data-stu-id="aa36a-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="aa36a-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="aa36a-139">quickScanOverdue</span></span>|<span data-ttu-id="aa36a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-140">Boolean</span></span>|<span data-ttu-id="aa36a-141">Quick scan überfällige oder nicht?</span><span class="sxs-lookup"><span data-stu-id="aa36a-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="aa36a-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="aa36a-142">fullScanOverdue</span></span>|<span data-ttu-id="aa36a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-143">Boolean</span></span>|<span data-ttu-id="aa36a-144">Des vollständigen Scan überfällige oder nicht?</span><span class="sxs-lookup"><span data-stu-id="aa36a-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="aa36a-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="aa36a-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="aa36a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-146">Boolean</span></span>|<span data-ttu-id="aa36a-147">Signatur veraltet oder nicht?</span><span class="sxs-lookup"><span data-stu-id="aa36a-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="aa36a-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="aa36a-148">rebootRequired</span></span>|<span data-ttu-id="aa36a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-149">Boolean</span></span>|<span data-ttu-id="aa36a-150">Neustart erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="aa36a-150">Reboot required or not?</span></span>|
|<span data-ttu-id="aa36a-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="aa36a-151">fullScanRequired</span></span>|<span data-ttu-id="aa36a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa36a-152">Boolean</span></span>|<span data-ttu-id="aa36a-153">Vollständigen Scan erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="aa36a-153">Full scan required or not?</span></span>|
|<span data-ttu-id="aa36a-154">%ENGINEVERSION%</span><span class="sxs-lookup"><span data-stu-id="aa36a-154">engineVersion</span></span>|<span data-ttu-id="aa36a-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa36a-155">String</span></span>|<span data-ttu-id="aa36a-156">Aktuelle Endpoint Protection Datenbankmodul, version</span><span class="sxs-lookup"><span data-stu-id="aa36a-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="aa36a-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="aa36a-157">signatureVersion</span></span>|<span data-ttu-id="aa36a-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa36a-158">String</span></span>|<span data-ttu-id="aa36a-159">Aktuelle Version der Malware-Definitionen</span><span class="sxs-lookup"><span data-stu-id="aa36a-159">Current malware definitions version</span></span>|
|<span data-ttu-id="aa36a-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="aa36a-160">antiMalwareVersion</span></span>|<span data-ttu-id="aa36a-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa36a-161">String</span></span>|<span data-ttu-id="aa36a-162">Aktuelle anti-Malware-version</span><span class="sxs-lookup"><span data-stu-id="aa36a-162">Current anti malware version</span></span>|
|<span data-ttu-id="aa36a-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="aa36a-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="aa36a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa36a-164">DateTimeOffset</span></span>|<span data-ttu-id="aa36a-165">Letzte schnell-Scan datetime</span><span class="sxs-lookup"><span data-stu-id="aa36a-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="aa36a-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="aa36a-166">lastFullScanDateTime</span></span>|<span data-ttu-id="aa36a-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa36a-167">DateTimeOffset</span></span>|<span data-ttu-id="aa36a-168">Letzte schnell-Scan datetime</span><span class="sxs-lookup"><span data-stu-id="aa36a-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="aa36a-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="aa36a-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="aa36a-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa36a-170">String</span></span>|<span data-ttu-id="aa36a-171">Letzte schnell-Scan Signatur-version</span><span class="sxs-lookup"><span data-stu-id="aa36a-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="aa36a-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="aa36a-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="aa36a-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa36a-173">String</span></span>|<span data-ttu-id="aa36a-174">Letzte vollständige Überprüfung Signatur-version</span><span class="sxs-lookup"><span data-stu-id="aa36a-174">Last full scan signature version</span></span>|
|<span data-ttu-id="aa36a-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa36a-175">lastReportedDateTime</span></span>|<span data-ttu-id="aa36a-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa36a-176">DateTimeOffset</span></span>|<span data-ttu-id="aa36a-177">Letzte Gerät Integritätsstatus gemeldet Zeit</span><span class="sxs-lookup"><span data-stu-id="aa36a-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa36a-178">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aa36a-178">Relationships</span></span>
|<span data-ttu-id="aa36a-179">Beziehung</span><span class="sxs-lookup"><span data-stu-id="aa36a-179">Relationship</span></span>|<span data-ttu-id="aa36a-180">Typ</span><span class="sxs-lookup"><span data-stu-id="aa36a-180">Type</span></span>|<span data-ttu-id="aa36a-181">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa36a-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa36a-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="aa36a-182">detectedMalwareState</span></span>|<span data-ttu-id="aa36a-183">[WindowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="aa36a-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="aa36a-184">Liste der Geräte Schadsoftware</span><span class="sxs-lookup"><span data-stu-id="aa36a-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa36a-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa36a-185">JSON Representation</span></span>
<span data-ttu-id="aa36a-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa36a-186">Here is a JSON representation of the resource.</span></span>
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




