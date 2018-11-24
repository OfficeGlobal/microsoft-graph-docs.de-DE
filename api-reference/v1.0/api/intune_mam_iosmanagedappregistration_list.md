# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="994c4-101">Auflisten von „iosManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="994c4-101">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="994c4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="994c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="994c4-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="994c4-103">List properties and relationships of the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="994c4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="994c4-104">Prerequisites</span></span>
<span data-ttu-id="994c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="994c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="994c4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="994c4-107">Permission type</span></span>|<span data-ttu-id="994c4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="994c4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="994c4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="994c4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="994c4-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="994c4-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="994c4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="994c4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="994c4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="994c4-112">Not supported.</span></span>|
|<span data-ttu-id="994c4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="994c4-113">Application</span></span>|<span data-ttu-id="994c4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="994c4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="994c4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="994c4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="994c4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="994c4-116">Request headers</span></span>
|<span data-ttu-id="994c4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="994c4-117">Header</span></span>|<span data-ttu-id="994c4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="994c4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="994c4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="994c4-119">Authorization</span></span>|<span data-ttu-id="994c4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="994c4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="994c4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="994c4-121">Accept</span></span>|<span data-ttu-id="994c4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="994c4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="994c4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="994c4-123">Request body</span></span>
<span data-ttu-id="994c4-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="994c4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="994c4-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="994c4-125">Response</span></span>
<span data-ttu-id="994c4-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="994c4-126">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="994c4-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="994c4-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="994c4-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="994c4-128">Request</span></span>
<span data-ttu-id="994c4-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="994c4-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="994c4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="994c4-130">Response</span></span>
<span data-ttu-id="994c4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="994c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
        "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
        "bundleId": "Bundle Id value"
      },
      "id": "47632c19-2c19-4763-192c-6347192c6347",
      "version": "Version value"
    }
  ]
}
```



