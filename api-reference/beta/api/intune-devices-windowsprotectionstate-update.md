---
title: WindowsProtectionState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsProtectionState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ce3c4fcd46e2d627f94e1728d38e9a8f0f91ad30
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939875"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="bd80b-103">WindowsProtectionState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bd80b-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="bd80b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd80b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd80b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd80b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd80b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd80b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd80b-107">Aktualisieren Sie die Eigenschaften eines [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd80b-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd80b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd80b-108">Prerequisites</span></span>
<span data-ttu-id="bd80b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd80b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd80b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd80b-111">Permission type</span></span>|<span data-ttu-id="bd80b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd80b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd80b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd80b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd80b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd80b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bd80b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd80b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd80b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd80b-116">Not supported.</span></span>|
|<span data-ttu-id="bd80b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd80b-117">Application</span></span>|<span data-ttu-id="bd80b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd80b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd80b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd80b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="bd80b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd80b-120">Request headers</span></span>
|<span data-ttu-id="bd80b-121">Header</span><span class="sxs-lookup"><span data-stu-id="bd80b-121">Header</span></span>|<span data-ttu-id="bd80b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd80b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd80b-123">Authorization</span></span>|<span data-ttu-id="bd80b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd80b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd80b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bd80b-125">Accept</span></span>|<span data-ttu-id="bd80b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd80b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd80b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd80b-127">Request body</span></span>
<span data-ttu-id="bd80b-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="bd80b-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="bd80b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="bd80b-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="bd80b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd80b-130">Property</span></span>|<span data-ttu-id="bd80b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bd80b-131">Type</span></span>|<span data-ttu-id="bd80b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd80b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd80b-133">id</span><span class="sxs-lookup"><span data-stu-id="bd80b-133">id</span></span>|<span data-ttu-id="bd80b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd80b-134">String</span></span>|<span data-ttu-id="bd80b-135">Der eindeutige Bezeichner für das Gerät Protection Status-Objekt.</span><span class="sxs-lookup"><span data-stu-id="bd80b-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="bd80b-136">Dies ist die Geräte-Id des Geräts</span><span class="sxs-lookup"><span data-stu-id="bd80b-136">This is device id of the device</span></span>|
|<span data-ttu-id="bd80b-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bd80b-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="bd80b-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-138">Boolean</span></span>|<span data-ttu-id="bd80b-139">Anti-Malware ist oder nicht aktiviert</span><span class="sxs-lookup"><span data-stu-id="bd80b-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="bd80b-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="bd80b-140">deviceState</span></span>|[<span data-ttu-id="bd80b-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="bd80b-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="bd80b-142">Zustand des Computers (wie bereinigen oder ausstehende vollständigen Scan oder Ausstehender Neustart usw.).</span><span class="sxs-lookup"><span data-stu-id="bd80b-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="bd80b-143">Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.</span><span class="sxs-lookup"><span data-stu-id="bd80b-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="bd80b-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bd80b-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="bd80b-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-145">Boolean</span></span>|<span data-ttu-id="bd80b-146">Echtzeit-Schutz ist oder nicht aktiviert?</span><span class="sxs-lookup"><span data-stu-id="bd80b-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="bd80b-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="bd80b-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="bd80b-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-148">Boolean</span></span>|<span data-ttu-id="bd80b-149">Netzwerk-Prüfung System aktiviert ist oder nicht?</span><span class="sxs-lookup"><span data-stu-id="bd80b-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="bd80b-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="bd80b-150">quickScanOverdue</span></span>|<span data-ttu-id="bd80b-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-151">Boolean</span></span>|<span data-ttu-id="bd80b-152">Quick scan überfällige oder nicht?</span><span class="sxs-lookup"><span data-stu-id="bd80b-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="bd80b-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="bd80b-153">fullScanOverdue</span></span>|<span data-ttu-id="bd80b-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-154">Boolean</span></span>|<span data-ttu-id="bd80b-155">Des vollständigen Scan überfällige oder nicht?</span><span class="sxs-lookup"><span data-stu-id="bd80b-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="bd80b-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="bd80b-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="bd80b-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-157">Boolean</span></span>|<span data-ttu-id="bd80b-158">Signatur veraltet oder nicht?</span><span class="sxs-lookup"><span data-stu-id="bd80b-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="bd80b-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="bd80b-159">rebootRequired</span></span>|<span data-ttu-id="bd80b-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-160">Boolean</span></span>|<span data-ttu-id="bd80b-161">Neustart erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="bd80b-161">Reboot required or not?</span></span>|
|<span data-ttu-id="bd80b-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="bd80b-162">fullScanRequired</span></span>|<span data-ttu-id="bd80b-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd80b-163">Boolean</span></span>|<span data-ttu-id="bd80b-164">Vollständigen Scan erforderlich oder nicht?</span><span class="sxs-lookup"><span data-stu-id="bd80b-164">Full scan required or not?</span></span>|
|<span data-ttu-id="bd80b-165">%ENGINEVERSION%</span><span class="sxs-lookup"><span data-stu-id="bd80b-165">engineVersion</span></span>|<span data-ttu-id="bd80b-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd80b-166">String</span></span>|<span data-ttu-id="bd80b-167">Aktuelle Endpoint Protection Datenbankmodul, version</span><span class="sxs-lookup"><span data-stu-id="bd80b-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="bd80b-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="bd80b-168">signatureVersion</span></span>|<span data-ttu-id="bd80b-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd80b-169">String</span></span>|<span data-ttu-id="bd80b-170">Aktuelle Version der Malware-Definitionen</span><span class="sxs-lookup"><span data-stu-id="bd80b-170">Current malware definitions version</span></span>|
|<span data-ttu-id="bd80b-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="bd80b-171">antiMalwareVersion</span></span>|<span data-ttu-id="bd80b-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd80b-172">String</span></span>|<span data-ttu-id="bd80b-173">Aktuelle anti-Malware-version</span><span class="sxs-lookup"><span data-stu-id="bd80b-173">Current anti malware version</span></span>|
|<span data-ttu-id="bd80b-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="bd80b-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="bd80b-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd80b-175">DateTimeOffset</span></span>|<span data-ttu-id="bd80b-176">Letzte schnell-Scan datetime</span><span class="sxs-lookup"><span data-stu-id="bd80b-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="bd80b-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="bd80b-177">lastFullScanDateTime</span></span>|<span data-ttu-id="bd80b-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd80b-178">DateTimeOffset</span></span>|<span data-ttu-id="bd80b-179">Letzte schnell-Scan datetime</span><span class="sxs-lookup"><span data-stu-id="bd80b-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="bd80b-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="bd80b-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="bd80b-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd80b-181">String</span></span>|<span data-ttu-id="bd80b-182">Letzte schnell-Scan Signatur-version</span><span class="sxs-lookup"><span data-stu-id="bd80b-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="bd80b-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="bd80b-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="bd80b-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd80b-184">String</span></span>|<span data-ttu-id="bd80b-185">Letzte vollständige Überprüfung Signatur-version</span><span class="sxs-lookup"><span data-stu-id="bd80b-185">Last full scan signature version</span></span>|
|<span data-ttu-id="bd80b-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd80b-186">lastReportedDateTime</span></span>|<span data-ttu-id="bd80b-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd80b-187">DateTimeOffset</span></span>|<span data-ttu-id="bd80b-188">Letzte Gerät Integritätsstatus gemeldet Zeit</span><span class="sxs-lookup"><span data-stu-id="bd80b-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="bd80b-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd80b-189">Response</span></span>
<span data-ttu-id="bd80b-190">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bd80b-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd80b-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd80b-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd80b-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd80b-192">Request</span></span>
<span data-ttu-id="bd80b-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd80b-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 804

{
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

### <a name="response"></a><span data-ttu-id="bd80b-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd80b-194">Response</span></span>
<span data-ttu-id="bd80b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd80b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





