---
title: importedWindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentity-Objekts.
ms.openlocfilehash: 7b5d79893ec30c203d4272d652ac43a225a37ec5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065089"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="89b64-103">importedWindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="89b64-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="89b64-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="89b64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89b64-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="89b64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89b64-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="89b64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89b64-107">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="89b64-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89b64-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="89b64-108">Prerequisites</span></span>
<span data-ttu-id="89b64-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89b64-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89b64-111">Permission type</span></span>|<span data-ttu-id="89b64-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89b64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89b64-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89b64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89b64-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b64-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="89b64-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89b64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89b64-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89b64-116">Not supported.</span></span>|
|<span data-ttu-id="89b64-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89b64-117">Application</span></span>|<span data-ttu-id="89b64-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89b64-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89b64-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89b64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="89b64-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89b64-120">Request headers</span></span>
|<span data-ttu-id="89b64-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="89b64-121">Header</span></span>|<span data-ttu-id="89b64-122">Wert</span><span class="sxs-lookup"><span data-stu-id="89b64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89b64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89b64-123">Authorization</span></span>|<span data-ttu-id="89b64-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="89b64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89b64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89b64-125">Accept</span></span>|<span data-ttu-id="89b64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89b64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89b64-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89b64-127">Request body</span></span>
<span data-ttu-id="89b64-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="89b64-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="89b64-129">Die folgende Tabelle enthält die Eigenschaften, die beim Erstellen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="89b64-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="89b64-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89b64-130">Property</span></span>|<span data-ttu-id="89b64-131">Typ</span><span class="sxs-lookup"><span data-stu-id="89b64-131">Type</span></span>|<span data-ttu-id="89b64-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89b64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89b64-133">id</span><span class="sxs-lookup"><span data-stu-id="89b64-133">id</span></span>|<span data-ttu-id="89b64-134">String</span><span class="sxs-lookup"><span data-stu-id="89b64-134">String</span></span>|<span data-ttu-id="89b64-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="89b64-135">The GUID for the object</span></span>|
|<span data-ttu-id="89b64-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="89b64-136">orderIdentifier</span></span>|<span data-ttu-id="89b64-137">String</span><span class="sxs-lookup"><span data-stu-id="89b64-137">String</span></span>|<span data-ttu-id="89b64-138">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="89b64-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="89b64-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="89b64-139">serialNumber</span></span>|<span data-ttu-id="89b64-140">String</span><span class="sxs-lookup"><span data-stu-id="89b64-140">String</span></span>|<span data-ttu-id="89b64-141">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="89b64-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="89b64-142">productKey</span><span class="sxs-lookup"><span data-stu-id="89b64-142">productKey</span></span>|<span data-ttu-id="89b64-143">String</span><span class="sxs-lookup"><span data-stu-id="89b64-143">String</span></span>|<span data-ttu-id="89b64-144">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="89b64-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="89b64-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="89b64-145">hardwareIdentifier</span></span>|<span data-ttu-id="89b64-146">Binary</span><span class="sxs-lookup"><span data-stu-id="89b64-146">Binary</span></span>|<span data-ttu-id="89b64-147">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="89b64-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="89b64-148">state</span><span class="sxs-lookup"><span data-stu-id="89b64-148">state</span></span>|[<span data-ttu-id="89b64-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="89b64-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="89b64-150">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="89b64-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="89b64-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="89b64-151">Response</span></span>
<span data-ttu-id="89b64-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89b64-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89b64-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89b64-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="89b64-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89b64-154">Request</span></span>
<span data-ttu-id="89b64-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89b64-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 464

{
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="89b64-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="89b64-156">Response</span></span>
<span data-ttu-id="89b64-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89b64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```





