# <a name="list-devicecategories"></a><span data-ttu-id="4196d-101">Auflisten von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="4196d-101">List deviceCategories</span></span>

> <span data-ttu-id="4196d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4196d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4196d-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) auf.</span><span class="sxs-lookup"><span data-stu-id="4196d-103">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4196d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4196d-104">Prerequisites</span></span>
<span data-ttu-id="4196d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4196d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4196d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4196d-107">Permission type</span></span>|<span data-ttu-id="4196d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4196d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4196d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4196d-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4196d-110">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="4196d-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4196d-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4196d-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4196d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4196d-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4196d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4196d-113">Not supported.</span></span>|
|<span data-ttu-id="4196d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4196d-114">Application</span></span>|<span data-ttu-id="4196d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4196d-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4196d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4196d-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="4196d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4196d-117">Request headers</span></span>
|<span data-ttu-id="4196d-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4196d-118">Header</span></span>|<span data-ttu-id="4196d-119">Wert</span><span class="sxs-lookup"><span data-stu-id="4196d-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4196d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4196d-120">Authorization</span></span>|<span data-ttu-id="4196d-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4196d-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4196d-122">Accept</span><span class="sxs-lookup"><span data-stu-id="4196d-122">Accept</span></span>|<span data-ttu-id="4196d-123">application/json</span><span class="sxs-lookup"><span data-stu-id="4196d-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4196d-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4196d-124">Request body</span></span>
<span data-ttu-id="4196d-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4196d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4196d-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="4196d-126">Response</span></span>
<span data-ttu-id="4196d-127">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4196d-127">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune_shared_devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4196d-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4196d-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="4196d-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4196d-129">Request</span></span>
<span data-ttu-id="4196d-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4196d-130">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="4196d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4196d-131">Response</span></span>
<span data-ttu-id="4196d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4196d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



