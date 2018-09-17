# <a name="get-reportroot"></a><span data-ttu-id="51736-101">Abrufen von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="51736-101">Get reportRoot</span></span>

> <span data-ttu-id="51736-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51736-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51736-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="51736-103">Read properties and relationships of the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51736-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51736-104">Prerequisites</span></span>
<span data-ttu-id="51736-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51736-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51736-107">Permission type</span></span>|<span data-ttu-id="51736-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51736-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51736-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51736-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="51736-110">&nbsp; &nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="51736-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="51736-111">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51736-111">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="51736-112">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="51736-112">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="51736-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="51736-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="51736-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51736-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51736-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51736-115">Not supported.</span></span>|
|<span data-ttu-id="51736-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51736-116">Application</span></span>|<span data-ttu-id="51736-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51736-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51736-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51736-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51736-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="51736-119">Optional query parameters</span></span>
<span data-ttu-id="51736-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51736-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51736-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51736-121">Request headers</span></span>
|<span data-ttu-id="51736-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="51736-122">Header</span></span>|<span data-ttu-id="51736-123">Wert</span><span class="sxs-lookup"><span data-stu-id="51736-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51736-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="51736-124">Authorization</span></span>|<span data-ttu-id="51736-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51736-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51736-126">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="51736-126">Accept</span></span>|<span data-ttu-id="51736-127">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="51736-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51736-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51736-128">Request body</span></span>
<span data-ttu-id="51736-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="51736-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51736-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="51736-130">Response</span></span>
<span data-ttu-id="51736-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [reportRoot](../resources/intune_shared_reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="51736-131">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51736-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51736-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="51736-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51736-133">Request</span></span>
<span data-ttu-id="51736-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51736-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="51736-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="51736-135">Response</span></span>
<span data-ttu-id="51736-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51736-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```








