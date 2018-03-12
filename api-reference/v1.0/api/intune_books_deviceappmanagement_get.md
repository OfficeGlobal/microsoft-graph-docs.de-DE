# <a name="get-deviceappmanagement"></a><span data-ttu-id="419b1-101">deviceAppManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="419b1-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="419b1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="419b1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="419b1-103">Lesen von Eigenschaften und Beziehungen des [deviceAppManagement](../resources/intune_books_deviceappmanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="419b1-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="419b1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="419b1-104">Prerequisites</span></span>
<span data-ttu-id="419b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="419b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="419b1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="419b1-107">Permission type</span></span>|<span data-ttu-id="419b1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="419b1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="419b1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="419b1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="419b1-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="419b1-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="419b1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="419b1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="419b1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="419b1-112">Not supported.</span></span>|
|<span data-ttu-id="419b1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="419b1-113">Application</span></span>|<span data-ttu-id="419b1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="419b1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="419b1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="419b1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="419b1-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="419b1-116">Optional query parameters</span></span>
<span data-ttu-id="419b1-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="419b1-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="419b1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="419b1-118">Request headers</span></span>
|<span data-ttu-id="419b1-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="419b1-119">Header</span></span>|<span data-ttu-id="419b1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="419b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="419b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="419b1-121">Authorization</span></span>|<span data-ttu-id="419b1-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="419b1-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="419b1-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="419b1-123">Accept</span></span>|<span data-ttu-id="419b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="419b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="419b1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="419b1-125">Request body</span></span>
<span data-ttu-id="419b1-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="419b1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="419b1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="419b1-127">Response</span></span>
<span data-ttu-id="419b1-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceAppManagement](../resources/intune_books_deviceappmanagement.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="419b1-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_books_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="419b1-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="419b1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="419b1-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="419b1-130">Request</span></span>
<span data-ttu-id="419b1-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="419b1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="419b1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="419b1-132">Response</span></span>
<span data-ttu-id="419b1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="419b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



