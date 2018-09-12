# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="2a764-101">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="2a764-101">Get deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="2a764-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2a764-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a764-103">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a764-103">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a764-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a764-104">Prerequisites</span></span>
<span data-ttu-id="2a764-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a764-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a764-107">Permission type</span></span>|<span data-ttu-id="2a764-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a764-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a764-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a764-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a764-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a764-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2a764-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a764-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a764-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a764-112">Not supported.</span></span>|
|<span data-ttu-id="2a764-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a764-113">Application</span></span>|<span data-ttu-id="2a764-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a764-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a764-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a764-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a764-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2a764-116">Optional query parameters</span></span>
<span data-ttu-id="2a764-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2a764-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2a764-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a764-118">Request headers</span></span>
|<span data-ttu-id="2a764-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a764-119">Header</span></span>|<span data-ttu-id="2a764-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2a764-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a764-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2a764-121">Authorization</span></span>|<span data-ttu-id="2a764-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a764-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a764-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2a764-123">Accept</span></span>|<span data-ttu-id="2a764-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="2a764-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a764-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a764-125">Request body</span></span>
<span data-ttu-id="2a764-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2a764-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a764-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a764-127">Response</span></span>
<span data-ttu-id="2a764-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a764-128">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a764-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a764-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a764-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a764-130">Request</span></span>
<span data-ttu-id="2a764-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a764-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="2a764-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a764-132">Response</span></span>
<span data-ttu-id="2a764-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a764-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 368

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
    "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
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








