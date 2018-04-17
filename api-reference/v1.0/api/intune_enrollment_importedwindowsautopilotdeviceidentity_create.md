# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="10a70-101">importedWindowsAutopilotDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="10a70-101">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="10a70-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10a70-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10a70-103">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="10a70-103">Create a new [managedMobileApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10a70-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10a70-104">Prerequisites</span></span>
<span data-ttu-id="10a70-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10a70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="10a70-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10a70-107">Permission type</span></span>|<span data-ttu-id="10a70-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10a70-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10a70-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10a70-109">Delegated (work or school account)</span></span>|<span data-ttu-id="10a70-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10a70-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10a70-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10a70-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10a70-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10a70-112">Not supported.</span></span>|
|<span data-ttu-id="10a70-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10a70-113">Application</span></span>|<span data-ttu-id="10a70-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10a70-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10a70-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10a70-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="10a70-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10a70-116">Request headers</span></span>
|<span data-ttu-id="10a70-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="10a70-117">Header</span></span>|<span data-ttu-id="10a70-118">Wert</span><span class="sxs-lookup"><span data-stu-id="10a70-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10a70-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="10a70-119">Authorization</span></span>|<span data-ttu-id="10a70-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10a70-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10a70-121">Accept</span><span class="sxs-lookup"><span data-stu-id="10a70-121">Accept</span></span>|<span data-ttu-id="10a70-122">application/json</span><span class="sxs-lookup"><span data-stu-id="10a70-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10a70-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10a70-123">Request body</span></span>
<span data-ttu-id="10a70-124">Geben Sie als Anforderungstext eine JSON-Darstellung des importedWindowsAutopilotDeviceIdentity-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="10a70-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="10a70-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das importedWindowsAutopilotDeviceIdentity-Objekt erstellen.</span><span class="sxs-lookup"><span data-stu-id="10a70-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="10a70-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10a70-126">Property</span></span>|<span data-ttu-id="10a70-127">Typ</span><span class="sxs-lookup"><span data-stu-id="10a70-127">Type</span></span>|<span data-ttu-id="10a70-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10a70-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10a70-129">id</span><span class="sxs-lookup"><span data-stu-id="10a70-129">id</span></span>|<span data-ttu-id="10a70-130">String</span><span class="sxs-lookup"><span data-stu-id="10a70-130">String</span></span>|<span data-ttu-id="10a70-131">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="10a70-131">The GUID for the object.</span></span>|
|<span data-ttu-id="10a70-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="10a70-132">orderIdentifier</span></span>|<span data-ttu-id="10a70-133">String</span><span class="sxs-lookup"><span data-stu-id="10a70-133">String</span></span>|<span data-ttu-id="10a70-134">Auftrags-ID des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="10a70-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10a70-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="10a70-135">serialNumber</span></span>|<span data-ttu-id="10a70-136">String</span><span class="sxs-lookup"><span data-stu-id="10a70-136">String</span></span>|<span data-ttu-id="10a70-137">Seriennummer des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="10a70-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10a70-138">productKey</span><span class="sxs-lookup"><span data-stu-id="10a70-138">productKey</span></span>|<span data-ttu-id="10a70-139">String</span><span class="sxs-lookup"><span data-stu-id="10a70-139">String</span></span>|<span data-ttu-id="10a70-140">Produktschlüssel des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="10a70-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10a70-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="10a70-141">hardwareIdentifier</span></span>|<span data-ttu-id="10a70-142">Binary</span><span class="sxs-lookup"><span data-stu-id="10a70-142">Binary</span></span>|<span data-ttu-id="10a70-143">Hardware-Blob des Windows AutoPilot-Geräts</span><span class="sxs-lookup"><span data-stu-id="10a70-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10a70-144">state</span><span class="sxs-lookup"><span data-stu-id="10a70-144">state</span></span>|[<span data-ttu-id="10a70-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="10a70-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="10a70-146">Aktueller Zustand des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="10a70-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="10a70-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="10a70-147">Response</span></span>
<span data-ttu-id="10a70-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="10a70-148">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10a70-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10a70-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="10a70-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10a70-150">Request</span></span>
<span data-ttu-id="10a70-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10a70-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10a70-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="10a70-152">Response</span></span>
<span data-ttu-id="10a70-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10a70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



