# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="6353b-101">Erstellen von importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="6353b-101">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="6353b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6353b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6353b-103">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6353b-103">Create a new [androidStoreApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6353b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6353b-104">Prerequisites</span></span>
<span data-ttu-id="6353b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6353b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6353b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6353b-107">Permission type</span></span>|<span data-ttu-id="6353b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6353b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6353b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6353b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6353b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6353b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6353b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6353b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6353b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6353b-112">Not supported.</span></span>|
|<span data-ttu-id="6353b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6353b-113">Application</span></span>|<span data-ttu-id="6353b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6353b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6353b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6353b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="6353b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6353b-116">Request headers</span></span>
|<span data-ttu-id="6353b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6353b-117">Header</span></span>|<span data-ttu-id="6353b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="6353b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6353b-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6353b-119">Authorization</span></span>|<span data-ttu-id="6353b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6353b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6353b-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6353b-121">Accept</span></span>|<span data-ttu-id="6353b-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="6353b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6353b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6353b-123">Request body</span></span>
<span data-ttu-id="6353b-124">Geben Sie im Anforderungstext eine JSON-Darstellung des importedWindowsAutopilotDeviceIdentityUpload-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6353b-124">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="6353b-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des  importedWindowsAutopilotDeviceIdentityUpload erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6353b-125">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="6353b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6353b-126">Property</span></span>|<span data-ttu-id="6353b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6353b-127">Type</span></span>|<span data-ttu-id="6353b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6353b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6353b-129">ID</span><span class="sxs-lookup"><span data-stu-id="6353b-129">id</span></span>|<span data-ttu-id="6353b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6353b-130">String</span></span>|<span data-ttu-id="6353b-131">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="6353b-131">The GUID for the object</span></span>|
|<span data-ttu-id="6353b-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="6353b-132">createdDateTimeUtc</span></span>|<span data-ttu-id="6353b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6353b-133">DateTimeOffset</span></span>|<span data-ttu-id="6353b-134">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="6353b-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="6353b-135">Status</span><span class="sxs-lookup"><span data-stu-id="6353b-135">status</span></span>|[<span data-ttu-id="6353b-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="6353b-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="6353b-137">Upload Status.</span><span class="sxs-lookup"><span data-stu-id="6353b-137">Upload status.</span></span> <span data-ttu-id="6353b-138">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="6353b-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="6353b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6353b-139">Response</span></span>
<span data-ttu-id="6353b-140">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201 Created` Antwortcode und ein [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6353b-140">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6353b-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6353b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="6353b-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6353b-142">Request</span></span>
<span data-ttu-id="6353b-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6353b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="6353b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="6353b-144">Response</span></span>
<span data-ttu-id="6353b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6353b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```








