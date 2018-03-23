# <a name="list-termsandconditionses"></a><span data-ttu-id="92f83-101">Auflisten von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="92f83-101">List termsAndConditionses</span></span>

> <span data-ttu-id="92f83-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="92f83-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92f83-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) auf.</span><span class="sxs-lookup"><span data-stu-id="92f83-103">List properties and relationships of the [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92f83-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="92f83-104">Prerequisites</span></span>
<span data-ttu-id="92f83-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="92f83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="92f83-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92f83-107">Permission type</span></span>|<span data-ttu-id="92f83-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92f83-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92f83-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92f83-109">Delegated (work or school account)</span></span>|<span data-ttu-id="92f83-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="92f83-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="92f83-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92f83-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92f83-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92f83-112">Not supported.</span></span>|
|<span data-ttu-id="92f83-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92f83-113">Application</span></span>|<span data-ttu-id="92f83-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92f83-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92f83-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92f83-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="92f83-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92f83-116">Request headers</span></span>
|<span data-ttu-id="92f83-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="92f83-117">Header</span></span>|<span data-ttu-id="92f83-118">Wert</span><span class="sxs-lookup"><span data-stu-id="92f83-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92f83-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="92f83-119">Authorization</span></span>|<span data-ttu-id="92f83-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="92f83-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="92f83-121">Accept</span><span class="sxs-lookup"><span data-stu-id="92f83-121">Accept</span></span>|<span data-ttu-id="92f83-122">application/json</span><span class="sxs-lookup"><span data-stu-id="92f83-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92f83-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92f83-123">Request body</span></span>
<span data-ttu-id="92f83-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="92f83-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92f83-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="92f83-125">Response</span></span>
<span data-ttu-id="92f83-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="92f83-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_companyterms_termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92f83-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92f83-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="92f83-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92f83-128">Request</span></span>
<span data-ttu-id="92f83-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92f83-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="92f83-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="92f83-130">Response</span></span>
<span data-ttu-id="92f83-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92f83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
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
  ]
}
```



