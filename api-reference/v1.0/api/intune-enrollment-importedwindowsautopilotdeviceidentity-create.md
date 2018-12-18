---
title: importedWindowsAutopilotDeviceIdentity erstellen
description: Erstellen eines neuen importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
ms.openlocfilehash: 10dbaed9d10a0b37df9e229d501bb6e469847ea5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334293"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="4d718-103">importedWindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="4d718-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="4d718-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4d718-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d718-105">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d718-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d718-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d718-106">Prerequisites</span></span>
<span data-ttu-id="4d718-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d718-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d718-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d718-109">Permission type</span></span>|<span data-ttu-id="4d718-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d718-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d718-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d718-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d718-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d718-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d718-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d718-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d718-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d718-114">Not supported.</span></span>|
|<span data-ttu-id="4d718-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d718-115">Application</span></span>|<span data-ttu-id="4d718-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d718-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d718-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d718-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="4d718-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d718-118">Request headers</span></span>
|<span data-ttu-id="4d718-119">Header</span><span class="sxs-lookup"><span data-stu-id="4d718-119">Header</span></span>|<span data-ttu-id="4d718-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4d718-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d718-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4d718-121">Authorization</span></span>|<span data-ttu-id="4d718-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d718-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d718-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4d718-123">Accept</span></span>|<span data-ttu-id="4d718-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d718-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d718-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d718-125">Request body</span></span>
<span data-ttu-id="4d718-126">Geben Sie als Anforderungstext eine JSON-Darstellung des importedWindowsAutopilotDeviceIdentity-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4d718-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="4d718-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das importedWindowsAutopilotDeviceIdentity-Objekt erstellen.</span><span class="sxs-lookup"><span data-stu-id="4d718-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="4d718-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d718-128">Property</span></span>|<span data-ttu-id="4d718-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4d718-129">Type</span></span>|<span data-ttu-id="4d718-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d718-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d718-131">id</span><span class="sxs-lookup"><span data-stu-id="4d718-131">id</span></span>|<span data-ttu-id="4d718-132">String</span><span class="sxs-lookup"><span data-stu-id="4d718-132">String</span></span>|<span data-ttu-id="4d718-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="4d718-133">The GUID for the object</span></span>|
|<span data-ttu-id="4d718-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="4d718-134">orderIdentifier</span></span>|<span data-ttu-id="4d718-135">String</span><span class="sxs-lookup"><span data-stu-id="4d718-135">String</span></span>|<span data-ttu-id="4d718-136">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4d718-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4d718-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4d718-137">serialNumber</span></span>|<span data-ttu-id="4d718-138">String</span><span class="sxs-lookup"><span data-stu-id="4d718-138">String</span></span>|<span data-ttu-id="4d718-139">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4d718-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4d718-140">productKey</span><span class="sxs-lookup"><span data-stu-id="4d718-140">productKey</span></span>|<span data-ttu-id="4d718-141">String</span><span class="sxs-lookup"><span data-stu-id="4d718-141">String</span></span>|<span data-ttu-id="4d718-142">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4d718-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4d718-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="4d718-143">hardwareIdentifier</span></span>|<span data-ttu-id="4d718-144">Binary</span><span class="sxs-lookup"><span data-stu-id="4d718-144">Binary</span></span>|<span data-ttu-id="4d718-145">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4d718-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4d718-146">state</span><span class="sxs-lookup"><span data-stu-id="4d718-146">state</span></span>|[<span data-ttu-id="4d718-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="4d718-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="4d718-148">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="4d718-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="4d718-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d718-149">Response</span></span>
<span data-ttu-id="4d718-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4d718-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d718-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d718-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d718-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d718-152">Request</span></span>
<span data-ttu-id="4d718-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d718-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d718-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d718-154">Response</span></span>
<span data-ttu-id="4d718-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d718-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



