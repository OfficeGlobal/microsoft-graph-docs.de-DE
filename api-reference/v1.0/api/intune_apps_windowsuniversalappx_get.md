# <a name="get-windowsuniversalappx"></a><span data-ttu-id="789ea-101">Abrufen von „windowsUniversalAppX“</span><span class="sxs-lookup"><span data-stu-id="789ea-101">Get windowsUniversalAppX</span></span>

> <span data-ttu-id="789ea-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="789ea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="789ea-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="789ea-103">Read properties and relationships of the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="789ea-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="789ea-104">Prerequisites</span></span>
<span data-ttu-id="789ea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="789ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="789ea-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="789ea-107">Permission type</span></span>|<span data-ttu-id="789ea-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="789ea-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="789ea-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="789ea-109">Delegated (work or school account)</span></span>|<span data-ttu-id="789ea-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="789ea-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="789ea-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="789ea-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="789ea-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="789ea-112">Not supported.</span></span>|
|<span data-ttu-id="789ea-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="789ea-113">Application</span></span>|<span data-ttu-id="789ea-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="789ea-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="789ea-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="789ea-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="789ea-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="789ea-116">Optional query parameters</span></span>
<span data-ttu-id="789ea-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="789ea-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="789ea-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="789ea-118">Request headers</span></span>
|<span data-ttu-id="789ea-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="789ea-119">Header</span></span>|<span data-ttu-id="789ea-120">Wert</span><span class="sxs-lookup"><span data-stu-id="789ea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="789ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="789ea-121">Authorization</span></span>|<span data-ttu-id="789ea-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="789ea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="789ea-123">Accept</span><span class="sxs-lookup"><span data-stu-id="789ea-123">Accept</span></span>|<span data-ttu-id="789ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="789ea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="789ea-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="789ea-125">Request body</span></span>
<span data-ttu-id="789ea-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="789ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="789ea-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="789ea-127">Response</span></span>
<span data-ttu-id="789ea-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="789ea-128">If successful, this method returns a `200 OK` response code and [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="789ea-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="789ea-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="789ea-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="789ea-130">Request</span></span>
<span data-ttu-id="789ea-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="789ea-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="789ea-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="789ea-132">Response</span></span>
<span data-ttu-id="789ea-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="789ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1450

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppX",
    "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "applicableArchitectures": "x86",
    "applicableDeviceTypes": "desktop",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "isBundle": true,
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true
    },
    "identityVersion": "Identity Version value"
  }
}
```



