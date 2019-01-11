---
title: WindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea1200951231b43b2d2fd9242c241a54518fb1c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853536"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="d4bfe-103">WindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d4bfe-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="d4bfe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4bfe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4bfe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4bfe-107">Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-107">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4bfe-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4bfe-108">Prerequisites</span></span>
<span data-ttu-id="d4bfe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4bfe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4bfe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4bfe-111">Permission type</span></span>|<span data-ttu-id="d4bfe-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4bfe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4bfe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4bfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4bfe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4bfe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4bfe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4bfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4bfe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4bfe-116">Not supported.</span></span>|
|<span data-ttu-id="d4bfe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4bfe-117">Application</span></span>|<span data-ttu-id="d4bfe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4bfe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4bfe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4bfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="d4bfe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4bfe-120">Request headers</span></span>
|<span data-ttu-id="d4bfe-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4bfe-121">Header</span></span>|<span data-ttu-id="d4bfe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d4bfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4bfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4bfe-123">Authorization</span></span>|<span data-ttu-id="d4bfe-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4bfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4bfe-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4bfe-125">Accept</span></span>|<span data-ttu-id="d4bfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4bfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4bfe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4bfe-127">Request body</span></span>
<span data-ttu-id="d4bfe-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-128">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="d4bfe-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-129">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="d4bfe-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4bfe-130">Property</span></span>|<span data-ttu-id="d4bfe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d4bfe-131">Type</span></span>|<span data-ttu-id="d4bfe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4bfe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4bfe-133">id</span><span class="sxs-lookup"><span data-stu-id="d4bfe-133">id</span></span>|<span data-ttu-id="d4bfe-134">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-134">String</span></span>|<span data-ttu-id="d4bfe-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="d4bfe-135">The GUID for the object</span></span>|
|<span data-ttu-id="d4bfe-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="d4bfe-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="d4bfe-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="d4bfe-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="d4bfe-138">Profil Zuordnungsstatus des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="d4bfe-139">Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="d4bfe-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="d4bfe-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="d4bfe-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="d4bfe-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="d4bfe-142">Profil Zuordnung detaillierter Status des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="d4bfe-143">Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="d4bfe-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4bfe-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="d4bfe-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4bfe-145">DateTimeOffset</span></span>|<span data-ttu-id="d4bfe-146">Profil festlegen Uhrzeit des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="d4bfe-147">orderIdentifier</span></span>|<span data-ttu-id="d4bfe-148">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-148">String</span></span>|<span data-ttu-id="d4bfe-149">Die Kennung des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="d4bfe-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="d4bfe-151">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-151">String</span></span>|<span data-ttu-id="d4bfe-152">Kennung des Geräts Autopilot Windows Bestellung.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d4bfe-153">serialNumber</span></span>|<span data-ttu-id="d4bfe-154">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-154">String</span></span>|<span data-ttu-id="d4bfe-155">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="d4bfe-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-156">productKey</span><span class="sxs-lookup"><span data-stu-id="d4bfe-156">productKey</span></span>|<span data-ttu-id="d4bfe-157">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-157">String</span></span>|<span data-ttu-id="d4bfe-158">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="d4bfe-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d4bfe-159">manufacturer</span></span>|<span data-ttu-id="d4bfe-160">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-160">String</span></span>|<span data-ttu-id="d4bfe-161">OEM-Hersteller des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-162">model</span><span class="sxs-lookup"><span data-stu-id="d4bfe-162">model</span></span>|<span data-ttu-id="d4bfe-163">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-163">String</span></span>|<span data-ttu-id="d4bfe-164">Modellname des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d4bfe-165">enrollmentState</span></span>|[<span data-ttu-id="d4bfe-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d4bfe-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d4bfe-167">Registrierung-Zustand des Geräts Autopilot Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="d4bfe-168">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d4bfe-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4bfe-169">lastContactedDateTime</span></span>|<span data-ttu-id="d4bfe-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4bfe-170">DateTimeOffset</span></span>|<span data-ttu-id="d4bfe-171">Intune kontaktiert Datum Uhrzeit der letzten des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d4bfe-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="d4bfe-172">addressableUserName</span></span>|<span data-ttu-id="d4bfe-173">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-173">String</span></span>|<span data-ttu-id="d4bfe-174">Adressierbaren Benutzername.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-174">Addressable user name.</span></span>|
|<span data-ttu-id="d4bfe-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4bfe-175">userPrincipalName</span></span>|<span data-ttu-id="d4bfe-176">String</span><span class="sxs-lookup"><span data-stu-id="d4bfe-176">String</span></span>|<span data-ttu-id="d4bfe-177">Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="d4bfe-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4bfe-178">Response</span></span>
<span data-ttu-id="d4bfe-179">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-179">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4bfe-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4bfe-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4bfe-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4bfe-181">Request</span></span>
<span data-ttu-id="d4bfe-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 686

{
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

### <a name="response"></a><span data-ttu-id="d4bfe-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4bfe-183">Response</span></span>
<span data-ttu-id="d4bfe-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4bfe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





