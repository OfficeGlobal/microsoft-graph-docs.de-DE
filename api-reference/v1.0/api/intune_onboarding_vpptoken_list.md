# <a name="list-vpptokens"></a><span data-ttu-id="8068f-101">vppTokens auflisten</span><span class="sxs-lookup"><span data-stu-id="8068f-101">List vppTokens</span></span>

> <span data-ttu-id="8068f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8068f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8068f-103">Auflisten von Eigenschaften und Beziehungen der [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8068f-103">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_vpptoken.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8068f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8068f-104">Prerequisites</span></span>
<span data-ttu-id="8068f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8068f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8068f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8068f-107">Permission type</span></span>|<span data-ttu-id="8068f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8068f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8068f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8068f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8068f-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8068f-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8068f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8068f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8068f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8068f-112">Not supported.</span></span>|
|<span data-ttu-id="8068f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8068f-113">Application</span></span>|<span data-ttu-id="8068f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8068f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8068f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8068f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="8068f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8068f-116">Request headers</span></span>
|<span data-ttu-id="8068f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8068f-117">Header</span></span>|<span data-ttu-id="8068f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8068f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8068f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8068f-119">Authorization</span></span>|<span data-ttu-id="8068f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8068f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8068f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8068f-121">Accept</span></span>|<span data-ttu-id="8068f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8068f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8068f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8068f-123">Request body</span></span>
<span data-ttu-id="8068f-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8068f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8068f-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8068f-125">Response</span></span>
<span data-ttu-id="8068f-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8068f-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_onboarding_vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8068f-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8068f-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8068f-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8068f-128">Request</span></span>
<span data-ttu-id="8068f-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8068f-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="8068f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8068f-130">Response</span></span>
<span data-ttu-id="8068f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8068f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "education",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "valid",
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value"
    }
  ]
}
```



