---
title: WindowsAutopilotDeviceIdentity erstellen
description: Erstellen eines neuen windowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b29da1f5a9552aa14e51d9ef88c52b143144885c
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571508"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="f01ab-103">WindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="f01ab-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="f01ab-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f01ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f01ab-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f01ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f01ab-106">Erstellen eines neuen [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f01ab-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f01ab-107">Prerequisites</span></span>
<span data-ttu-id="f01ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f01ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f01ab-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f01ab-110">Permission type</span></span>|<span data-ttu-id="f01ab-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f01ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f01ab-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f01ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f01ab-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f01ab-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f01ab-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f01ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f01ab-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f01ab-115">Not supported.</span></span>|
|<span data-ttu-id="f01ab-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f01ab-116">Application</span></span>|<span data-ttu-id="f01ab-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f01ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f01ab-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f01ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="f01ab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f01ab-119">Request headers</span></span>
|<span data-ttu-id="f01ab-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f01ab-120">Header</span></span>|<span data-ttu-id="f01ab-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f01ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f01ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f01ab-122">Authorization</span></span>|<span data-ttu-id="f01ab-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f01ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f01ab-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f01ab-124">Accept</span></span>|<span data-ttu-id="f01ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f01ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f01ab-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f01ab-126">Request body</span></span>
<span data-ttu-id="f01ab-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsAutopilotDeviceIdentity-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f01ab-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="f01ab-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsAutopilotDeviceIdentity erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f01ab-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="f01ab-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f01ab-129">Property</span></span>|<span data-ttu-id="f01ab-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f01ab-130">Type</span></span>|<span data-ttu-id="f01ab-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f01ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f01ab-132">id</span><span class="sxs-lookup"><span data-stu-id="f01ab-132">id</span></span>|<span data-ttu-id="f01ab-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f01ab-133">String</span></span>|<span data-ttu-id="f01ab-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="f01ab-134">The GUID for the object</span></span>|
|<span data-ttu-id="f01ab-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="f01ab-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="f01ab-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="f01ab-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="f01ab-137">Profil Zuordnungsstatus des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="f01ab-138">Mögliche Werte: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f01ab-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="f01ab-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="f01ab-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="f01ab-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="f01ab-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="f01ab-141">Profilzuweisung detaillierter Status des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="f01ab-142">Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="f01ab-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="f01ab-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="f01ab-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="f01ab-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f01ab-144">DateTimeOffset</span></span>|<span data-ttu-id="f01ab-145">Festgelegte Zeit des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="f01ab-146">orderIdentifier</span></span>|<span data-ttu-id="f01ab-147">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-147">String</span></span>|<span data-ttu-id="f01ab-148">Auftragsbezeichner des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="f01ab-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="f01ab-150">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-150">String</span></span>|<span data-ttu-id="f01ab-151">Bestellkennung des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f01ab-152">serialNumber</span></span>|<span data-ttu-id="f01ab-153">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-153">String</span></span>|<span data-ttu-id="f01ab-154">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="f01ab-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-155">productKey</span><span class="sxs-lookup"><span data-stu-id="f01ab-155">productKey</span></span>|<span data-ttu-id="f01ab-156">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-156">String</span></span>|<span data-ttu-id="f01ab-157">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="f01ab-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-158">Hersteller</span><span class="sxs-lookup"><span data-stu-id="f01ab-158">manufacturer</span></span>|<span data-ttu-id="f01ab-159">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-159">String</span></span>|<span data-ttu-id="f01ab-160">OEM-Hersteller des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-161">model</span><span class="sxs-lookup"><span data-stu-id="f01ab-161">model</span></span>|<span data-ttu-id="f01ab-162">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-162">String</span></span>|<span data-ttu-id="f01ab-163">Modellname des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f01ab-164">enrollmentState</span></span>|[<span data-ttu-id="f01ab-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f01ab-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f01ab-166">InTune-Registrierungsstatus des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="f01ab-167">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f01ab-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f01ab-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f01ab-168">lastContactedDateTime</span></span>|<span data-ttu-id="f01ab-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f01ab-169">DateTimeOffset</span></span>|<span data-ttu-id="f01ab-170">InTune zuletzt kontaktierte Datum Uhrzeit des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="f01ab-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f01ab-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="f01ab-171">addressableUserName</span></span>|<span data-ttu-id="f01ab-172">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-172">String</span></span>|<span data-ttu-id="f01ab-173">Adressierbarer Benutzername.</span><span class="sxs-lookup"><span data-stu-id="f01ab-173">Addressable user name.</span></span>|
|<span data-ttu-id="f01ab-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f01ab-174">userPrincipalName</span></span>|<span data-ttu-id="f01ab-175">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-175">String</span></span>|<span data-ttu-id="f01ab-176">Benutzerprinzipal Name.</span><span class="sxs-lookup"><span data-stu-id="f01ab-176">User Principal Name.</span></span>|
|<span data-ttu-id="f01ab-177">resourceName</span><span class="sxs-lookup"><span data-stu-id="f01ab-177">resourceName</span></span>|<span data-ttu-id="f01ab-178">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-178">String</span></span>|<span data-ttu-id="f01ab-179">Ressourcen Name.</span><span class="sxs-lookup"><span data-stu-id="f01ab-179">Resource Name.</span></span>|
|<span data-ttu-id="f01ab-180">skuNumber</span><span class="sxs-lookup"><span data-stu-id="f01ab-180">skuNumber</span></span>|<span data-ttu-id="f01ab-181">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-181">String</span></span>|<span data-ttu-id="f01ab-182">SKU-Nummer</span><span class="sxs-lookup"><span data-stu-id="f01ab-182">SKU Number</span></span>|
|<span data-ttu-id="f01ab-183">systemFamily</span><span class="sxs-lookup"><span data-stu-id="f01ab-183">systemFamily</span></span>|<span data-ttu-id="f01ab-184">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-184">String</span></span>|<span data-ttu-id="f01ab-185">System Familie</span><span class="sxs-lookup"><span data-stu-id="f01ab-185">System Family</span></span>|
|<span data-ttu-id="f01ab-186">Eigenschaften azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="f01ab-186">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="f01ab-187">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-187">String</span></span>|<span data-ttu-id="f01ab-188">AAD-Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="f01ab-188">AAD Device ID</span></span>|
|<span data-ttu-id="f01ab-189">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f01ab-189">managedDeviceId</span></span>|<span data-ttu-id="f01ab-190">String</span><span class="sxs-lookup"><span data-stu-id="f01ab-190">String</span></span>|<span data-ttu-id="f01ab-191">Verwaltete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="f01ab-191">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="f01ab-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="f01ab-192">Response</span></span>
<span data-ttu-id="f01ab-193">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f01ab-193">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f01ab-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f01ab-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="f01ab-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f01ab-195">Request</span></span>
<span data-ttu-id="f01ab-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f01ab-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="f01ab-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="f01ab-197">Response</span></span>
<span data-ttu-id="f01ab-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f01ab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




