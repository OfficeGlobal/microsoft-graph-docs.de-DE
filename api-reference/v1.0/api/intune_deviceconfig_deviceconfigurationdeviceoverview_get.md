# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="ca535-101">deviceConfigurationDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="ca535-101">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="ca535-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ca535-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca535-103">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ca535-103">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca535-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ca535-104">Prerequisites</span></span>
<span data-ttu-id="ca535-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ca535-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca535-107">Permission type</span></span>|<span data-ttu-id="ca535-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca535-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca535-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca535-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ca535-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca535-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ca535-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca535-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca535-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca535-112">Not supported.</span></span>|
|<span data-ttu-id="ca535-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca535-113">Application</span></span>|<span data-ttu-id="ca535-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca535-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca535-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca535-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca535-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ca535-116">Optional query parameters</span></span>
<span data-ttu-id="ca535-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ca535-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ca535-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca535-118">Request headers</span></span>
|<span data-ttu-id="ca535-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ca535-119">Header</span></span>|<span data-ttu-id="ca535-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ca535-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca535-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca535-121">Authorization</span></span>|<span data-ttu-id="ca535-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ca535-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ca535-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ca535-123">Accept</span></span>|<span data-ttu-id="ca535-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ca535-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca535-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca535-125">Request body</span></span>
<span data-ttu-id="ca535-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ca535-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca535-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca535-127">Response</span></span>
<span data-ttu-id="ca535-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca535-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca535-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca535-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca535-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca535-130">Request</span></span>
<span data-ttu-id="ca535-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca535-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="ca535-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca535-132">Response</span></span>
<span data-ttu-id="ca535-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca535-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



