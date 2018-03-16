# <a name="get-managedebookassignment"></a><span data-ttu-id="f88bb-101">Abrufen von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="f88bb-101">Get managedEBookAssignment</span></span>

> <span data-ttu-id="f88bb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f88bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f88bb-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f88bb-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f88bb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f88bb-104">Prerequisites</span></span>
<span data-ttu-id="f88bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f88bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f88bb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f88bb-107">Permission type</span></span>|<span data-ttu-id="f88bb-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f88bb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f88bb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f88bb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f88bb-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f88bb-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f88bb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f88bb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f88bb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f88bb-112">Not supported.</span></span>|
|<span data-ttu-id="f88bb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f88bb-113">Application</span></span>|<span data-ttu-id="f88bb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f88bb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f88bb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f88bb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f88bb-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f88bb-116">Optional query parameters</span></span>
<span data-ttu-id="f88bb-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f88bb-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f88bb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f88bb-118">Request headers</span></span>
|<span data-ttu-id="f88bb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f88bb-119">Header</span></span>|<span data-ttu-id="f88bb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f88bb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f88bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f88bb-121">Authorization</span></span>|<span data-ttu-id="f88bb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f88bb-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f88bb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f88bb-123">Accept</span></span>|<span data-ttu-id="f88bb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f88bb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f88bb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f88bb-125">Request body</span></span>
<span data-ttu-id="f88bb-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f88bb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f88bb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f88bb-127">Response</span></span>
<span data-ttu-id="f88bb-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f88bb-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f88bb-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f88bb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f88bb-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f88bb-130">Request</span></span>
<span data-ttu-id="f88bb-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f88bb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f88bb-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f88bb-132">Response</span></span>
<span data-ttu-id="f88bb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f88bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookAssignment",
    "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```



