---
title: WindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAutopilotDeviceIdentity-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 018b45712ce7a35d2b7a19a09bca7ea7dd1650d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423867"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="0bfd1-103">WindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0bfd1-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="0bfd1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0bfd1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bfd1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bfd1-107">Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-107">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bfd1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0bfd1-108">Prerequisites</span></span>
<span data-ttu-id="0bfd1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bfd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0bfd1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bfd1-111">Permission type</span></span>|<span data-ttu-id="0bfd1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bfd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bfd1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bfd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bfd1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bfd1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0bfd1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bfd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bfd1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bfd1-116">Not supported.</span></span>|
|<span data-ttu-id="0bfd1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bfd1-117">Application</span></span>|<span data-ttu-id="0bfd1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bfd1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bfd1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bfd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="0bfd1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bfd1-120">Request headers</span></span>
|<span data-ttu-id="0bfd1-121">Header</span><span class="sxs-lookup"><span data-stu-id="0bfd1-121">Header</span></span>|<span data-ttu-id="0bfd1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0bfd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bfd1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0bfd1-123">Authorization</span></span>|<span data-ttu-id="0bfd1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bfd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bfd1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0bfd1-125">Accept</span></span>|<span data-ttu-id="0bfd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bfd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bfd1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bfd1-127">Request body</span></span>
<span data-ttu-id="0bfd1-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-128">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="0bfd1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-129">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="0bfd1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0bfd1-130">Property</span></span>|<span data-ttu-id="0bfd1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0bfd1-131">Type</span></span>|<span data-ttu-id="0bfd1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bfd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bfd1-133">id</span><span class="sxs-lookup"><span data-stu-id="0bfd1-133">id</span></span>|<span data-ttu-id="0bfd1-134">String</span><span class="sxs-lookup"><span data-stu-id="0bfd1-134">String</span></span>|<span data-ttu-id="0bfd1-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="0bfd1-135">The GUID for the object</span></span>|
|<span data-ttu-id="0bfd1-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="0bfd1-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="0bfd1-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="0bfd1-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="0bfd1-138">Profil Zuordnungsstatus des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="0bfd1-139">Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="0bfd1-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="0bfd1-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="0bfd1-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="0bfd1-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="0bfd1-142">Profil Zuordnung detaillierter Status des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="0bfd1-143">Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="0bfd1-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bfd1-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="0bfd1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bfd1-145">DateTimeOffset</span></span>|<span data-ttu-id="0bfd1-146">Profil festlegen Uhrzeit des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="0bfd1-147">orderIdentifier</span></span>|<span data-ttu-id="0bfd1-148">String</span><span class="sxs-lookup"><span data-stu-id="0bfd1-148">String</span></span>|<span data-ttu-id="0bfd1-149">Die Kennung des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="0bfd1-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="0bfd1-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bfd1-151">String</span></span>|<span data-ttu-id="0bfd1-152">Kennung des Geräts Autopilot Windows Bestellung.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0bfd1-153">serialNumber</span></span>|<span data-ttu-id="0bfd1-154">String</span><span class="sxs-lookup"><span data-stu-id="0bfd1-154">String</span></span>|<span data-ttu-id="0bfd1-155">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="0bfd1-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-156">productKey</span><span class="sxs-lookup"><span data-stu-id="0bfd1-156">productKey</span></span>|<span data-ttu-id="0bfd1-157">String</span><span class="sxs-lookup"><span data-stu-id="0bfd1-157">String</span></span>|<span data-ttu-id="0bfd1-158">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="0bfd1-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0bfd1-159">manufacturer</span></span>|<span data-ttu-id="0bfd1-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bfd1-160">String</span></span>|<span data-ttu-id="0bfd1-161">OEM-Hersteller des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-162">model</span><span class="sxs-lookup"><span data-stu-id="0bfd1-162">model</span></span>|<span data-ttu-id="0bfd1-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bfd1-163">String</span></span>|<span data-ttu-id="0bfd1-164">Modellname des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0bfd1-165">enrollmentState</span></span>|[<span data-ttu-id="0bfd1-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0bfd1-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="0bfd1-167">Registrierung-Zustand des Geräts Autopilot Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="0bfd1-168">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="0bfd1-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bfd1-169">lastContactedDateTime</span></span>|<span data-ttu-id="0bfd1-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bfd1-170">DateTimeOffset</span></span>|<span data-ttu-id="0bfd1-171">Intune kontaktiert Datum Uhrzeit der letzten des Geräts Autopilot Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0bfd1-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="0bfd1-172">addressableUserName</span></span>|<span data-ttu-id="0bfd1-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bfd1-173">String</span></span>|<span data-ttu-id="0bfd1-174">Adressierbaren Benutzername.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-174">Addressable user name.</span></span>|
|<span data-ttu-id="0bfd1-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0bfd1-175">userPrincipalName</span></span>|<span data-ttu-id="0bfd1-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bfd1-176">String</span></span>|<span data-ttu-id="0bfd1-177">Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="0bfd1-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bfd1-178">Response</span></span>
<span data-ttu-id="0bfd1-179">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-179">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bfd1-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bfd1-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bfd1-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bfd1-181">Request</span></span>
<span data-ttu-id="0bfd1-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="0bfd1-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bfd1-183">Response</span></span>
<span data-ttu-id="0bfd1-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bfd1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




