# <a name="list-devicecompliancepolicystates"></a><span data-ttu-id="5d0a5-101">Auflisten von „deviceCompliancePolicyState“</span><span class="sxs-lookup"><span data-stu-id="5d0a5-101">List deviceCompliancePolicyStates</span></span>

> <span data-ttu-id="5d0a5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d0a5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d0a5-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5d0a5-103">List properties and relationships of the [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d0a5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d0a5-104">Prerequisites</span></span>
<span data-ttu-id="5d0a5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d0a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d0a5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d0a5-107">Permission type</span></span>|<span data-ttu-id="5d0a5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d0a5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d0a5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d0a5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5d0a5-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d0a5-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5d0a5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d0a5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d0a5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d0a5-112">Not supported.</span></span>|
|<span data-ttu-id="5d0a5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d0a5-113">Application</span></span>|<span data-ttu-id="5d0a5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d0a5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d0a5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d0a5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

## <a name="request-headers"></a><span data-ttu-id="5d0a5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d0a5-116">Request headers</span></span>
|<span data-ttu-id="5d0a5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d0a5-117">Header</span></span>|<span data-ttu-id="5d0a5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5d0a5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d0a5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d0a5-119">Authorization</span></span>|<span data-ttu-id="5d0a5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d0a5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d0a5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5d0a5-121">Accept</span></span>|<span data-ttu-id="5d0a5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5d0a5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d0a5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d0a5-123">Request body</span></span>
<span data-ttu-id="5d0a5-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5d0a5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d0a5-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d0a5-125">Response</span></span>
<span data-ttu-id="5d0a5-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5d0a5-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_deviceconfig_devicecompliancepolicystate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d0a5-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d0a5-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d0a5-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d0a5-128">Request</span></span>
<span data-ttu-id="5d0a5-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d0a5-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

### <a name="response"></a><span data-ttu-id="5d0a5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d0a5-130">Response</span></span>
<span data-ttu-id="5d0a5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d0a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1175

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
      "id": "2999e387-e387-2999-87e3-992987e39929",
      "settingStates": [
        {
          "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
          "setting": "Setting value",
          "settingName": "Setting Name value",
          "instanceDisplayName": "Instance Display Name value",
          "state": "notApplicable",
          "errorCode": 9,
          "errorDescription": "Error Description value",
          "userId": "User Id value",
          "userName": "User Name value",
          "userEmail": "User Email value",
          "userPrincipalName": "User Principal Name value",
          "sources": [
            {
              "@odata.type": "microsoft.graph.settingSource",
              "id": "Id value",
              "displayName": "Display Name value"
            }
          ],
          "currentValue": "Current Value value"
        }
      ],
      "displayName": "Display Name value",
      "version": 7,
      "platformType": "iOS",
      "state": "notApplicable",
      "settingCount": 12
    }
  ]
}
```



