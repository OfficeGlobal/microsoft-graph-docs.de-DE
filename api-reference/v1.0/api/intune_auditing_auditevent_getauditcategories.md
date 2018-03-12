# <a name="getauditcategories-function"></a><span data-ttu-id="b0895-101">getAuditCategories-Funktion</span><span class="sxs-lookup"><span data-stu-id="b0895-101">getAuditCategories function</span></span>

> <span data-ttu-id="b0895-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b0895-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0895-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b0895-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0895-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b0895-104">Prerequisites</span></span>
<span data-ttu-id="b0895-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b0895-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0895-107">Permission type</span></span>|<span data-ttu-id="b0895-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0895-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0895-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0895-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b0895-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0895-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0895-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0895-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0895-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0895-112">Not supported.</span></span>|
|<span data-ttu-id="b0895-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0895-113">Application</span></span>|<span data-ttu-id="b0895-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0895-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0895-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0895-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="b0895-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0895-116">Request headers</span></span>
|<span data-ttu-id="b0895-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b0895-117">Header</span></span>|<span data-ttu-id="b0895-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b0895-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0895-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0895-119">Authorization</span></span>|<span data-ttu-id="b0895-120">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b0895-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b0895-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b0895-121">Accept</span></span>|<span data-ttu-id="b0895-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b0895-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0895-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0895-123">Request body</span></span>
<span data-ttu-id="b0895-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b0895-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0895-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0895-125">Response</span></span>
<span data-ttu-id="b0895-126">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolge-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0895-126">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0895-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0895-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0895-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0895-128">Request</span></span>
<span data-ttu-id="b0895-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0895-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="b0895-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0895-130">Response</span></span>
<span data-ttu-id="b0895-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0895-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```



