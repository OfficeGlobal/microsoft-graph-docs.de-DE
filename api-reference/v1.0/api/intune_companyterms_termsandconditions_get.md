# <a name="get-termsandconditions"></a><span data-ttu-id="cd36e-101">termsAndConditions abrufen</span><span class="sxs-lookup"><span data-stu-id="cd36e-101">Get termsAndConditions</span></span>

> <span data-ttu-id="cd36e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cd36e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd36e-103">Liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="cd36e-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd36e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cd36e-104">Prerequisites</span></span>
<span data-ttu-id="cd36e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd36e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd36e-107">Permission type</span></span>|<span data-ttu-id="cd36e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd36e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd36e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd36e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cd36e-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd36e-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cd36e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd36e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd36e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd36e-112">Not supported.</span></span>|
|<span data-ttu-id="cd36e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd36e-113">Application</span></span>|<span data-ttu-id="cd36e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd36e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd36e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd36e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd36e-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cd36e-116">Optional query parameters</span></span>
<span data-ttu-id="cd36e-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd36e-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cd36e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd36e-118">Request headers</span></span>
|<span data-ttu-id="cd36e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd36e-119">Header</span></span>|<span data-ttu-id="cd36e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cd36e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd36e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd36e-121">Authorization</span></span>|<span data-ttu-id="cd36e-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd36e-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cd36e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cd36e-123">Accept</span></span>|<span data-ttu-id="cd36e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cd36e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd36e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd36e-125">Request body</span></span>
<span data-ttu-id="cd36e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cd36e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd36e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd36e-127">Response</span></span>
<span data-ttu-id="cd36e-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd36e-128">If successful, this method returns a `200 OK` response code and a [section](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd36e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd36e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd36e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd36e-130">Request</span></span>
<span data-ttu-id="cd36e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd36e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="cd36e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd36e-132">Response</span></span>
<span data-ttu-id="cd36e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd36e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7
  }
}
```



