---
title: importedWindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af2e3e113c96f5b91a2c617f1c3d34dd26274bf0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144247"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="0261f-103">importedWindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0261f-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="0261f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0261f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0261f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0261f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0261f-106">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0261f-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0261f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0261f-107">Prerequisites</span></span>
<span data-ttu-id="0261f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0261f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0261f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0261f-110">Permission type</span></span>|<span data-ttu-id="0261f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0261f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0261f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0261f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0261f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0261f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0261f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0261f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0261f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0261f-115">Not supported.</span></span>|
|<span data-ttu-id="0261f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0261f-116">Application</span></span>|<span data-ttu-id="0261f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0261f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0261f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0261f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="0261f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0261f-119">Request headers</span></span>
|<span data-ttu-id="0261f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0261f-120">Header</span></span>|<span data-ttu-id="0261f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0261f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0261f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0261f-122">Authorization</span></span>|<span data-ttu-id="0261f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0261f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0261f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0261f-124">Accept</span></span>|<span data-ttu-id="0261f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0261f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0261f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0261f-126">Request body</span></span>
<span data-ttu-id="0261f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0261f-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="0261f-128">Die folgende Tabelle enthält die Eigenschaften, die beim Erstellen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0261f-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="0261f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0261f-129">Property</span></span>|<span data-ttu-id="0261f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0261f-130">Type</span></span>|<span data-ttu-id="0261f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0261f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0261f-132">id</span><span class="sxs-lookup"><span data-stu-id="0261f-132">id</span></span>|<span data-ttu-id="0261f-133">string</span><span class="sxs-lookup"><span data-stu-id="0261f-133">String</span></span>|<span data-ttu-id="0261f-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="0261f-134">The GUID for the object</span></span>|
|<span data-ttu-id="0261f-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="0261f-135">orderIdentifier</span></span>|<span data-ttu-id="0261f-136">String</span><span class="sxs-lookup"><span data-stu-id="0261f-136">String</span></span>|<span data-ttu-id="0261f-137">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="0261f-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0261f-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0261f-138">serialNumber</span></span>|<span data-ttu-id="0261f-139">String</span><span class="sxs-lookup"><span data-stu-id="0261f-139">String</span></span>|<span data-ttu-id="0261f-140">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="0261f-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0261f-141">productKey</span><span class="sxs-lookup"><span data-stu-id="0261f-141">productKey</span></span>|<span data-ttu-id="0261f-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0261f-142">String</span></span>|<span data-ttu-id="0261f-143">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="0261f-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0261f-144">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="0261f-144">hardwareIdentifier</span></span>|<span data-ttu-id="0261f-145">Binary</span><span class="sxs-lookup"><span data-stu-id="0261f-145">Binary</span></span>|<span data-ttu-id="0261f-146">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="0261f-146">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0261f-147">state</span><span class="sxs-lookup"><span data-stu-id="0261f-147">state</span></span>|[<span data-ttu-id="0261f-148">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="0261f-148">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="0261f-149">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="0261f-149">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="0261f-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="0261f-150">Response</span></span>
<span data-ttu-id="0261f-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0261f-151">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0261f-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0261f-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="0261f-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0261f-153">Request</span></span>
<span data-ttu-id="0261f-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0261f-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="0261f-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="0261f-155">Response</span></span>
<span data-ttu-id="0261f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0261f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




