---
title: importedWindowsAutopilotDeviceIdentity erstellen
description: Erstellen eines neuen importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c13f46d168bbb20d8166d063d3f12695ce02f50a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146256"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="5b97c-103">importedWindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="5b97c-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="5b97c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b97c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b97c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5b97c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b97c-106">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b97c-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b97c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b97c-107">Prerequisites</span></span>
<span data-ttu-id="5b97c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b97c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5b97c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b97c-110">Permission type</span></span>|<span data-ttu-id="5b97c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b97c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b97c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b97c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b97c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b97c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b97c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b97c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b97c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b97c-115">Not supported.</span></span>|
|<span data-ttu-id="5b97c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b97c-116">Application</span></span>|<span data-ttu-id="5b97c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b97c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b97c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b97c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="5b97c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b97c-119">Request headers</span></span>
|<span data-ttu-id="5b97c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b97c-120">Header</span></span>|<span data-ttu-id="5b97c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5b97c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b97c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b97c-122">Authorization</span></span>|<span data-ttu-id="5b97c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b97c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b97c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5b97c-124">Accept</span></span>|<span data-ttu-id="5b97c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b97c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b97c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b97c-126">Request body</span></span>
<span data-ttu-id="5b97c-127">Geben Sie als Anforderungstext eine JSON-Darstellung des importedWindowsAutopilotDeviceIdentity-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5b97c-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="5b97c-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das importedWindowsAutopilotDeviceIdentity-Objekt erstellen.</span><span class="sxs-lookup"><span data-stu-id="5b97c-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="5b97c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b97c-129">Property</span></span>|<span data-ttu-id="5b97c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5b97c-130">Type</span></span>|<span data-ttu-id="5b97c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b97c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b97c-132">id</span><span class="sxs-lookup"><span data-stu-id="5b97c-132">id</span></span>|<span data-ttu-id="5b97c-133">string</span><span class="sxs-lookup"><span data-stu-id="5b97c-133">String</span></span>|<span data-ttu-id="5b97c-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="5b97c-134">The GUID for the object</span></span>|
|<span data-ttu-id="5b97c-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b97c-135">orderIdentifier</span></span>|<span data-ttu-id="5b97c-136">String</span><span class="sxs-lookup"><span data-stu-id="5b97c-136">String</span></span>|<span data-ttu-id="5b97c-137">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="5b97c-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b97c-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5b97c-138">serialNumber</span></span>|<span data-ttu-id="5b97c-139">String</span><span class="sxs-lookup"><span data-stu-id="5b97c-139">String</span></span>|<span data-ttu-id="5b97c-140">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="5b97c-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b97c-141">productKey</span><span class="sxs-lookup"><span data-stu-id="5b97c-141">productKey</span></span>|<span data-ttu-id="5b97c-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b97c-142">String</span></span>|<span data-ttu-id="5b97c-143">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="5b97c-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b97c-144">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b97c-144">hardwareIdentifier</span></span>|<span data-ttu-id="5b97c-145">Binary</span><span class="sxs-lookup"><span data-stu-id="5b97c-145">Binary</span></span>|<span data-ttu-id="5b97c-146">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="5b97c-146">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b97c-147">state</span><span class="sxs-lookup"><span data-stu-id="5b97c-147">state</span></span>|[<span data-ttu-id="5b97c-148">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="5b97c-148">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="5b97c-149">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="5b97c-149">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="5b97c-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b97c-150">Response</span></span>
<span data-ttu-id="5b97c-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5b97c-151">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b97c-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b97c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b97c-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b97c-153">Request</span></span>
<span data-ttu-id="5b97c-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b97c-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="5b97c-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b97c-155">Response</span></span>
<span data-ttu-id="5b97c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b97c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




