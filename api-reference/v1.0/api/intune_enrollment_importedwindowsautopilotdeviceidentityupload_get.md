# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="46d7a-101">Abrufen von importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="46d7a-101">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="46d7a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46d7a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46d7a-103">Lesen der Eigenschaften und Beziehungen des [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="46d7a-103">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46d7a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46d7a-104">Prerequisites</span></span>
<span data-ttu-id="46d7a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="46d7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="46d7a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46d7a-107">Permission type</span></span>|<span data-ttu-id="46d7a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46d7a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46d7a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46d7a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="46d7a-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="46d7a-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="46d7a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46d7a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46d7a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46d7a-112">Not supported.</span></span>|
|<span data-ttu-id="46d7a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46d7a-113">Application</span></span>|<span data-ttu-id="46d7a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46d7a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46d7a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46d7a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46d7a-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="46d7a-116">Optional query parameters</span></span>
<span data-ttu-id="46d7a-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="46d7a-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="46d7a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46d7a-118">Request headers</span></span>
|<span data-ttu-id="46d7a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="46d7a-119">Header</span></span>|<span data-ttu-id="46d7a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="46d7a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46d7a-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="46d7a-121">Authorization</span></span>|<span data-ttu-id="46d7a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46d7a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46d7a-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="46d7a-123">Accept</span></span>|<span data-ttu-id="46d7a-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="46d7a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d7a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46d7a-125">Request body</span></span>
<span data-ttu-id="46d7a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="46d7a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46d7a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="46d7a-127">Response</span></span>
<span data-ttu-id="46d7a-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="46d7a-128">If successful, this method returns a `200 OK` response code and a [androidStoreApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46d7a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46d7a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="46d7a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46d7a-130">Request</span></span>
<span data-ttu-id="46d7a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46d7a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="46d7a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="46d7a-132">Response</span></span>
<span data-ttu-id="46d7a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46d7a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
    "id": "8d639524-9524-8d63-2495-638d2495638d",
    "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
    "status": "pending"
  }
}
```








