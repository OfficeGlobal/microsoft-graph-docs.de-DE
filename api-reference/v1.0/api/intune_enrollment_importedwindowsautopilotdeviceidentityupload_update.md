# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="3630c-101">importedWindowsAutopilotDeviceIdentityUpload aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3630c-101">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="3630c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3630c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3630c-103">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3630c-103">Update the properties of a [deviceAppManagement](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3630c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3630c-104">Prerequisites</span></span>
<span data-ttu-id="3630c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3630c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3630c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3630c-107">Permission type</span></span>|<span data-ttu-id="3630c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3630c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3630c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3630c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3630c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3630c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3630c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3630c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3630c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3630c-112">Not supported.</span></span>|
|<span data-ttu-id="3630c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3630c-113">Application</span></span>|<span data-ttu-id="3630c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3630c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3630c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3630c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="3630c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3630c-116">Request headers</span></span>
|<span data-ttu-id="3630c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3630c-117">Header</span></span>|<span data-ttu-id="3630c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3630c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3630c-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3630c-119">Authorization</span></span>|<span data-ttu-id="3630c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3630c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3630c-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="3630c-121">Accept</span></span>|<span data-ttu-id="3630c-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="3630c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3630c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3630c-123">Request body</span></span>
<span data-ttu-id="3630c-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3630c-124">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="3630c-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3630c-125">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="3630c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3630c-126">Property</span></span>|<span data-ttu-id="3630c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3630c-127">Type</span></span>|<span data-ttu-id="3630c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3630c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3630c-129">ID</span><span class="sxs-lookup"><span data-stu-id="3630c-129">id</span></span>|<span data-ttu-id="3630c-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3630c-130">String</span></span>|<span data-ttu-id="3630c-131">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="3630c-131">The GUID for the object</span></span>|
|<span data-ttu-id="3630c-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="3630c-132">createdDateTimeUtc</span></span>|<span data-ttu-id="3630c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3630c-133">DateTimeOffset</span></span>|<span data-ttu-id="3630c-134">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="3630c-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="3630c-135">Status</span><span class="sxs-lookup"><span data-stu-id="3630c-135">status</span></span>|[<span data-ttu-id="3630c-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="3630c-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="3630c-137">Upload Status.</span><span class="sxs-lookup"><span data-stu-id="3630c-137">Upload status.</span></span> <span data-ttu-id="3630c-138">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="3630c-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="3630c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="3630c-139">Response</span></span>
<span data-ttu-id="3630c-140">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eine aktualisierte [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3630c-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3630c-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3630c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="3630c-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3630c-142">Request</span></span>
<span data-ttu-id="3630c-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3630c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 89

{
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="3630c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="3630c-144">Response</span></span>
<span data-ttu-id="3630c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3630c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```







