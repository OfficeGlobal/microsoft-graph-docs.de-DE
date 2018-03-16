# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="cf7f7-101">Abrufen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="cf7f7-101">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="cf7f7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf7f7-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="cf7f7-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf7f7-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf7f7-104">Prerequisites</span></span>
<span data-ttu-id="cf7f7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf7f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf7f7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf7f7-107">Permission type</span></span>|<span data-ttu-id="cf7f7-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf7f7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf7f7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf7f7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cf7f7-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf7f7-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf7f7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf7f7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf7f7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf7f7-112">Not supported.</span></span>|
|<span data-ttu-id="cf7f7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf7f7-113">Application</span></span>|<span data-ttu-id="cf7f7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf7f7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf7f7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf7f7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf7f7-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf7f7-116">Optional query parameters</span></span>
<span data-ttu-id="cf7f7-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf7f7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf7f7-118">Request headers</span></span>
|<span data-ttu-id="cf7f7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cf7f7-119">Header</span></span>|<span data-ttu-id="cf7f7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cf7f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf7f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf7f7-121">Authorization</span></span>|<span data-ttu-id="cf7f7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf7f7-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cf7f7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cf7f7-123">Accept</span></span>|<span data-ttu-id="cf7f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf7f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf7f7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf7f7-125">Request body</span></span>
<span data-ttu-id="cf7f7-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf7f7-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf7f7-127">Response</span></span>
<span data-ttu-id="cf7f7-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf7f7-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf7f7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf7f7-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf7f7-130">Request</span></span>
<span data-ttu-id="cf7f7-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="cf7f7-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf7f7-132">Response</span></span>
<span data-ttu-id="cf7f7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



