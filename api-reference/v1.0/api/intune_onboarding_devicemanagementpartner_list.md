# <a name="list-devicemanagementpartners"></a><span data-ttu-id="83eb9-101">deviceManagementPartners auflisten</span><span class="sxs-lookup"><span data-stu-id="83eb9-101">List deviceManagementPartners</span></span>

> <span data-ttu-id="83eb9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83eb9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83eb9-103">Auflisten von Eigenschaften und Beziehungen der [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="83eb9-103">List properties and relationships of the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83eb9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="83eb9-104">Prerequisites</span></span>
<span data-ttu-id="83eb9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="83eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83eb9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83eb9-107">Permission type</span></span>|<span data-ttu-id="83eb9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83eb9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83eb9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83eb9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="83eb9-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83eb9-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="83eb9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83eb9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83eb9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83eb9-112">Not supported.</span></span>|
|<span data-ttu-id="83eb9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83eb9-113">Application</span></span>|<span data-ttu-id="83eb9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83eb9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83eb9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83eb9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="83eb9-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83eb9-116">Request headers</span></span>
|<span data-ttu-id="83eb9-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="83eb9-117">Header</span></span>|<span data-ttu-id="83eb9-118">Wert</span><span class="sxs-lookup"><span data-stu-id="83eb9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83eb9-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="83eb9-119">Authorization</span></span>|<span data-ttu-id="83eb9-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="83eb9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83eb9-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="83eb9-121">Accept</span></span>|<span data-ttu-id="83eb9-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="83eb9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83eb9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83eb9-123">Request body</span></span>
<span data-ttu-id="83eb9-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="83eb9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83eb9-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="83eb9-125">Response</span></span>
<span data-ttu-id="83eb9-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="83eb9-126">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83eb9-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83eb9-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="83eb9-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83eb9-128">Request</span></span>
<span data-ttu-id="83eb9-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83eb9-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="83eb9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="83eb9-130">Response</span></span>
<span data-ttu-id="83eb9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83eb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```








