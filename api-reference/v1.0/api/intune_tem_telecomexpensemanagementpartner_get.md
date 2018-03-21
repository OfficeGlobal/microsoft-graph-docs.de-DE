# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="d98a0-101">telecomExpenseManagementPartner abrufen</span><span class="sxs-lookup"><span data-stu-id="d98a0-101">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="d98a0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d98a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d98a0-103">Lesen von Eigenschaften und Beziehungen des [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d98a0-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d98a0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d98a0-104">Prerequisites</span></span>
<span data-ttu-id="d98a0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d98a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d98a0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d98a0-107">Permission type</span></span>|<span data-ttu-id="d98a0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d98a0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d98a0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d98a0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d98a0-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d98a0-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d98a0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d98a0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d98a0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d98a0-112">Not supported.</span></span>|
|<span data-ttu-id="d98a0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d98a0-113">Application</span></span>|<span data-ttu-id="d98a0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d98a0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d98a0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d98a0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d98a0-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d98a0-116">Optional query parameters</span></span>
<span data-ttu-id="d98a0-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d98a0-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d98a0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d98a0-118">Request headers</span></span>
|<span data-ttu-id="d98a0-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d98a0-119">Header</span></span>|<span data-ttu-id="d98a0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d98a0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d98a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d98a0-121">Authorization</span></span>|<span data-ttu-id="d98a0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d98a0-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d98a0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d98a0-123">Accept</span></span>|<span data-ttu-id="d98a0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d98a0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d98a0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d98a0-125">Request body</span></span>
<span data-ttu-id="d98a0-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d98a0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d98a0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d98a0-127">Response</span></span>
<span data-ttu-id="d98a0-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d98a0-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d98a0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d98a0-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d98a0-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d98a0-130">Request</span></span>
<span data-ttu-id="d98a0-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d98a0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="d98a0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d98a0-132">Response</span></span>
<span data-ttu-id="d98a0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d98a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



