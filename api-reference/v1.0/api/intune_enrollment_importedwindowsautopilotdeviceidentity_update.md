# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="ff703-101">importedWindowsAutopilotDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ff703-101">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="ff703-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff703-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff703-103">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff703-103">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff703-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff703-104">Prerequisites</span></span>
<span data-ttu-id="ff703-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff703-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff703-107">Permission type</span></span>|<span data-ttu-id="ff703-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff703-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff703-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff703-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ff703-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff703-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff703-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff703-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff703-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff703-112">Not supported.</span></span>|
|<span data-ttu-id="ff703-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff703-113">Application</span></span>|<span data-ttu-id="ff703-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff703-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff703-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff703-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="ff703-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff703-116">Request headers</span></span>
|<span data-ttu-id="ff703-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ff703-117">Header</span></span>|<span data-ttu-id="ff703-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ff703-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff703-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff703-119">Authorization</span></span>|<span data-ttu-id="ff703-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff703-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff703-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ff703-121">Accept</span></span>|<span data-ttu-id="ff703-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ff703-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff703-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff703-123">Request body</span></span>
<span data-ttu-id="ff703-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ff703-124">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="ff703-125">Die folgende Tabelle enthält die Eigenschaften, die beim Erstellen des [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ff703-125">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="ff703-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff703-126">Property</span></span>|<span data-ttu-id="ff703-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ff703-127">Type</span></span>|<span data-ttu-id="ff703-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff703-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff703-129">id</span><span class="sxs-lookup"><span data-stu-id="ff703-129">id</span></span>|<span data-ttu-id="ff703-130">String</span><span class="sxs-lookup"><span data-stu-id="ff703-130">String</span></span>|<span data-ttu-id="ff703-131">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="ff703-131">The GUID for the object</span></span>|
|<span data-ttu-id="ff703-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff703-132">orderIdentifier</span></span>|<span data-ttu-id="ff703-133">String</span><span class="sxs-lookup"><span data-stu-id="ff703-133">String</span></span>|<span data-ttu-id="ff703-134">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="ff703-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ff703-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ff703-135">serialNumber</span></span>|<span data-ttu-id="ff703-136">String</span><span class="sxs-lookup"><span data-stu-id="ff703-136">String</span></span>|<span data-ttu-id="ff703-137">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="ff703-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ff703-138">productKey</span><span class="sxs-lookup"><span data-stu-id="ff703-138">productKey</span></span>|<span data-ttu-id="ff703-139">String</span><span class="sxs-lookup"><span data-stu-id="ff703-139">String</span></span>|<span data-ttu-id="ff703-140">Product Key des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="ff703-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ff703-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff703-141">hardwareIdentifier</span></span>|<span data-ttu-id="ff703-142">Binary</span><span class="sxs-lookup"><span data-stu-id="ff703-142">Binary</span></span>|<span data-ttu-id="ff703-143">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="ff703-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ff703-144">state</span><span class="sxs-lookup"><span data-stu-id="ff703-144">state</span></span>|[<span data-ttu-id="ff703-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="ff703-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="ff703-146">Aktueller Status des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="ff703-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="ff703-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff703-147">Response</span></span>
<span data-ttu-id="ff703-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff703-148">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff703-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff703-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff703-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff703-150">Request</span></span>
<span data-ttu-id="ff703-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff703-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff703-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff703-152">Response</span></span>
<span data-ttu-id="ff703-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff703-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



