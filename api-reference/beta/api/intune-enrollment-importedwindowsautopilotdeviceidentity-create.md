---
title: importedWindowsAutopilotDeviceIdentity erstellen
description: Erstellen eines neuen importedWindowsAutopilotDeviceIdentity-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c951e6b0489d5d42035d6f415efe64a8b6fb5d3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400725"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="25580-103">importedWindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="25580-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="25580-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="25580-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25580-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25580-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25580-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25580-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25580-107">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="25580-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25580-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="25580-108">Prerequisites</span></span>
<span data-ttu-id="25580-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="25580-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="25580-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25580-111">Permission type</span></span>|<span data-ttu-id="25580-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25580-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25580-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25580-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25580-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25580-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="25580-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25580-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25580-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25580-116">Not supported.</span></span>|
|<span data-ttu-id="25580-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25580-117">Application</span></span>|<span data-ttu-id="25580-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25580-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25580-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25580-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="25580-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25580-120">Request headers</span></span>
|<span data-ttu-id="25580-121">Header</span><span class="sxs-lookup"><span data-stu-id="25580-121">Header</span></span>|<span data-ttu-id="25580-122">Wert</span><span class="sxs-lookup"><span data-stu-id="25580-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25580-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="25580-123">Authorization</span></span>|<span data-ttu-id="25580-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="25580-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25580-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="25580-125">Accept</span></span>|<span data-ttu-id="25580-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25580-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25580-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25580-127">Request body</span></span>
<span data-ttu-id="25580-128">Geben Sie als Anforderungstext eine JSON-Darstellung des importedWindowsAutopilotDeviceIdentity-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="25580-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="25580-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das importedWindowsAutopilotDeviceIdentity-Objekt erstellen.</span><span class="sxs-lookup"><span data-stu-id="25580-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="25580-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="25580-130">Property</span></span>|<span data-ttu-id="25580-131">Typ</span><span class="sxs-lookup"><span data-stu-id="25580-131">Type</span></span>|<span data-ttu-id="25580-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25580-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25580-133">id</span><span class="sxs-lookup"><span data-stu-id="25580-133">id</span></span>|<span data-ttu-id="25580-134">String</span><span class="sxs-lookup"><span data-stu-id="25580-134">String</span></span>|<span data-ttu-id="25580-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="25580-135">The GUID for the object</span></span>|
|<span data-ttu-id="25580-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="25580-136">orderIdentifier</span></span>|<span data-ttu-id="25580-137">String</span><span class="sxs-lookup"><span data-stu-id="25580-137">String</span></span>|<span data-ttu-id="25580-138">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="25580-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="25580-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="25580-139">serialNumber</span></span>|<span data-ttu-id="25580-140">String</span><span class="sxs-lookup"><span data-stu-id="25580-140">String</span></span>|<span data-ttu-id="25580-141">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="25580-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="25580-142">productKey</span><span class="sxs-lookup"><span data-stu-id="25580-142">productKey</span></span>|<span data-ttu-id="25580-143">String</span><span class="sxs-lookup"><span data-stu-id="25580-143">String</span></span>|<span data-ttu-id="25580-144">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="25580-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="25580-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="25580-145">hardwareIdentifier</span></span>|<span data-ttu-id="25580-146">Binary</span><span class="sxs-lookup"><span data-stu-id="25580-146">Binary</span></span>|<span data-ttu-id="25580-147">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="25580-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="25580-148">state</span><span class="sxs-lookup"><span data-stu-id="25580-148">state</span></span>|[<span data-ttu-id="25580-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="25580-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="25580-150">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="25580-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="25580-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="25580-151">Response</span></span>
<span data-ttu-id="25580-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="25580-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25580-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25580-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="25580-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25580-154">Request</span></span>
<span data-ttu-id="25580-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25580-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25580-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="25580-156">Response</span></span>
<span data-ttu-id="25580-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25580-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




