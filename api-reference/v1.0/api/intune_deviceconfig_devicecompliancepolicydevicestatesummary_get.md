# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="7a76f-101">deviceCompliancePolicyDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="7a76f-101">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="7a76f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a76f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a76f-103">Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a76f-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a76f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a76f-104">Prerequisites</span></span>
<span data-ttu-id="7a76f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a76f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7a76f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a76f-107">Permission type</span></span>|<span data-ttu-id="7a76f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a76f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a76f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a76f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7a76f-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a76f-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a76f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a76f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a76f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a76f-112">Not supported.</span></span>|
|<span data-ttu-id="7a76f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a76f-113">Application</span></span>|<span data-ttu-id="7a76f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a76f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a76f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a76f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a76f-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7a76f-116">Optional query parameters</span></span>
<span data-ttu-id="7a76f-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7a76f-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a76f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a76f-118">Request headers</span></span>
|<span data-ttu-id="7a76f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a76f-119">Header</span></span>|<span data-ttu-id="7a76f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7a76f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a76f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a76f-121">Authorization</span></span>|<span data-ttu-id="7a76f-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a76f-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a76f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7a76f-123">Accept</span></span>|<span data-ttu-id="7a76f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a76f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a76f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a76f-125">Request body</span></span>
<span data-ttu-id="7a76f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7a76f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a76f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a76f-127">Response</span></span>
<span data-ttu-id="7a76f-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a76f-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a76f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a76f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a76f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a76f-130">Request</span></span>
<span data-ttu-id="7a76f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a76f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="7a76f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a76f-132">Response</span></span>
<span data-ttu-id="7a76f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a76f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
    "inGracePeriodCount": 2,
    "configManagerCount": 2,
    "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```



