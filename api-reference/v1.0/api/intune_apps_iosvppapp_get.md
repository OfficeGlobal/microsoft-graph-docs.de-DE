# <a name="get-iosvppapp"></a><span data-ttu-id="81d0c-101">iosVppApp abrufen</span><span class="sxs-lookup"><span data-stu-id="81d0c-101">Get iosVppApp</span></span>

> <span data-ttu-id="81d0c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="81d0c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81d0c-103">Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="81d0c-103">Read properties and relationships of the [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81d0c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="81d0c-104">Prerequisites</span></span>
<span data-ttu-id="81d0c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81d0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81d0c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81d0c-107">Permission type</span></span>|<span data-ttu-id="81d0c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81d0c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81d0c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81d0c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="81d0c-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81d0c-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="81d0c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81d0c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81d0c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81d0c-112">Not supported.</span></span>|
|<span data-ttu-id="81d0c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81d0c-113">Application</span></span>|<span data-ttu-id="81d0c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81d0c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81d0c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81d0c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81d0c-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="81d0c-116">Optional query parameters</span></span>
<span data-ttu-id="81d0c-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="81d0c-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="81d0c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81d0c-118">Request headers</span></span>
|<span data-ttu-id="81d0c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="81d0c-119">Header</span></span>|<span data-ttu-id="81d0c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="81d0c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81d0c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81d0c-121">Authorization</span></span>|<span data-ttu-id="81d0c-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="81d0c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81d0c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="81d0c-123">Accept</span></span>|<span data-ttu-id="81d0c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81d0c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81d0c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81d0c-125">Request body</span></span>
<span data-ttu-id="81d0c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="81d0c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81d0c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="81d0c-127">Response</span></span>
<span data-ttu-id="81d0c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosVppApp](../resources/intune_apps_iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81d0c-128">If successful, this method returns a `200 OK` response code and [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81d0c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81d0c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="81d0c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81d0c-130">Request</span></span>
<span data-ttu-id="81d0c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81d0c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="81d0c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="81d0c-132">Response</span></span>
<span data-ttu-id="81d0c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81d0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppApp",
    "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value"
  }
}
```



