# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="20fa4-101">importedWindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="20fa4-101">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="20fa4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="20fa4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20fa4-103">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="20fa4-103">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20fa4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="20fa4-104">Prerequisites</span></span>
<span data-ttu-id="20fa4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20fa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20fa4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20fa4-107">Permission type</span></span>|<span data-ttu-id="20fa4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20fa4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20fa4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20fa4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="20fa4-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20fa4-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="20fa4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20fa4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20fa4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20fa4-112">Not supported.</span></span>|
|<span data-ttu-id="20fa4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20fa4-113">Application</span></span>|<span data-ttu-id="20fa4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20fa4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20fa4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20fa4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="20fa4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20fa4-116">Request headers</span></span>
|<span data-ttu-id="20fa4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="20fa4-117">Header</span></span>|<span data-ttu-id="20fa4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="20fa4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20fa4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="20fa4-119">Authorization</span></span>|<span data-ttu-id="20fa4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="20fa4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20fa4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="20fa4-121">Accept</span></span>|<span data-ttu-id="20fa4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="20fa4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20fa4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20fa4-123">Request body</span></span>
<span data-ttu-id="20fa4-124">Geben Sie als Anforderungstext eine JSON-Darstellung des importedWindowsAutopilotDeviceIdentity-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="20fa4-124">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="20fa4-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das importedWindowsAutopilotDeviceIdentity-Objekt erstellen.</span><span class="sxs-lookup"><span data-stu-id="20fa4-125">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="20fa4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20fa4-126">Property</span></span>|<span data-ttu-id="20fa4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="20fa4-127">Type</span></span>|<span data-ttu-id="20fa4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20fa4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20fa4-129">id</span><span class="sxs-lookup"><span data-stu-id="20fa4-129">id</span></span>|<span data-ttu-id="20fa4-130">String</span><span class="sxs-lookup"><span data-stu-id="20fa4-130">String</span></span>|<span data-ttu-id="20fa4-131">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="20fa4-131">The GUID for the object</span></span>|
|<span data-ttu-id="20fa4-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="20fa4-132">orderIdentifier</span></span>|<span data-ttu-id="20fa4-133">String</span><span class="sxs-lookup"><span data-stu-id="20fa4-133">String</span></span>|<span data-ttu-id="20fa4-134">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="20fa4-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="20fa4-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="20fa4-135">serialNumber</span></span>|<span data-ttu-id="20fa4-136">String</span><span class="sxs-lookup"><span data-stu-id="20fa4-136">String</span></span>|<span data-ttu-id="20fa4-137">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="20fa4-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="20fa4-138">productKey</span><span class="sxs-lookup"><span data-stu-id="20fa4-138">productKey</span></span>|<span data-ttu-id="20fa4-139">String</span><span class="sxs-lookup"><span data-stu-id="20fa4-139">String</span></span>|<span data-ttu-id="20fa4-140">Produktschlüssel des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="20fa4-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="20fa4-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="20fa4-141">hardwareIdentifier</span></span>|<span data-ttu-id="20fa4-142">Binary</span><span class="sxs-lookup"><span data-stu-id="20fa4-142">Binary</span></span>|<span data-ttu-id="20fa4-143">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="20fa4-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="20fa4-144">state</span><span class="sxs-lookup"><span data-stu-id="20fa4-144">state</span></span>|[<span data-ttu-id="20fa4-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="20fa4-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="20fa4-146">Aktueller Zustand des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="20fa4-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="20fa4-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="20fa4-147">Response</span></span>
<span data-ttu-id="20fa4-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="20fa4-148">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20fa4-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20fa4-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="20fa4-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20fa4-150">Request</span></span>
<span data-ttu-id="20fa4-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20fa4-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20fa4-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="20fa4-152">Response</span></span>
<span data-ttu-id="20fa4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20fa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



