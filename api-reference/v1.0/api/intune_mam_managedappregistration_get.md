# <a name="get-managedappregistration"></a><span data-ttu-id="57d5d-101">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="57d5d-101">Get managedAppRegistration</span></span>

> <span data-ttu-id="57d5d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="57d5d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57d5d-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="57d5d-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57d5d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57d5d-104">Prerequisites</span></span>
<span data-ttu-id="57d5d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57d5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57d5d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57d5d-107">Permission type</span></span>|<span data-ttu-id="57d5d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57d5d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57d5d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57d5d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57d5d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="57d5d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="57d5d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57d5d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57d5d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57d5d-112">Not supported.</span></span>|
|<span data-ttu-id="57d5d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57d5d-113">Application</span></span>|<span data-ttu-id="57d5d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57d5d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57d5d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57d5d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57d5d-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="57d5d-116">Optional query parameters</span></span>
<span data-ttu-id="57d5d-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="57d5d-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="57d5d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57d5d-118">Request headers</span></span>
|<span data-ttu-id="57d5d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="57d5d-119">Header</span></span>|<span data-ttu-id="57d5d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="57d5d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57d5d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="57d5d-121">Authorization</span></span>|<span data-ttu-id="57d5d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="57d5d-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="57d5d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="57d5d-123">Accept</span></span>|<span data-ttu-id="57d5d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="57d5d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57d5d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57d5d-125">Request body</span></span>
<span data-ttu-id="57d5d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="57d5d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57d5d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="57d5d-127">Response</span></span>
<span data-ttu-id="57d5d-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="57d5d-128">If successful, this method returns a `200 OK` response code and a [section](../resources/intune_mam_managedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57d5d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57d5d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="57d5d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57d5d-130">Request</span></span>
<span data-ttu-id="57d5d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57d5d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="57d5d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="57d5d-132">Response</span></span>
<span data-ttu-id="57d5d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57d5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "5496aa60-aa60-5496-60aa-965460aa9654",
    "version": "Version value"
  }
}
```



