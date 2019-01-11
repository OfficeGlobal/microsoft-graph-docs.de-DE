---
title: Ressourcentyp windowsProtectionState
description: Gerät Protection Status Entität.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a21cc27039f3119836e0027b2558cadadab1b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884105"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="34129-103">Ressourcentyp windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="34129-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="34129-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34129-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34129-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34129-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34129-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="34129-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34129-107">Gerät Protection Status Entität.</span><span class="sxs-lookup"><span data-stu-id="34129-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="34129-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="34129-108">Methods</span></span>
|<span data-ttu-id="34129-109">Methode</span><span class="sxs-lookup"><span data-stu-id="34129-109">Method</span></span>|<span data-ttu-id="34129-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="34129-110">Return Type</span></span>|<span data-ttu-id="34129-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34129-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34129-112">Abrufen von windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="34129-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="34129-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="34129-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="34129-114">Lesen Sie Eigenschaften und Beziehungen des [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="34129-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="34129-115">WindowsProtectionState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="34129-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="34129-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="34129-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="34129-117">Aktualisieren Sie die Eigenschaften eines [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="34129-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34129-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34129-118">Properties</span></span>
|<span data-ttu-id="34129-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34129-119">Property</span></span>|<span data-ttu-id="34129-120">Typ</span><span class="sxs-lookup"><span data-stu-id="34129-120">Type</span></span>|<span data-ttu-id="34129-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34129-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34129-122">id</span><span class="sxs-lookup"><span data-stu-id="34129-122">id</span></span>|<span data-ttu-id="34129-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34129-123">String</span></span>|<span data-ttu-id="34129-124">Der eindeutige Bezeichner für das Gerät Protection Status-Objekt.</span><span class="sxs-lookup"><span data-stu-id="34129-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="34129-125">Dies ist die Geräte-Id des Geräts</span><span class="sxs-lookup"><span data-stu-id="34129-125">This is device id of the device</span></span>|
|<span data-ttu-id="34129-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="34129-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="34129-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-127">Boolean</span></span>|<span data-ttu-id="34129-128">Anti-Malware ist oder nicht aktiviert</span><span class="sxs-lookup"><span data-stu-id="34129-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="34129-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="34129-129">deviceState</span></span>|[<span data-ttu-id="34129-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="34129-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="34129-131">Zustand des Computers (wie bereinigen oder ausstehende vollständigen Scan oder Ausstehender Neustart usw.).</span><span class="sxs-lookup"><span data-stu-id="34129-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="34129-132">Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.</span><span class="sxs-lookup"><span data-stu-id="34129-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="34129-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="34129-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="34129-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-134">Boolean</span></span>|<span data-ttu-id="34129-135">Echtzeit-Schutz ist oder nicht aktiviert?</span><span class="sxs-lookup"><span data-stu-id="34129-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="34129-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="34129-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="34129-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-137">Boolean</span></span>|<span data-ttu-id="34129-138">Netzwerk-Prüfung System aktiviert ist oder nicht?</span><span class="sxs-lookup"><span data-stu-id="34129-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="34129-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="34129-139">quickScanOverdue</span></span>|<span data-ttu-id="34129-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-140">Boolean</span></span>|<span data-ttu-id="34129-141">Quick scan überfällige oder nicht?</span><span class="sxs-lookup"><span data-stu-id="34129-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="34129-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="34129-142">fullScanOverdue</span></span>|<span data-ttu-id="34129-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-143">Boolean</span></span>|<span data-ttu-id="34129-144">Des vollständigen Scan überfällige oder nicht?</span><span class="sxs-lookup"><span data-stu-id="34129-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="34129-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="34129-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="34129-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-146">Boolean</span></span>|<span data-ttu-id="34129-147">Signatur veraltet oder nicht?</span><span class="sxs-lookup"><span data-stu-id="34129-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="34129-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="34129-148">rebootRequired</span></span>|<span data-ttu-id="34129-149">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-149">Boolean</span></span>|<span data-ttu-id="34129-150">Neustart erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="34129-150">Reboot required or not?</span></span>|
|<span data-ttu-id="34129-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="34129-151">fullScanRequired</span></span>|<span data-ttu-id="34129-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34129-152">Boolean</span></span>|<span data-ttu-id="34129-153">Vollständigen Scan erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="34129-153">Full scan required or not?</span></span>|
|<span data-ttu-id="34129-154">%ENGINEVERSION%</span><span class="sxs-lookup"><span data-stu-id="34129-154">engineVersion</span></span>|<span data-ttu-id="34129-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34129-155">String</span></span>|<span data-ttu-id="34129-156">Aktuelle Endpoint Protection Datenbankmodul, version</span><span class="sxs-lookup"><span data-stu-id="34129-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="34129-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="34129-157">signatureVersion</span></span>|<span data-ttu-id="34129-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34129-158">String</span></span>|<span data-ttu-id="34129-159">Aktuelle Version der Malware-Definitionen</span><span class="sxs-lookup"><span data-stu-id="34129-159">Current malware definitions version</span></span>|
|<span data-ttu-id="34129-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="34129-160">antiMalwareVersion</span></span>|<span data-ttu-id="34129-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34129-161">String</span></span>|<span data-ttu-id="34129-162">Aktuelle anti-Malware-version</span><span class="sxs-lookup"><span data-stu-id="34129-162">Current anti malware version</span></span>|
|<span data-ttu-id="34129-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="34129-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="34129-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34129-164">DateTimeOffset</span></span>|<span data-ttu-id="34129-165">Letzte schnell-Scan datetime</span><span class="sxs-lookup"><span data-stu-id="34129-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="34129-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="34129-166">lastFullScanDateTime</span></span>|<span data-ttu-id="34129-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34129-167">DateTimeOffset</span></span>|<span data-ttu-id="34129-168">Letzte schnell-Scan datetime</span><span class="sxs-lookup"><span data-stu-id="34129-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="34129-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="34129-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="34129-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34129-170">String</span></span>|<span data-ttu-id="34129-171">Letzte schnell-Scan Signatur-version</span><span class="sxs-lookup"><span data-stu-id="34129-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="34129-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="34129-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="34129-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34129-173">String</span></span>|<span data-ttu-id="34129-174">Letzte vollständige Überprüfung Signatur-version</span><span class="sxs-lookup"><span data-stu-id="34129-174">Last full scan signature version</span></span>|
|<span data-ttu-id="34129-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="34129-175">lastReportedDateTime</span></span>|<span data-ttu-id="34129-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34129-176">DateTimeOffset</span></span>|<span data-ttu-id="34129-177">Letzte Gerät Integritätsstatus gemeldet Zeit</span><span class="sxs-lookup"><span data-stu-id="34129-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="34129-178">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="34129-178">Relationships</span></span>
|<span data-ttu-id="34129-179">Beziehung</span><span class="sxs-lookup"><span data-stu-id="34129-179">Relationship</span></span>|<span data-ttu-id="34129-180">Typ</span><span class="sxs-lookup"><span data-stu-id="34129-180">Type</span></span>|<span data-ttu-id="34129-181">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34129-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34129-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="34129-182">detectedMalwareState</span></span>|<span data-ttu-id="34129-183">[WindowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="34129-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="34129-184">Liste der Geräte Schadsoftware</span><span class="sxs-lookup"><span data-stu-id="34129-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34129-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34129-185">JSON Representation</span></span>
<span data-ttu-id="34129-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="34129-186">Here is a JSON representation of the resource.</span></span>
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





