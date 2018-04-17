# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="eb84b-101">Abrufen von „enrollmentTroubleshootingEvent“</span><span class="sxs-lookup"><span data-stu-id="eb84b-101">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="eb84b-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eb84b-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb84b-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb84b-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb84b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb84b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb84b-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="eb84b-105">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb84b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb84b-106">Prerequisites</span></span>
<span data-ttu-id="eb84b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb84b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb84b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb84b-109">Permission type</span></span>|<span data-ttu-id="eb84b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb84b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb84b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb84b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb84b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb84b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="eb84b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb84b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb84b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb84b-114">Not supported.</span></span>|
|<span data-ttu-id="eb84b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb84b-115">Application</span></span>|<span data-ttu-id="eb84b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb84b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb84b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb84b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb84b-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="eb84b-118">Optional query parameters</span></span>
<span data-ttu-id="eb84b-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb84b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eb84b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb84b-120">Request headers</span></span>
|<span data-ttu-id="eb84b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eb84b-121">Header</span></span>|<span data-ttu-id="eb84b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="eb84b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb84b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb84b-123">Authorization</span></span>|<span data-ttu-id="eb84b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb84b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb84b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eb84b-125">Accept</span></span>|<span data-ttu-id="eb84b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb84b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb84b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb84b-127">Request body</span></span>
<span data-ttu-id="eb84b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb84b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb84b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb84b-129">Response</span></span>
<span data-ttu-id="eb84b-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb84b-130">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb84b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb84b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb84b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb84b-132">Request</span></span>
<span data-ttu-id="eb84b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb84b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="eb84b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb84b-134">Response</span></span>
<span data-ttu-id="eb84b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb84b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
    "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "operatingSystem": "Operating System value",
    "osVersion": "Os Version value",
    "userId": "User Id value",
    "deviceId": "Device Id value",
    "enrollmentType": "userEnrollment",
    "failureCategory": "authentication",
    "failureReason": "Failure Reason value"
  }
}
```



