---
title: Erstellen von windowsAutopilotDeviceIdentity
description: Erstellen eines neuen WindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 56d200bd53e94715ba102f6c96bba3e3b5dd892b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919099"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="af04a-103">Erstellen von windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="af04a-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="af04a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="af04a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af04a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="af04a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af04a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af04a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af04a-107">Erstellen eines neuen [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="af04a-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af04a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af04a-108">Prerequisites</span></span>
<span data-ttu-id="af04a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af04a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af04a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af04a-111">Permission type</span></span>|<span data-ttu-id="af04a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af04a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af04a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af04a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af04a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af04a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="af04a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af04a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af04a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af04a-116">Not supported.</span></span>|
|<span data-ttu-id="af04a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af04a-117">Application</span></span>|<span data-ttu-id="af04a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af04a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af04a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af04a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="af04a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af04a-120">Request headers</span></span>
|<span data-ttu-id="af04a-121">Header</span><span class="sxs-lookup"><span data-stu-id="af04a-121">Header</span></span>|<span data-ttu-id="af04a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="af04a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af04a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af04a-123">Authorization</span></span>|<span data-ttu-id="af04a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af04a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af04a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="af04a-125">Accept</span></span>|<span data-ttu-id="af04a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af04a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af04a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af04a-127">Request body</span></span>
<span data-ttu-id="af04a-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsAutopilotDeviceIdentity eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="af04a-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="af04a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsAutopilotDeviceIdentity erstellen.</span><span class="sxs-lookup"><span data-stu-id="af04a-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="af04a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af04a-130">Property</span></span>|<span data-ttu-id="af04a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="af04a-131">Type</span></span>|<span data-ttu-id="af04a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af04a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af04a-133">id</span><span class="sxs-lookup"><span data-stu-id="af04a-133">id</span></span>|<span data-ttu-id="af04a-134">String</span><span class="sxs-lookup"><span data-stu-id="af04a-134">String</span></span>|<span data-ttu-id="af04a-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="af04a-135">The GUID for the object</span></span>|
|<span data-ttu-id="af04a-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="af04a-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="af04a-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="af04a-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="af04a-138">Profil Zuordnungsstatus des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="af04a-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="af04a-139">Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="af04a-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="af04a-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="af04a-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="af04a-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="af04a-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="af04a-142">Profil Zuordnung detaillierter Status des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="af04a-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="af04a-143">Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="af04a-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="af04a-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="af04a-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="af04a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af04a-145">DateTimeOffset</span></span>|<span data-ttu-id="af04a-146">Profil festlegen Uhrzeit des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="af04a-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="af04a-147">orderIdentifier</span></span>|<span data-ttu-id="af04a-148">String</span><span class="sxs-lookup"><span data-stu-id="af04a-148">String</span></span>|<span data-ttu-id="af04a-149">Die Kennung des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="af04a-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="af04a-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="af04a-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af04a-151">String</span></span>|<span data-ttu-id="af04a-152">Kennung des Geräts Autopilot Windows Bestellung.</span><span class="sxs-lookup"><span data-stu-id="af04a-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="af04a-153">serialNumber</span></span>|<span data-ttu-id="af04a-154">String</span><span class="sxs-lookup"><span data-stu-id="af04a-154">String</span></span>|<span data-ttu-id="af04a-155">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="af04a-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-156">productKey</span><span class="sxs-lookup"><span data-stu-id="af04a-156">productKey</span></span>|<span data-ttu-id="af04a-157">String</span><span class="sxs-lookup"><span data-stu-id="af04a-157">String</span></span>|<span data-ttu-id="af04a-158">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="af04a-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="af04a-159">manufacturer</span></span>|<span data-ttu-id="af04a-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af04a-160">String</span></span>|<span data-ttu-id="af04a-161">OEM-Hersteller des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="af04a-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-162">model</span><span class="sxs-lookup"><span data-stu-id="af04a-162">model</span></span>|<span data-ttu-id="af04a-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af04a-163">String</span></span>|<span data-ttu-id="af04a-164">Modellname des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="af04a-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="af04a-165">enrollmentState</span></span>|[<span data-ttu-id="af04a-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="af04a-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="af04a-167">Registrierung-Zustand des Geräts Autopilot Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="af04a-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="af04a-168">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="af04a-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="af04a-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="af04a-169">lastContactedDateTime</span></span>|<span data-ttu-id="af04a-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af04a-170">DateTimeOffset</span></span>|<span data-ttu-id="af04a-171">Intune kontaktiert Datum Uhrzeit der letzten des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="af04a-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af04a-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="af04a-172">addressableUserName</span></span>|<span data-ttu-id="af04a-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af04a-173">String</span></span>|<span data-ttu-id="af04a-174">Adressierbaren Benutzername.</span><span class="sxs-lookup"><span data-stu-id="af04a-174">Addressable user name.</span></span>|
|<span data-ttu-id="af04a-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af04a-175">userPrincipalName</span></span>|<span data-ttu-id="af04a-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af04a-176">String</span></span>|<span data-ttu-id="af04a-177">Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="af04a-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="af04a-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="af04a-178">Response</span></span>
<span data-ttu-id="af04a-179">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="af04a-179">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af04a-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af04a-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="af04a-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af04a-181">Request</span></span>
<span data-ttu-id="af04a-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af04a-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af04a-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="af04a-183">Response</span></span>
<span data-ttu-id="af04a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af04a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





