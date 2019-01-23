---
title: importedWindowsAutopilotDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentity-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5fa7434a5ee9e5218e6bfd40bad6b6497b5f4b47
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404785"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="1ad2f-103">importedWindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1ad2f-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="1ad2f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1ad2f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ad2f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ad2f-107">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ad2f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1ad2f-108">Prerequisites</span></span>
<span data-ttu-id="1ad2f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ad2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1ad2f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ad2f-111">Permission type</span></span>|<span data-ttu-id="1ad2f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ad2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ad2f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ad2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ad2f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ad2f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1ad2f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ad2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ad2f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ad2f-116">Not supported.</span></span>|
|<span data-ttu-id="1ad2f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ad2f-117">Application</span></span>|<span data-ttu-id="1ad2f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ad2f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ad2f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ad2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="1ad2f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ad2f-120">Request headers</span></span>
|<span data-ttu-id="1ad2f-121">Header</span><span class="sxs-lookup"><span data-stu-id="1ad2f-121">Header</span></span>|<span data-ttu-id="1ad2f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1ad2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ad2f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1ad2f-123">Authorization</span></span>|<span data-ttu-id="1ad2f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1ad2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ad2f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1ad2f-125">Accept</span></span>|<span data-ttu-id="1ad2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ad2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ad2f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ad2f-127">Request body</span></span>
<span data-ttu-id="1ad2f-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="1ad2f-129">Die folgende Tabelle enthält die Eigenschaften, die beim Erstellen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="1ad2f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ad2f-130">Property</span></span>|<span data-ttu-id="1ad2f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1ad2f-131">Type</span></span>|<span data-ttu-id="1ad2f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ad2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ad2f-133">id</span><span class="sxs-lookup"><span data-stu-id="1ad2f-133">id</span></span>|<span data-ttu-id="1ad2f-134">String</span><span class="sxs-lookup"><span data-stu-id="1ad2f-134">String</span></span>|<span data-ttu-id="1ad2f-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="1ad2f-135">The GUID for the object</span></span>|
|<span data-ttu-id="1ad2f-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="1ad2f-136">orderIdentifier</span></span>|<span data-ttu-id="1ad2f-137">String</span><span class="sxs-lookup"><span data-stu-id="1ad2f-137">String</span></span>|<span data-ttu-id="1ad2f-138">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="1ad2f-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1ad2f-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1ad2f-139">serialNumber</span></span>|<span data-ttu-id="1ad2f-140">String</span><span class="sxs-lookup"><span data-stu-id="1ad2f-140">String</span></span>|<span data-ttu-id="1ad2f-141">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="1ad2f-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1ad2f-142">productKey</span><span class="sxs-lookup"><span data-stu-id="1ad2f-142">productKey</span></span>|<span data-ttu-id="1ad2f-143">String</span><span class="sxs-lookup"><span data-stu-id="1ad2f-143">String</span></span>|<span data-ttu-id="1ad2f-144">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="1ad2f-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1ad2f-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="1ad2f-145">hardwareIdentifier</span></span>|<span data-ttu-id="1ad2f-146">Binary</span><span class="sxs-lookup"><span data-stu-id="1ad2f-146">Binary</span></span>|<span data-ttu-id="1ad2f-147">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="1ad2f-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1ad2f-148">state</span><span class="sxs-lookup"><span data-stu-id="1ad2f-148">state</span></span>|[<span data-ttu-id="1ad2f-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="1ad2f-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="1ad2f-150">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="1ad2f-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="1ad2f-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ad2f-151">Response</span></span>
<span data-ttu-id="1ad2f-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ad2f-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ad2f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ad2f-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ad2f-154">Request</span></span>
<span data-ttu-id="1ad2f-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ad2f-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ad2f-156">Response</span></span>
<span data-ttu-id="1ad2f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ad2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




