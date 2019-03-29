---
title: Windowsprotectionstate wurde aktualisieren
description: Aktualisieren der Eigenschaften eines Windowsprotectionstate wurde-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a77cf48766d2ea6aec8f9f2f1017530226be5bc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973887"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="b94c6-103">Windowsprotectionstate wurde aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b94c6-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="b94c6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b94c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b94c6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b94c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b94c6-106">Aktualisieren der Eigenschaften eines [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b94c6-106">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b94c6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b94c6-107">Prerequisites</span></span>
<span data-ttu-id="b94c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b94c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b94c6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b94c6-110">Permission type</span></span>|<span data-ttu-id="b94c6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b94c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b94c6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b94c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b94c6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b94c6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b94c6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b94c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b94c6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b94c6-115">Not supported.</span></span>|
|<span data-ttu-id="b94c6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b94c6-116">Application</span></span>|<span data-ttu-id="b94c6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b94c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b94c6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b94c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="b94c6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b94c6-119">Request headers</span></span>
|<span data-ttu-id="b94c6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b94c6-120">Header</span></span>|<span data-ttu-id="b94c6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b94c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b94c6-122">Authorization</span></span>|<span data-ttu-id="b94c6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b94c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b94c6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b94c6-124">Accept</span></span>|<span data-ttu-id="b94c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b94c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b94c6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b94c6-126">Request body</span></span>
<span data-ttu-id="b94c6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b94c6-127">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="b94c6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b94c6-128">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="b94c6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b94c6-129">Property</span></span>|<span data-ttu-id="b94c6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b94c6-130">Type</span></span>|<span data-ttu-id="b94c6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b94c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b94c6-132">id</span><span class="sxs-lookup"><span data-stu-id="b94c6-132">id</span></span>|<span data-ttu-id="b94c6-133">String</span><span class="sxs-lookup"><span data-stu-id="b94c6-133">String</span></span>|<span data-ttu-id="b94c6-134">Der eindeutige Bezeichner für das Statusobjekt des Geräteschutzes.</span><span class="sxs-lookup"><span data-stu-id="b94c6-134">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="b94c6-135">Dies ist die Geräte-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b94c6-135">This is device id of the device</span></span>|
|<span data-ttu-id="b94c6-136">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b94c6-136">malwareProtectionEnabled</span></span>|<span data-ttu-id="b94c6-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-137">Boolean</span></span>|<span data-ttu-id="b94c6-138">Antischadsoftware ist aktiviert oder nicht</span><span class="sxs-lookup"><span data-stu-id="b94c6-138">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="b94c6-139">deviceState</span><span class="sxs-lookup"><span data-stu-id="b94c6-139">deviceState</span></span>|[<span data-ttu-id="b94c6-140">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="b94c6-140">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="b94c6-141">Status des Computers (wie Clean oder ausstehender vollständiger Scan oder ausstehender Neustart usw.).</span><span class="sxs-lookup"><span data-stu-id="b94c6-141">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="b94c6-142">Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.</span><span class="sxs-lookup"><span data-stu-id="b94c6-142">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="b94c6-143">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b94c6-143">realTimeProtectionEnabled</span></span>|<span data-ttu-id="b94c6-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-144">Boolean</span></span>|<span data-ttu-id="b94c6-145">Echtzeitschutz ist aktiviert oder nicht?</span><span class="sxs-lookup"><span data-stu-id="b94c6-145">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="b94c6-146">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="b94c6-146">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="b94c6-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-147">Boolean</span></span>|<span data-ttu-id="b94c6-148">Netzwerk Inspektionssystem aktiviert oder nicht?</span><span class="sxs-lookup"><span data-stu-id="b94c6-148">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="b94c6-149">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="b94c6-149">quickScanOverdue</span></span>|<span data-ttu-id="b94c6-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-150">Boolean</span></span>|<span data-ttu-id="b94c6-151">Schnellscan überfällig oder nicht?</span><span class="sxs-lookup"><span data-stu-id="b94c6-151">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="b94c6-152">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="b94c6-152">fullScanOverdue</span></span>|<span data-ttu-id="b94c6-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-153">Boolean</span></span>|<span data-ttu-id="b94c6-154">Vollständiger Scan überfällig oder nicht?</span><span class="sxs-lookup"><span data-stu-id="b94c6-154">Full scan overdue or not?</span></span>|
|<span data-ttu-id="b94c6-155">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="b94c6-155">signatureUpdateOverdue</span></span>|<span data-ttu-id="b94c6-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-156">Boolean</span></span>|<span data-ttu-id="b94c6-157">Signatur veraltet oder nicht?</span><span class="sxs-lookup"><span data-stu-id="b94c6-157">Signature out of date or not?</span></span>|
|<span data-ttu-id="b94c6-158">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="b94c6-158">rebootRequired</span></span>|<span data-ttu-id="b94c6-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-159">Boolean</span></span>|<span data-ttu-id="b94c6-160">Neustart erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="b94c6-160">Reboot required or not?</span></span>|
|<span data-ttu-id="b94c6-161">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="b94c6-161">fullScanRequired</span></span>|<span data-ttu-id="b94c6-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b94c6-162">Boolean</span></span>|<span data-ttu-id="b94c6-163">Vollständige Überprüfung erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="b94c6-163">Full scan required or not?</span></span>|
|<span data-ttu-id="b94c6-164">engineVersion</span><span class="sxs-lookup"><span data-stu-id="b94c6-164">engineVersion</span></span>|<span data-ttu-id="b94c6-165">String</span><span class="sxs-lookup"><span data-stu-id="b94c6-165">String</span></span>|<span data-ttu-id="b94c6-166">Version des aktuellen Endpoint Protection-Moduls</span><span class="sxs-lookup"><span data-stu-id="b94c6-166">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="b94c6-167">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="b94c6-167">signatureVersion</span></span>|<span data-ttu-id="b94c6-168">String</span><span class="sxs-lookup"><span data-stu-id="b94c6-168">String</span></span>|<span data-ttu-id="b94c6-169">Aktuelle Version der Malware-Definitionen</span><span class="sxs-lookup"><span data-stu-id="b94c6-169">Current malware definitions version</span></span>|
|<span data-ttu-id="b94c6-170">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="b94c6-170">antiMalwareVersion</span></span>|<span data-ttu-id="b94c6-171">String</span><span class="sxs-lookup"><span data-stu-id="b94c6-171">String</span></span>|<span data-ttu-id="b94c6-172">Aktuelle Antischadsoftware-Version</span><span class="sxs-lookup"><span data-stu-id="b94c6-172">Current anti malware version</span></span>|
|<span data-ttu-id="b94c6-173">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="b94c6-173">lastQuickScanDateTime</span></span>|<span data-ttu-id="b94c6-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b94c6-174">DateTimeOffset</span></span>|<span data-ttu-id="b94c6-175">Datum der letzten Schnellüberprüfung</span><span class="sxs-lookup"><span data-stu-id="b94c6-175">Last quick scan datetime</span></span>|
|<span data-ttu-id="b94c6-176">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="b94c6-176">lastFullScanDateTime</span></span>|<span data-ttu-id="b94c6-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b94c6-177">DateTimeOffset</span></span>|<span data-ttu-id="b94c6-178">Datum der letzten Schnellüberprüfung</span><span class="sxs-lookup"><span data-stu-id="b94c6-178">Last quick scan datetime</span></span>|
|<span data-ttu-id="b94c6-179">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="b94c6-179">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="b94c6-180">String</span><span class="sxs-lookup"><span data-stu-id="b94c6-180">String</span></span>|<span data-ttu-id="b94c6-181">Letzte Schnellscan-Signaturversion</span><span class="sxs-lookup"><span data-stu-id="b94c6-181">Last quick scan signature version</span></span>|
|<span data-ttu-id="b94c6-182">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="b94c6-182">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="b94c6-183">String</span><span class="sxs-lookup"><span data-stu-id="b94c6-183">String</span></span>|<span data-ttu-id="b94c6-184">Letzte vollständige Scan-Signaturversion</span><span class="sxs-lookup"><span data-stu-id="b94c6-184">Last full scan signature version</span></span>|
|<span data-ttu-id="b94c6-185">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b94c6-185">lastReportedDateTime</span></span>|<span data-ttu-id="b94c6-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b94c6-186">DateTimeOffset</span></span>|<span data-ttu-id="b94c6-187">Zeitpunkt des letzten Geräte Integritätsstatus</span><span class="sxs-lookup"><span data-stu-id="b94c6-187">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="b94c6-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="b94c6-188">Response</span></span>
<span data-ttu-id="b94c6-189">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b94c6-189">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b94c6-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b94c6-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="b94c6-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b94c6-191">Request</span></span>
<span data-ttu-id="b94c6-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b94c6-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 865

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b94c6-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="b94c6-193">Response</span></span>
<span data-ttu-id="b94c6-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b94c6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




