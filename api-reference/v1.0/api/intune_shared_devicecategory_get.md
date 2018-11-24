# <a name="get-devicecategory"></a><span data-ttu-id="9ed87-101">Abrufen von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="9ed87-101">Get deviceCategory</span></span>



> <span data-ttu-id="9ed87-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ed87-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ed87-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9ed87-103">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ed87-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ed87-104">Prerequisites</span></span>
<span data-ttu-id="9ed87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ed87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ed87-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ed87-107">Permission type</span></span>|<span data-ttu-id="9ed87-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ed87-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ed87-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ed87-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9ed87-110">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="9ed87-110">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9ed87-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ed87-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="9ed87-112">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="9ed87-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9ed87-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ed87-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9ed87-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ed87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ed87-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ed87-115">Not supported.</span></span>|
|<span data-ttu-id="9ed87-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ed87-116">Application</span></span>|<span data-ttu-id="9ed87-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ed87-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ed87-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ed87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ed87-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9ed87-119">Optional query parameters</span></span>
<span data-ttu-id="9ed87-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ed87-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ed87-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ed87-121">Request headers</span></span>
|<span data-ttu-id="9ed87-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ed87-122">Header</span></span>|<span data-ttu-id="9ed87-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9ed87-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ed87-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed87-124">Authorization</span></span>|<span data-ttu-id="9ed87-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ed87-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ed87-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9ed87-126">Accept</span></span>|<span data-ttu-id="9ed87-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ed87-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ed87-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ed87-128">Request body</span></span>
<span data-ttu-id="9ed87-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9ed87-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ed87-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ed87-130">Response</span></span>
<span data-ttu-id="9ed87-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9ed87-131">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ed87-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ed87-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ed87-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ed87-133">Request</span></span>
<span data-ttu-id="9ed87-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ed87-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="9ed87-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ed87-135">Response</span></span>
<span data-ttu-id="9ed87-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ed87-136">Here is an example of the response.</span></span> <span data-ttu-id="9ed87-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="9ed87-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9ed87-138">Eigenschaften von einer tatsächlichen Aufruf zurückgegeben variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="9ed87-138">Properties returned from an actual call vary according to context.</span></span>

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



