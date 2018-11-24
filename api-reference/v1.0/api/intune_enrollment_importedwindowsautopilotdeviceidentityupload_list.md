# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="81ec1-101">Liste importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="81ec1-101">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="81ec1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="81ec1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81ec1-103">Listeneigenschaften und Beziehungen der [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="81ec1-103">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81ec1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="81ec1-104">Prerequisites</span></span>
<span data-ttu-id="81ec1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81ec1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81ec1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81ec1-107">Permission type</span></span>|<span data-ttu-id="81ec1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81ec1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81ec1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81ec1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="81ec1-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="81ec1-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="81ec1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81ec1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81ec1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81ec1-112">Not supported.</span></span>|
|<span data-ttu-id="81ec1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81ec1-113">Application</span></span>|<span data-ttu-id="81ec1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81ec1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81ec1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81ec1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="81ec1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81ec1-116">Request headers</span></span>
|<span data-ttu-id="81ec1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="81ec1-117">Header</span></span>|<span data-ttu-id="81ec1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="81ec1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81ec1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="81ec1-119">Authorization</span></span>|<span data-ttu-id="81ec1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="81ec1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81ec1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="81ec1-121">Accept</span></span>|<span data-ttu-id="81ec1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="81ec1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ec1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81ec1-123">Request body</span></span>
<span data-ttu-id="81ec1-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="81ec1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81ec1-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="81ec1-125">Response</span></span>
<span data-ttu-id="81ec1-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="81ec1-126">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ec1-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81ec1-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="81ec1-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81ec1-128">Request</span></span>
<span data-ttu-id="81ec1-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81ec1-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="81ec1-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="81ec1-130">Response</span></span>
<span data-ttu-id="81ec1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81ec1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```



