---
title: WindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines windowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4132ebc9d93eae71712b04479c1139e1942a9979
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958732"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="2d532-103">WindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2d532-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="2d532-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d532-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d532-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2d532-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d532-106">Aktualisieren der Eigenschaften eines [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2d532-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d532-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2d532-107">Prerequisites</span></span>
<span data-ttu-id="2d532-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d532-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d532-110">Permission type</span></span>|<span data-ttu-id="2d532-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d532-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d532-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d532-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d532-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d532-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d532-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d532-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d532-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d532-115">Not supported.</span></span>|
|<span data-ttu-id="2d532-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d532-116">Application</span></span>|<span data-ttu-id="2d532-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d532-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d532-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d532-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="2d532-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d532-119">Request headers</span></span>
|<span data-ttu-id="2d532-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2d532-120">Header</span></span>|<span data-ttu-id="2d532-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2d532-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d532-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d532-122">Authorization</span></span>|<span data-ttu-id="2d532-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2d532-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d532-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2d532-124">Accept</span></span>|<span data-ttu-id="2d532-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d532-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d532-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d532-126">Request body</span></span>
<span data-ttu-id="2d532-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2d532-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="2d532-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2d532-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="2d532-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d532-129">Property</span></span>|<span data-ttu-id="2d532-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2d532-130">Type</span></span>|<span data-ttu-id="2d532-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d532-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d532-132">id</span><span class="sxs-lookup"><span data-stu-id="2d532-132">id</span></span>|<span data-ttu-id="2d532-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d532-133">String</span></span>|<span data-ttu-id="2d532-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="2d532-134">The GUID for the object</span></span>|
|<span data-ttu-id="2d532-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="2d532-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="2d532-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="2d532-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="2d532-137">Profil Zuordnungsstatus des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="2d532-138">Mögliche Werte: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2d532-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="2d532-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="2d532-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="2d532-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="2d532-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="2d532-141">Profilzuweisung detaillierter Status des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="2d532-142">Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="2d532-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="2d532-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d532-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="2d532-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d532-144">DateTimeOffset</span></span>|<span data-ttu-id="2d532-145">Festgelegte Zeit des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="2d532-146">orderIdentifier</span></span>|<span data-ttu-id="2d532-147">String</span><span class="sxs-lookup"><span data-stu-id="2d532-147">String</span></span>|<span data-ttu-id="2d532-148">Auftragsbezeichner des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="2d532-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="2d532-150">String</span><span class="sxs-lookup"><span data-stu-id="2d532-150">String</span></span>|<span data-ttu-id="2d532-151">Bestellkennung des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="2d532-152">serialNumber</span></span>|<span data-ttu-id="2d532-153">String</span><span class="sxs-lookup"><span data-stu-id="2d532-153">String</span></span>|<span data-ttu-id="2d532-154">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="2d532-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-155">productKey</span><span class="sxs-lookup"><span data-stu-id="2d532-155">productKey</span></span>|<span data-ttu-id="2d532-156">String</span><span class="sxs-lookup"><span data-stu-id="2d532-156">String</span></span>|<span data-ttu-id="2d532-157">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="2d532-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-158">Hersteller</span><span class="sxs-lookup"><span data-stu-id="2d532-158">manufacturer</span></span>|<span data-ttu-id="2d532-159">String</span><span class="sxs-lookup"><span data-stu-id="2d532-159">String</span></span>|<span data-ttu-id="2d532-160">OEM-Hersteller des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-161">model</span><span class="sxs-lookup"><span data-stu-id="2d532-161">model</span></span>|<span data-ttu-id="2d532-162">String</span><span class="sxs-lookup"><span data-stu-id="2d532-162">String</span></span>|<span data-ttu-id="2d532-163">Modellname des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2d532-164">enrollmentState</span></span>|[<span data-ttu-id="2d532-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2d532-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2d532-166">InTune-Registrierungsstatus des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="2d532-167">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2d532-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2d532-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d532-168">lastContactedDateTime</span></span>|<span data-ttu-id="2d532-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d532-169">DateTimeOffset</span></span>|<span data-ttu-id="2d532-170">InTune zuletzt kontaktierte Datum Uhrzeit des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d532-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2d532-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="2d532-171">addressableUserName</span></span>|<span data-ttu-id="2d532-172">String</span><span class="sxs-lookup"><span data-stu-id="2d532-172">String</span></span>|<span data-ttu-id="2d532-173">Adressierbarer Benutzername.</span><span class="sxs-lookup"><span data-stu-id="2d532-173">Addressable user name.</span></span>|
|<span data-ttu-id="2d532-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d532-174">userPrincipalName</span></span>|<span data-ttu-id="2d532-175">String</span><span class="sxs-lookup"><span data-stu-id="2d532-175">String</span></span>|<span data-ttu-id="2d532-176">Benutzerprinzipal Name.</span><span class="sxs-lookup"><span data-stu-id="2d532-176">User Principal Name.</span></span>|
|<span data-ttu-id="2d532-177">resourceName</span><span class="sxs-lookup"><span data-stu-id="2d532-177">resourceName</span></span>|<span data-ttu-id="2d532-178">String</span><span class="sxs-lookup"><span data-stu-id="2d532-178">String</span></span>|<span data-ttu-id="2d532-179">Ressourcen Name.</span><span class="sxs-lookup"><span data-stu-id="2d532-179">Resource Name.</span></span>|
|<span data-ttu-id="2d532-180">skuNumber</span><span class="sxs-lookup"><span data-stu-id="2d532-180">skuNumber</span></span>|<span data-ttu-id="2d532-181">String</span><span class="sxs-lookup"><span data-stu-id="2d532-181">String</span></span>|<span data-ttu-id="2d532-182">SKU-Nummer</span><span class="sxs-lookup"><span data-stu-id="2d532-182">SKU Number</span></span>|
|<span data-ttu-id="2d532-183">systemFamily</span><span class="sxs-lookup"><span data-stu-id="2d532-183">systemFamily</span></span>|<span data-ttu-id="2d532-184">String</span><span class="sxs-lookup"><span data-stu-id="2d532-184">String</span></span>|<span data-ttu-id="2d532-185">System Familie</span><span class="sxs-lookup"><span data-stu-id="2d532-185">System Family</span></span>|
|<span data-ttu-id="2d532-186">Eigenschaften azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="2d532-186">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="2d532-187">String</span><span class="sxs-lookup"><span data-stu-id="2d532-187">String</span></span>|<span data-ttu-id="2d532-188">AAD-Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="2d532-188">AAD Device ID</span></span>|
|<span data-ttu-id="2d532-189">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2d532-189">managedDeviceId</span></span>|<span data-ttu-id="2d532-190">String</span><span class="sxs-lookup"><span data-stu-id="2d532-190">String</span></span>|<span data-ttu-id="2d532-191">Verwaltete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="2d532-191">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="2d532-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d532-192">Response</span></span>
<span data-ttu-id="2d532-193">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2d532-193">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d532-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d532-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d532-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d532-195">Request</span></span>
<span data-ttu-id="2d532-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d532-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 1001

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="2d532-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d532-197">Response</span></span>
<span data-ttu-id="2d532-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d532-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1050

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value"
}
```




