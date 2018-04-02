# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="111c4-101">mobileThreatDefenseConnector abrufen</span><span class="sxs-lookup"><span data-stu-id="111c4-101">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="111c4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="111c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="111c4-103">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="111c4-103">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="111c4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="111c4-104">Prerequisites</span></span>
<span data-ttu-id="111c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="111c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="111c4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="111c4-107">Permission type</span></span>|<span data-ttu-id="111c4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="111c4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="111c4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="111c4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="111c4-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="111c4-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="111c4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="111c4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="111c4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="111c4-112">Not supported.</span></span>|
|<span data-ttu-id="111c4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="111c4-113">Application</span></span>|<span data-ttu-id="111c4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="111c4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="111c4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="111c4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="111c4-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="111c4-116">Optional query parameters</span></span>
<span data-ttu-id="111c4-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="111c4-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="111c4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="111c4-118">Request headers</span></span>
|<span data-ttu-id="111c4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="111c4-119">Header</span></span>|<span data-ttu-id="111c4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="111c4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="111c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="111c4-121">Authorization</span></span>|<span data-ttu-id="111c4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="111c4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="111c4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="111c4-123">Accept</span></span>|<span data-ttu-id="111c4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="111c4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="111c4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="111c4-125">Request body</span></span>
<span data-ttu-id="111c4-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="111c4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="111c4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="111c4-127">Response</span></span>
<span data-ttu-id="111c4-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="111c4-128">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="111c4-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="111c4-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="111c4-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="111c4-130">Request</span></span>
<span data-ttu-id="111c4-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="111c4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="111c4-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="111c4-132">Response</span></span>
<span data-ttu-id="111c4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="111c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidEnabled": true,
    "iosEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6
  }
}
```



