# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="f5c4b-101">enrollmentTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="f5c4b-101">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="f5c4b-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5c4b-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5c4b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5c4b-105">Auflisten von Eigenschaften und Beziehungen der [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5c4b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f5c4b-106">Prerequisites</span></span>
<span data-ttu-id="f5c4b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5c4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5c4b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5c4b-109">Permission type</span></span>|<span data-ttu-id="f5c4b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5c4b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5c4b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5c4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f5c4b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c4b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f5c4b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5c4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5c4b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5c4b-114">Not supported.</span></span>|
|<span data-ttu-id="f5c4b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5c4b-115">Application</span></span>|<span data-ttu-id="f5c4b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5c4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5c4b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5c4b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f5c4b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5c4b-118">Request headers</span></span>
|<span data-ttu-id="f5c4b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f5c4b-119">Header</span></span>|<span data-ttu-id="f5c4b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f5c4b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5c4b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5c4b-121">Authorization</span></span>|<span data-ttu-id="f5c4b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f5c4b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5c4b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f5c4b-123">Accept</span></span>|<span data-ttu-id="f5c4b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f5c4b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5c4b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5c4b-125">Request body</span></span>
<span data-ttu-id="f5c4b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5c4b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5c4b-127">Response</span></span>
<span data-ttu-id="f5c4b-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5c4b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5c4b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5c4b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5c4b-130">Request</span></span>
<span data-ttu-id="f5c4b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="f5c4b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5c4b-132">Response</span></span>
<span data-ttu-id="f5c4b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5c4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
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
  ]
}
```



