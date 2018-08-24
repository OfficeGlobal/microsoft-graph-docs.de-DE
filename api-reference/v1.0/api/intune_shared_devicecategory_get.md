# <a name="get-devicecategory"></a><span data-ttu-id="3bb6b-101">Abrufen von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="3bb6b-101">Get deviceCategory</span></span>

> <span data-ttu-id="3bb6b-102">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph werden in einer Vorschauversion bereitgestellt und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bb6b-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3bb6b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bb6b-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="3bb6b-105">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bb6b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3bb6b-106">Prerequisites</span></span>
<span data-ttu-id="3bb6b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3bb6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3bb6b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3bb6b-109">Permission type</span></span>|<span data-ttu-id="3bb6b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3bb6b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bb6b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3bb6b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3bb6b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bb6b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3bb6b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3bb6b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bb6b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bb6b-114">Not supported.</span></span>|
|<span data-ttu-id="3bb6b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3bb6b-115">Application</span></span>|<span data-ttu-id="3bb6b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bb6b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bb6b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bb6b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bb6b-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3bb6b-118">Optional query parameters</span></span>
<span data-ttu-id="3bb6b-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bb6b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3bb6b-120">Request headers</span></span>
|<span data-ttu-id="3bb6b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3bb6b-121">Header</span></span>|<span data-ttu-id="3bb6b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3bb6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bb6b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3bb6b-123">Authorization</span></span>|<span data-ttu-id="3bb6b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3bb6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bb6b-125">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="3bb6b-125">Accept</span></span>|<span data-ttu-id="3bb6b-126">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="3bb6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bb6b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3bb6b-127">Request body</span></span>
<span data-ttu-id="3bb6b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bb6b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bb6b-129">Response</span></span>
<span data-ttu-id="3bb6b-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-130">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bb6b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3bb6b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bb6b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bb6b-132">Request</span></span>
<span data-ttu-id="3bb6b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="3bb6b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bb6b-134">Response</span></span>
<span data-ttu-id="3bb6b-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-135">Here is an example of the response.</span></span> <span data-ttu-id="3bb6b-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3bb6b-137">Die von einem gegenwärtigen Anruf zurückgegebenen Eigenschaften variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-137">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```



