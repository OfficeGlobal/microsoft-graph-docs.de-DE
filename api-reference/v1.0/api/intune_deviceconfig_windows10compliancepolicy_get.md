# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="9b4fd-101">windows10CompliancePolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="9b4fd-101">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="9b4fd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b4fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b4fd-103">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9b4fd-103">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b4fd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b4fd-104">Prerequisites</span></span>
<span data-ttu-id="9b4fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b4fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9b4fd-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b4fd-107">Permission type</span></span>|<span data-ttu-id="9b4fd-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b4fd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b4fd-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b4fd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9b4fd-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b4fd-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b4fd-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b4fd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b4fd-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b4fd-112">Not supported.</span></span>|
|<span data-ttu-id="9b4fd-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b4fd-113">Application</span></span>|<span data-ttu-id="9b4fd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b4fd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b4fd-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b4fd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b4fd-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9b4fd-116">Optional query parameters</span></span>
<span data-ttu-id="9b4fd-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9b4fd-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9b4fd-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b4fd-118">Request headers</span></span>
|<span data-ttu-id="9b4fd-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9b4fd-119">Header</span></span>|<span data-ttu-id="9b4fd-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9b4fd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b4fd-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9b4fd-121">Authorization</span></span>|<span data-ttu-id="9b4fd-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b4fd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b4fd-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="9b4fd-123">Accept</span></span>|<span data-ttu-id="9b4fd-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="9b4fd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b4fd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b4fd-125">Request body</span></span>
<span data-ttu-id="9b4fd-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9b4fd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b4fd-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b4fd-127">Response</span></span>
<span data-ttu-id="9b4fd-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b4fd-128">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b4fd-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b4fd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b4fd-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b4fd-130">Request</span></span>
<span data-ttu-id="9b4fd-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b4fd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="9b4fd-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b4fd-132">Response</span></span>
<span data-ttu-id="9b4fd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b4fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1197

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
    "id": "2919ae62-ae62-2919-62ae-192962ae1929",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordRequiredToUnlockFromIdle": true,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "requireHealthyDeviceReport": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
    "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true
  }
}
```








