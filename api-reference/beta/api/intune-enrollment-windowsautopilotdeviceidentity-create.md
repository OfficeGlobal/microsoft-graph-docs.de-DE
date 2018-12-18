---
title: Erstellen von windowsAutopilotDeviceIdentity
description: Erstellen eines neuen WindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
ms.openlocfilehash: 1e4a9d43755fff787efa08a8c727e6ddc35fa904
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316016"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="46f7f-103">Erstellen von windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="46f7f-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="46f7f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46f7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46f7f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46f7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46f7f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46f7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46f7f-107">Erstellen eines neuen [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="46f7f-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46f7f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46f7f-108">Prerequisites</span></span>
<span data-ttu-id="46f7f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46f7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46f7f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46f7f-111">Permission type</span></span>|<span data-ttu-id="46f7f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46f7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46f7f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46f7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46f7f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46f7f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46f7f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46f7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46f7f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46f7f-116">Not supported.</span></span>|
|<span data-ttu-id="46f7f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46f7f-117">Application</span></span>|<span data-ttu-id="46f7f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46f7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46f7f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46f7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="46f7f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46f7f-120">Request headers</span></span>
|<span data-ttu-id="46f7f-121">Header</span><span class="sxs-lookup"><span data-stu-id="46f7f-121">Header</span></span>|<span data-ttu-id="46f7f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="46f7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46f7f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="46f7f-123">Authorization</span></span>|<span data-ttu-id="46f7f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46f7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46f7f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46f7f-125">Accept</span></span>|<span data-ttu-id="46f7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46f7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46f7f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46f7f-127">Request body</span></span>
<span data-ttu-id="46f7f-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsAutopilotDeviceIdentity eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="46f7f-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="46f7f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsAutopilotDeviceIdentity erstellen.</span><span class="sxs-lookup"><span data-stu-id="46f7f-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="46f7f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46f7f-130">Property</span></span>|<span data-ttu-id="46f7f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="46f7f-131">Type</span></span>|<span data-ttu-id="46f7f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46f7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46f7f-133">id</span><span class="sxs-lookup"><span data-stu-id="46f7f-133">id</span></span>|<span data-ttu-id="46f7f-134">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-134">String</span></span>|<span data-ttu-id="46f7f-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="46f7f-135">The GUID for the object</span></span>|
|<span data-ttu-id="46f7f-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="46f7f-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="46f7f-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="46f7f-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="46f7f-138">Profil Zuordnungsstatus des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="46f7f-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="46f7f-139">Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="46f7f-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="46f7f-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="46f7f-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="46f7f-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="46f7f-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="46f7f-142">Profil Zuordnung detaillierter Status des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="46f7f-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="46f7f-143">Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="46f7f-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="46f7f-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="46f7f-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="46f7f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46f7f-145">DateTimeOffset</span></span>|<span data-ttu-id="46f7f-146">Profil festlegen Uhrzeit des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="46f7f-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="46f7f-147">orderIdentifier</span></span>|<span data-ttu-id="46f7f-148">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-148">String</span></span>|<span data-ttu-id="46f7f-149">Die Kennung des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="46f7f-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="46f7f-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="46f7f-151">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-151">String</span></span>|<span data-ttu-id="46f7f-152">Kennung des Geräts Autopilot Windows Bestellung.</span><span class="sxs-lookup"><span data-stu-id="46f7f-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="46f7f-153">serialNumber</span></span>|<span data-ttu-id="46f7f-154">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-154">String</span></span>|<span data-ttu-id="46f7f-155">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="46f7f-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-156">productKey</span><span class="sxs-lookup"><span data-stu-id="46f7f-156">productKey</span></span>|<span data-ttu-id="46f7f-157">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-157">String</span></span>|<span data-ttu-id="46f7f-158">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="46f7f-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="46f7f-159">manufacturer</span></span>|<span data-ttu-id="46f7f-160">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-160">String</span></span>|<span data-ttu-id="46f7f-161">OEM-Hersteller des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="46f7f-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-162">model</span><span class="sxs-lookup"><span data-stu-id="46f7f-162">model</span></span>|<span data-ttu-id="46f7f-163">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-163">String</span></span>|<span data-ttu-id="46f7f-164">Modellname des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="46f7f-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="46f7f-165">enrollmentState</span></span>|[<span data-ttu-id="46f7f-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="46f7f-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="46f7f-167">Registrierung-Zustand des Geräts Autopilot Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="46f7f-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="46f7f-168">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="46f7f-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="46f7f-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="46f7f-169">lastContactedDateTime</span></span>|<span data-ttu-id="46f7f-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46f7f-170">DateTimeOffset</span></span>|<span data-ttu-id="46f7f-171">Intune kontaktiert Datum Uhrzeit der letzten des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="46f7f-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46f7f-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="46f7f-172">addressableUserName</span></span>|<span data-ttu-id="46f7f-173">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-173">String</span></span>|<span data-ttu-id="46f7f-174">Adressierbaren Benutzername.</span><span class="sxs-lookup"><span data-stu-id="46f7f-174">Addressable user name.</span></span>|
|<span data-ttu-id="46f7f-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46f7f-175">userPrincipalName</span></span>|<span data-ttu-id="46f7f-176">String</span><span class="sxs-lookup"><span data-stu-id="46f7f-176">String</span></span>|<span data-ttu-id="46f7f-177">Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="46f7f-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="46f7f-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="46f7f-178">Response</span></span>
<span data-ttu-id="46f7f-179">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="46f7f-179">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46f7f-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46f7f-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="46f7f-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46f7f-181">Request</span></span>
<span data-ttu-id="46f7f-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46f7f-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 755

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
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="46f7f-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="46f7f-183">Response</span></span>
<span data-ttu-id="46f7f-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46f7f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 804

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
  "userPrincipalName": "User Principal Name value"
}
```





