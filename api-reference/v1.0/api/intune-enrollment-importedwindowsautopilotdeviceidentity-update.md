---
title: importedWindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
ms.openlocfilehash: ba28b77811082b6339987f173d874e453a91aa75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334265"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="4f1d9-103">importedWindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4f1d9-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="4f1d9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4f1d9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f1d9-105">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4f1d9-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f1d9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4f1d9-106">Prerequisites</span></span>
<span data-ttu-id="4f1d9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f1d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f1d9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f1d9-109">Permission type</span></span>|<span data-ttu-id="4f1d9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f1d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f1d9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f1d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f1d9-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f1d9-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4f1d9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f1d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f1d9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f1d9-114">Not supported.</span></span>|
|<span data-ttu-id="4f1d9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f1d9-115">Application</span></span>|<span data-ttu-id="4f1d9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f1d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f1d9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f1d9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="4f1d9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f1d9-118">Request headers</span></span>
|<span data-ttu-id="4f1d9-119">Header</span><span class="sxs-lookup"><span data-stu-id="4f1d9-119">Header</span></span>|<span data-ttu-id="4f1d9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4f1d9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f1d9-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4f1d9-121">Authorization</span></span>|<span data-ttu-id="4f1d9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f1d9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f1d9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4f1d9-123">Accept</span></span>|<span data-ttu-id="4f1d9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f1d9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f1d9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f1d9-125">Request body</span></span>
<span data-ttu-id="4f1d9-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4f1d9-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="4f1d9-127">Die folgende Tabelle enthält die Eigenschaften, die beim Erstellen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4f1d9-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="4f1d9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f1d9-128">Property</span></span>|<span data-ttu-id="4f1d9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4f1d9-129">Type</span></span>|<span data-ttu-id="4f1d9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f1d9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f1d9-131">id</span><span class="sxs-lookup"><span data-stu-id="4f1d9-131">id</span></span>|<span data-ttu-id="4f1d9-132">String</span><span class="sxs-lookup"><span data-stu-id="4f1d9-132">String</span></span>|<span data-ttu-id="4f1d9-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="4f1d9-133">The GUID for the object</span></span>|
|<span data-ttu-id="4f1d9-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f1d9-134">orderIdentifier</span></span>|<span data-ttu-id="4f1d9-135">String</span><span class="sxs-lookup"><span data-stu-id="4f1d9-135">String</span></span>|<span data-ttu-id="4f1d9-136">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4f1d9-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4f1d9-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4f1d9-137">serialNumber</span></span>|<span data-ttu-id="4f1d9-138">String</span><span class="sxs-lookup"><span data-stu-id="4f1d9-138">String</span></span>|<span data-ttu-id="4f1d9-139">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4f1d9-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4f1d9-140">productKey</span><span class="sxs-lookup"><span data-stu-id="4f1d9-140">productKey</span></span>|<span data-ttu-id="4f1d9-141">String</span><span class="sxs-lookup"><span data-stu-id="4f1d9-141">String</span></span>|<span data-ttu-id="4f1d9-142">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4f1d9-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4f1d9-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f1d9-143">hardwareIdentifier</span></span>|<span data-ttu-id="4f1d9-144">Binary</span><span class="sxs-lookup"><span data-stu-id="4f1d9-144">Binary</span></span>|<span data-ttu-id="4f1d9-145">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="4f1d9-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4f1d9-146">state</span><span class="sxs-lookup"><span data-stu-id="4f1d9-146">state</span></span>|[<span data-ttu-id="4f1d9-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="4f1d9-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="4f1d9-148">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="4f1d9-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="4f1d9-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f1d9-149">Response</span></span>
<span data-ttu-id="4f1d9-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f1d9-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f1d9-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f1d9-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f1d9-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f1d9-152">Request</span></span>
<span data-ttu-id="4f1d9-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f1d9-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="4f1d9-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f1d9-154">Response</span></span>
<span data-ttu-id="4f1d9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f1d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



