# <a name="get-deviceappmanagement"></a><span data-ttu-id="4e2d1-101">Abrufen von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="4e2d1-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="4e2d1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e2d1-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4e2d1-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e2d1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e2d1-104">Prerequisites</span></span>
<span data-ttu-id="4e2d1-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="4e2d1-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e2d1-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="4e2d1-107">Beachten Sie, dass die entsprechende Berechtigung gemäß dem Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="4e2d1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e2d1-108">Permission type</span></span>|<span data-ttu-id="4e2d1-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e2d1-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e2d1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e2d1-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4e2d1-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e2d1-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="4e2d1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e2d1-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e2d1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e2d1-113">Not supported.</span></span>|
|<span data-ttu-id="4e2d1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e2d1-114">Application</span></span>|<span data-ttu-id="4e2d1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e2d1-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e2d1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e2d1-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e2d1-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4e2d1-117">Optional query parameters</span></span>
<span data-ttu-id="4e2d1-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4e2d1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e2d1-119">Request headers</span></span>
|<span data-ttu-id="4e2d1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4e2d1-120">Header</span></span>|<span data-ttu-id="4e2d1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4e2d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e2d1-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4e2d1-122">Authorization</span></span>|<span data-ttu-id="4e2d1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e2d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e2d1-124">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="4e2d1-124">Accept</span></span>|<span data-ttu-id="4e2d1-125">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="4e2d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e2d1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e2d1-126">Request body</span></span>
<span data-ttu-id="4e2d1-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e2d1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e2d1-128">Response</span></span>
<span data-ttu-id="4e2d1-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-129">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e2d1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e2d1-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e2d1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e2d1-131">Request</span></span>
<span data-ttu-id="4e2d1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="4e2d1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e2d1-133">Response</span></span>
<span data-ttu-id="4e2d1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e2d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



