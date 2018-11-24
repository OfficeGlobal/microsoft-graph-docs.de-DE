# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="4933f-101">Auflisten von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="4933f-101">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="4933f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4933f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4933f-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="4933f-103">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4933f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4933f-104">Prerequisites</span></span>
<span data-ttu-id="4933f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4933f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4933f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4933f-107">Permission type</span></span>|<span data-ttu-id="4933f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4933f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4933f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4933f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4933f-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4933f-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4933f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4933f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4933f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4933f-112">Not supported.</span></span>|
|<span data-ttu-id="4933f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4933f-113">Application</span></span>|<span data-ttu-id="4933f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4933f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4933f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4933f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4933f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4933f-116">Request headers</span></span>
|<span data-ttu-id="4933f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4933f-117">Header</span></span>|<span data-ttu-id="4933f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4933f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4933f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4933f-119">Authorization</span></span>|<span data-ttu-id="4933f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4933f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4933f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4933f-121">Accept</span></span>|<span data-ttu-id="4933f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4933f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4933f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4933f-123">Request body</span></span>
<span data-ttu-id="4933f-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4933f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4933f-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="4933f-125">Response</span></span>
<span data-ttu-id="4933f-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4933f-126">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4933f-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4933f-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="4933f-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4933f-128">Request</span></span>
<span data-ttu-id="4933f-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4933f-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="4933f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="4933f-130">Response</span></span>
<span data-ttu-id="4933f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4933f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
      "id": "63a79499-9499-63a7-9994-a7639994a763",
      "installStatus": "available",
      "osVersion": "Os Version value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



