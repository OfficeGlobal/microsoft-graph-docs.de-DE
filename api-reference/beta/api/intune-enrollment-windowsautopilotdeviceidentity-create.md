---
title: WindowsAutopilotDeviceIdentity erstellen
description: Erstellen eines neuen windowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d87a27c120f4866725e2f91828e8c267f655e69c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175304"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="34d3b-103">WindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="34d3b-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="34d3b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34d3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34d3b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="34d3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34d3b-106">Erstellen eines neuen [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34d3b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="34d3b-107">Prerequisites</span></span>
<span data-ttu-id="34d3b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="34d3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="34d3b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34d3b-110">Permission type</span></span>|<span data-ttu-id="34d3b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34d3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34d3b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34d3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34d3b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34d3b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="34d3b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34d3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34d3b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34d3b-115">Not supported.</span></span>|
|<span data-ttu-id="34d3b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34d3b-116">Application</span></span>|<span data-ttu-id="34d3b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34d3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34d3b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34d3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="34d3b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34d3b-119">Request headers</span></span>
|<span data-ttu-id="34d3b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="34d3b-120">Header</span></span>|<span data-ttu-id="34d3b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="34d3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34d3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34d3b-122">Authorization</span></span>|<span data-ttu-id="34d3b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="34d3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34d3b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="34d3b-124">Accept</span></span>|<span data-ttu-id="34d3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34d3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34d3b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34d3b-126">Request body</span></span>
<span data-ttu-id="34d3b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsAutopilotDeviceIdentity-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="34d3b-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="34d3b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsAutopilotDeviceIdentity erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="34d3b-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="34d3b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34d3b-129">Property</span></span>|<span data-ttu-id="34d3b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="34d3b-130">Type</span></span>|<span data-ttu-id="34d3b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34d3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34d3b-132">id</span><span class="sxs-lookup"><span data-stu-id="34d3b-132">id</span></span>|<span data-ttu-id="34d3b-133">string</span><span class="sxs-lookup"><span data-stu-id="34d3b-133">String</span></span>|<span data-ttu-id="34d3b-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="34d3b-134">The GUID for the object</span></span>|
|<span data-ttu-id="34d3b-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="34d3b-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="34d3b-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="34d3b-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="34d3b-137">Profil Zuordnungsstatus des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="34d3b-138">Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="34d3b-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="34d3b-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="34d3b-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="34d3b-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="34d3b-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="34d3b-141">Profilzuweisung detaillierter Status des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="34d3b-142">Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="34d3b-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="34d3b-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="34d3b-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="34d3b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34d3b-144">DateTimeOffset</span></span>|<span data-ttu-id="34d3b-145">Festgelegte Zeit des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="34d3b-146">orderIdentifier</span></span>|<span data-ttu-id="34d3b-147">String</span><span class="sxs-lookup"><span data-stu-id="34d3b-147">String</span></span>|<span data-ttu-id="34d3b-148">Auftragsbezeichner des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="34d3b-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="34d3b-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34d3b-150">String</span></span>|<span data-ttu-id="34d3b-151">Bestellkennung des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="34d3b-152">serialNumber</span></span>|<span data-ttu-id="34d3b-153">String</span><span class="sxs-lookup"><span data-stu-id="34d3b-153">String</span></span>|<span data-ttu-id="34d3b-154">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="34d3b-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-155">productKey</span><span class="sxs-lookup"><span data-stu-id="34d3b-155">productKey</span></span>|<span data-ttu-id="34d3b-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34d3b-156">String</span></span>|<span data-ttu-id="34d3b-157">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="34d3b-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-158">manufacturer</span><span class="sxs-lookup"><span data-stu-id="34d3b-158">manufacturer</span></span>|<span data-ttu-id="34d3b-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34d3b-159">String</span></span>|<span data-ttu-id="34d3b-160">OEM-Hersteller des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-161">model</span><span class="sxs-lookup"><span data-stu-id="34d3b-161">model</span></span>|<span data-ttu-id="34d3b-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34d3b-162">String</span></span>|<span data-ttu-id="34d3b-163">Modellname des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="34d3b-164">enrollmentState</span></span>|[<span data-ttu-id="34d3b-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="34d3b-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="34d3b-166">InTune-Registrierungsstatus des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="34d3b-167">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="34d3b-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="34d3b-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="34d3b-168">lastContactedDateTime</span></span>|<span data-ttu-id="34d3b-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34d3b-169">DateTimeOffset</span></span>|<span data-ttu-id="34d3b-170">InTune zuletzt kontaktierte Datum Uhrzeit des Windows Autopilot-Geräts.</span><span class="sxs-lookup"><span data-stu-id="34d3b-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="34d3b-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="34d3b-171">addressableUserName</span></span>|<span data-ttu-id="34d3b-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34d3b-172">String</span></span>|<span data-ttu-id="34d3b-173">Adressierbarer Benutzername.</span><span class="sxs-lookup"><span data-stu-id="34d3b-173">Addressable user name.</span></span>|
|<span data-ttu-id="34d3b-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34d3b-174">userPrincipalName</span></span>|<span data-ttu-id="34d3b-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34d3b-175">String</span></span>|<span data-ttu-id="34d3b-176">Benutzerprinzipal Name.</span><span class="sxs-lookup"><span data-stu-id="34d3b-176">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="34d3b-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="34d3b-177">Response</span></span>
<span data-ttu-id="34d3b-178">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="34d3b-178">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34d3b-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34d3b-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="34d3b-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34d3b-180">Request</span></span>
<span data-ttu-id="34d3b-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34d3b-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34d3b-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="34d3b-182">Response</span></span>
<span data-ttu-id="34d3b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34d3b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




