# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="9df6a-101">iosUpdateConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="9df6a-101">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="9df6a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9df6a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9df6a-103">Lesen von Eigenschaften und Beziehungen des [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9df6a-103">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9df6a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9df6a-104">Prerequisites</span></span>
<span data-ttu-id="9df6a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9df6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9df6a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9df6a-107">Permission type</span></span>|<span data-ttu-id="9df6a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9df6a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9df6a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9df6a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9df6a-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9df6a-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9df6a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9df6a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9df6a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9df6a-112">Not supported.</span></span>|
|<span data-ttu-id="9df6a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9df6a-113">Application</span></span>|<span data-ttu-id="9df6a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9df6a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9df6a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9df6a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9df6a-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9df6a-116">Optional query parameters</span></span>
<span data-ttu-id="9df6a-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9df6a-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9df6a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9df6a-118">Request headers</span></span>
|<span data-ttu-id="9df6a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9df6a-119">Header</span></span>|<span data-ttu-id="9df6a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9df6a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9df6a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9df6a-121">Authorization</span></span>|<span data-ttu-id="9df6a-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9df6a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9df6a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9df6a-123">Accept</span></span>|<span data-ttu-id="9df6a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9df6a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9df6a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9df6a-125">Request body</span></span>
<span data-ttu-id="9df6a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9df6a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9df6a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9df6a-127">Response</span></span>
<span data-ttu-id="9df6a-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9df6a-128">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9df6a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9df6a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9df6a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9df6a-130">Request</span></span>
<span data-ttu-id="9df6a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9df6a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9df6a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9df6a-132">Response</span></span>
<span data-ttu-id="9df6a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9df6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6
  }
}
```



