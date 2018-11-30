---
title: importedWindowsAutopilotDeviceIdentity erstellen
description: Erstellen eines neuen importedWindowsAutopilotDeviceIdentity-Objekts.
ms.openlocfilehash: 3a6923ba43d188ca1cf904285e1f430e1902f595
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018382"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="e3964-103">importedWindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="e3964-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="e3964-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3964-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3964-105">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3964-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3964-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3964-106">Prerequisites</span></span>
<span data-ttu-id="e3964-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3964-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3964-109">Permission type</span></span>|<span data-ttu-id="e3964-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3964-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3964-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3964-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3964-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3964-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e3964-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3964-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3964-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3964-114">Not supported.</span></span>|
|<span data-ttu-id="e3964-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3964-115">Application</span></span>|<span data-ttu-id="e3964-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3964-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3964-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3964-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e3964-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3964-118">Request headers</span></span>
|<span data-ttu-id="e3964-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e3964-119">Header</span></span>|<span data-ttu-id="e3964-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e3964-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3964-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3964-121">Authorization</span></span>|<span data-ttu-id="e3964-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3964-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3964-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3964-123">Accept</span></span>|<span data-ttu-id="e3964-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3964-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3964-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3964-125">Request body</span></span>
<span data-ttu-id="e3964-126">Geben Sie als Anforderungstext eine JSON-Darstellung des importedWindowsAutopilotDeviceIdentity-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e3964-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="e3964-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das importedWindowsAutopilotDeviceIdentity-Objekt erstellen.</span><span class="sxs-lookup"><span data-stu-id="e3964-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="e3964-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3964-128">Property</span></span>|<span data-ttu-id="e3964-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e3964-129">Type</span></span>|<span data-ttu-id="e3964-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3964-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3964-131">id</span><span class="sxs-lookup"><span data-stu-id="e3964-131">id</span></span>|<span data-ttu-id="e3964-132">String</span><span class="sxs-lookup"><span data-stu-id="e3964-132">String</span></span>|<span data-ttu-id="e3964-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="e3964-133">The GUID for the object</span></span>|
|<span data-ttu-id="e3964-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="e3964-134">orderIdentifier</span></span>|<span data-ttu-id="e3964-135">String</span><span class="sxs-lookup"><span data-stu-id="e3964-135">String</span></span>|<span data-ttu-id="e3964-136">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="e3964-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3964-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e3964-137">serialNumber</span></span>|<span data-ttu-id="e3964-138">String</span><span class="sxs-lookup"><span data-stu-id="e3964-138">String</span></span>|<span data-ttu-id="e3964-139">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="e3964-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3964-140">productKey</span><span class="sxs-lookup"><span data-stu-id="e3964-140">productKey</span></span>|<span data-ttu-id="e3964-141">String</span><span class="sxs-lookup"><span data-stu-id="e3964-141">String</span></span>|<span data-ttu-id="e3964-142">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="e3964-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3964-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="e3964-143">hardwareIdentifier</span></span>|<span data-ttu-id="e3964-144">Binary</span><span class="sxs-lookup"><span data-stu-id="e3964-144">Binary</span></span>|<span data-ttu-id="e3964-145">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="e3964-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3964-146">state</span><span class="sxs-lookup"><span data-stu-id="e3964-146">state</span></span>|[<span data-ttu-id="e3964-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="e3964-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="e3964-148">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="e3964-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="e3964-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3964-149">Response</span></span>
<span data-ttu-id="e3964-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e3964-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3964-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3964-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3964-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3964-152">Request</span></span>
<span data-ttu-id="e3964-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3964-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="e3964-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3964-154">Response</span></span>
<span data-ttu-id="e3964-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3964-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



