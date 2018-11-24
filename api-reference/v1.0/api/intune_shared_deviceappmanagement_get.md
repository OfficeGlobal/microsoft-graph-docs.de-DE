# <a name="get-deviceappmanagement"></a><span data-ttu-id="21289-101">Abrufen von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="21289-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="21289-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21289-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21289-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="21289-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21289-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21289-104">Prerequisites</span></span>

<span data-ttu-id="21289-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="21289-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="21289-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="21289-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="21289-107">Beachten Sie, dass die entsprechende Berechtigungen gemäß den Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="21289-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="21289-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21289-108">Permission type</span></span>|<span data-ttu-id="21289-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21289-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21289-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21289-110">Delegated (work or school account)</span></span>|<span data-ttu-id="21289-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21289-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="21289-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21289-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21289-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21289-113">Not supported.</span></span>|
|<span data-ttu-id="21289-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21289-114">Application</span></span>|<span data-ttu-id="21289-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21289-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21289-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21289-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21289-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="21289-117">Optional query parameters</span></span>
<span data-ttu-id="21289-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="21289-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21289-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21289-119">Request headers</span></span>
|<span data-ttu-id="21289-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="21289-120">Header</span></span>|<span data-ttu-id="21289-121">Wert</span><span class="sxs-lookup"><span data-stu-id="21289-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21289-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21289-122">Authorization</span></span>|<span data-ttu-id="21289-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21289-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21289-124">Accept</span><span class="sxs-lookup"><span data-stu-id="21289-124">Accept</span></span>|<span data-ttu-id="21289-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21289-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21289-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21289-126">Request body</span></span>
<span data-ttu-id="21289-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="21289-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21289-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="21289-128">Response</span></span>
<span data-ttu-id="21289-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21289-129">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="21289-130">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="21289-130">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="21289-131">Beispielantwort</span><span class="sxs-lookup"><span data-stu-id="21289-131">Example response</span></span>
<span data-ttu-id="21289-132">Der Kürze halber werden möglicherweise im Response-Objekt dargestellten abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="21289-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="21289-133">Alle Eigenschaften werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21289-133">All properties will be returned from an actual call.</span></span>

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



