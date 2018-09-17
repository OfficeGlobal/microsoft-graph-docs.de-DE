# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="e90fb-101">Auflisten von „deviceCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="e90fb-101">List deviceCompliancePolicies</span></span>

> <span data-ttu-id="e90fb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e90fb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e90fb-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e90fb-103">List properties and relationships of the [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e90fb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e90fb-104">Prerequisites</span></span>
<span data-ttu-id="e90fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e90fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e90fb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e90fb-107">Permission type</span></span>|<span data-ttu-id="e90fb-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e90fb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e90fb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e90fb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e90fb-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e90fb-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e90fb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e90fb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e90fb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e90fb-112">Not supported.</span></span>|
|<span data-ttu-id="e90fb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e90fb-113">Application</span></span>|<span data-ttu-id="e90fb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e90fb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e90fb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e90fb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e90fb-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e90fb-116">Request headers</span></span>
|<span data-ttu-id="e90fb-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e90fb-117">Header</span></span>|<span data-ttu-id="e90fb-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e90fb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e90fb-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e90fb-119">Authorization</span></span>|<span data-ttu-id="e90fb-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e90fb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e90fb-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e90fb-121">Accept</span></span>|<span data-ttu-id="e90fb-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="e90fb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e90fb-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e90fb-123">Request body</span></span>
<span data-ttu-id="e90fb-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e90fb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e90fb-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="e90fb-125">Response</span></span>
<span data-ttu-id="e90fb-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e90fb-126">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e90fb-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e90fb-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e90fb-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e90fb-128">Request</span></span>
<span data-ttu-id="e90fb-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e90fb-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="e90fb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e90fb-130">Response</span></span>
<span data-ttu-id="e90fb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e90fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```








