---
title: importedWindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a81e7b8291bab7698869c60d5403fd07be08cb5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261334"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="44e36-103">importedWindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="44e36-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="44e36-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="44e36-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44e36-105">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="44e36-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44e36-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44e36-106">Prerequisites</span></span>
<span data-ttu-id="44e36-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="44e36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44e36-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44e36-109">Permission type</span></span>|<span data-ttu-id="44e36-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44e36-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44e36-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44e36-111">Delegated (work or school account)</span></span>|<span data-ttu-id="44e36-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e36-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="44e36-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44e36-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44e36-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44e36-114">Not supported.</span></span>|
|<span data-ttu-id="44e36-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44e36-115">Application</span></span>|<span data-ttu-id="44e36-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44e36-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44e36-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44e36-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="44e36-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44e36-118">Request headers</span></span>
|<span data-ttu-id="44e36-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="44e36-119">Header</span></span>|<span data-ttu-id="44e36-120">Wert</span><span class="sxs-lookup"><span data-stu-id="44e36-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44e36-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44e36-121">Authorization</span></span>|<span data-ttu-id="44e36-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44e36-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44e36-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="44e36-123">Accept</span></span>|<span data-ttu-id="44e36-124">application/json</span><span class="sxs-lookup"><span data-stu-id="44e36-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44e36-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44e36-125">Request body</span></span>
<span data-ttu-id="44e36-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="44e36-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="44e36-127">Die folgende Tabelle enthält die Eigenschaften, die beim Erstellen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="44e36-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="44e36-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44e36-128">Property</span></span>|<span data-ttu-id="44e36-129">Typ</span><span class="sxs-lookup"><span data-stu-id="44e36-129">Type</span></span>|<span data-ttu-id="44e36-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44e36-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44e36-131">id</span><span class="sxs-lookup"><span data-stu-id="44e36-131">id</span></span>|<span data-ttu-id="44e36-132">string</span><span class="sxs-lookup"><span data-stu-id="44e36-132">String</span></span>|<span data-ttu-id="44e36-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="44e36-133">The GUID for the object</span></span>|
|<span data-ttu-id="44e36-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="44e36-134">orderIdentifier</span></span>|<span data-ttu-id="44e36-135">String</span><span class="sxs-lookup"><span data-stu-id="44e36-135">String</span></span>|<span data-ttu-id="44e36-136">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="44e36-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44e36-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="44e36-137">serialNumber</span></span>|<span data-ttu-id="44e36-138">String</span><span class="sxs-lookup"><span data-stu-id="44e36-138">String</span></span>|<span data-ttu-id="44e36-139">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="44e36-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44e36-140">productKey</span><span class="sxs-lookup"><span data-stu-id="44e36-140">productKey</span></span>|<span data-ttu-id="44e36-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44e36-141">String</span></span>|<span data-ttu-id="44e36-142">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="44e36-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44e36-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="44e36-143">hardwareIdentifier</span></span>|<span data-ttu-id="44e36-144">Binary</span><span class="sxs-lookup"><span data-stu-id="44e36-144">Binary</span></span>|<span data-ttu-id="44e36-145">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="44e36-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44e36-146">state</span><span class="sxs-lookup"><span data-stu-id="44e36-146">state</span></span>|[<span data-ttu-id="44e36-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="44e36-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="44e36-148">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="44e36-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="44e36-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="44e36-149">Response</span></span>
<span data-ttu-id="44e36-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44e36-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44e36-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44e36-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="44e36-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44e36-152">Request</span></span>
<span data-ttu-id="44e36-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44e36-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44e36-154">Reaktion</span><span class="sxs-lookup"><span data-stu-id="44e36-154">Response</span></span>
<span data-ttu-id="44e36-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44e36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



