# <a name="get-devicemanagement"></a><span data-ttu-id="b1ccb-101">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="b1ccb-101">Get deviceManagement</span></span>

> <span data-ttu-id="b1ccb-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1ccb-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1ccb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1ccb-105">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-105">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1ccb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1ccb-106">Prerequisites</span></span>
<span data-ttu-id="b1ccb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1ccb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1ccb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1ccb-109">Permission type</span></span>|<span data-ttu-id="b1ccb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1ccb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1ccb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1ccb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1ccb-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1ccb-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b1ccb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1ccb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1ccb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1ccb-114">Not supported.</span></span>|
|<span data-ttu-id="b1ccb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1ccb-115">Application</span></span>|<span data-ttu-id="b1ccb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1ccb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1ccb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1ccb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1ccb-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b1ccb-118">Optional query parameters</span></span>
<span data-ttu-id="b1ccb-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1ccb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1ccb-120">Request headers</span></span>
|<span data-ttu-id="b1ccb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b1ccb-121">Header</span></span>|<span data-ttu-id="b1ccb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b1ccb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1ccb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1ccb-123">Authorization</span></span>|<span data-ttu-id="b1ccb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1ccb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1ccb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1ccb-125">Accept</span></span>|<span data-ttu-id="b1ccb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1ccb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1ccb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1ccb-127">Request body</span></span>
<span data-ttu-id="b1ccb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1ccb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1ccb-129">Response</span></span>
<span data-ttu-id="b1ccb-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-130">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1ccb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1ccb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1ccb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1ccb-132">Request</span></span>
<span data-ttu-id="b1ccb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="b1ccb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1ccb-134">Response</span></span>
<span data-ttu-id="b1ccb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1ccb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```



