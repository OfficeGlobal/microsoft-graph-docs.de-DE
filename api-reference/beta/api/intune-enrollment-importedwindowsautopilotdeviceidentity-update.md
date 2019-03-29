---
title: importedWindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b59b0374485dbaf3f23a137df2ed3b61a7bca97
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961238"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="6cc95-103">importedWindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6cc95-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="6cc95-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6cc95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cc95-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6cc95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cc95-106">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6cc95-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cc95-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6cc95-107">Prerequisites</span></span>
<span data-ttu-id="6cc95-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cc95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc95-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6cc95-110">Permission type</span></span>|<span data-ttu-id="6cc95-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6cc95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc95-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6cc95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc95-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cc95-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6cc95-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6cc95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc95-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cc95-115">Not supported.</span></span>|
|<span data-ttu-id="6cc95-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6cc95-116">Application</span></span>|<span data-ttu-id="6cc95-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cc95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc95-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cc95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="6cc95-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6cc95-119">Request headers</span></span>
|<span data-ttu-id="6cc95-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6cc95-120">Header</span></span>|<span data-ttu-id="6cc95-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6cc95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc95-122">Authorization</span></span>|<span data-ttu-id="6cc95-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6cc95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc95-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6cc95-124">Accept</span></span>|<span data-ttu-id="6cc95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc95-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6cc95-126">Request body</span></span>
<span data-ttu-id="6cc95-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6cc95-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="6cc95-128">Die folgende Tabelle enthält die Eigenschaften, die beim Erstellen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6cc95-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="6cc95-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6cc95-129">Property</span></span>|<span data-ttu-id="6cc95-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6cc95-130">Type</span></span>|<span data-ttu-id="6cc95-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6cc95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc95-132">id</span><span class="sxs-lookup"><span data-stu-id="6cc95-132">id</span></span>|<span data-ttu-id="6cc95-133">String</span><span class="sxs-lookup"><span data-stu-id="6cc95-133">String</span></span>|<span data-ttu-id="6cc95-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="6cc95-134">The GUID for the object</span></span>|
|<span data-ttu-id="6cc95-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="6cc95-135">orderIdentifier</span></span>|<span data-ttu-id="6cc95-136">String</span><span class="sxs-lookup"><span data-stu-id="6cc95-136">String</span></span>|<span data-ttu-id="6cc95-137">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="6cc95-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6cc95-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6cc95-138">serialNumber</span></span>|<span data-ttu-id="6cc95-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6cc95-139">String</span></span>|<span data-ttu-id="6cc95-140">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="6cc95-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6cc95-141">productKey</span><span class="sxs-lookup"><span data-stu-id="6cc95-141">productKey</span></span>|<span data-ttu-id="6cc95-142">String</span><span class="sxs-lookup"><span data-stu-id="6cc95-142">String</span></span>|<span data-ttu-id="6cc95-143">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="6cc95-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6cc95-144">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="6cc95-144">hardwareIdentifier</span></span>|<span data-ttu-id="6cc95-145">Binary</span><span class="sxs-lookup"><span data-stu-id="6cc95-145">Binary</span></span>|<span data-ttu-id="6cc95-146">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="6cc95-146">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6cc95-147">state</span><span class="sxs-lookup"><span data-stu-id="6cc95-147">state</span></span>|[<span data-ttu-id="6cc95-148">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="6cc95-148">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="6cc95-149">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="6cc95-149">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="6cc95-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cc95-150">Response</span></span>
<span data-ttu-id="6cc95-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cc95-151">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc95-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6cc95-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cc95-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cc95-153">Request</span></span>
<span data-ttu-id="6cc95-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6cc95-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cc95-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cc95-155">Response</span></span>
<span data-ttu-id="6cc95-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cc95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




