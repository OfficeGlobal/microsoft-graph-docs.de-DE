# <a name="list-managedebookassignments"></a><span data-ttu-id="58e50-101">Auflisten von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="58e50-101">List managedEBookAssignments</span></span>

> <span data-ttu-id="58e50-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="58e50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58e50-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="58e50-103">List properties and relationships of the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58e50-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58e50-104">Prerequisites</span></span>
<span data-ttu-id="58e50-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58e50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58e50-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58e50-107">Permission type</span></span>|<span data-ttu-id="58e50-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58e50-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58e50-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58e50-109">Delegated (work or school account)</span></span>|<span data-ttu-id="58e50-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e50-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="58e50-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58e50-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58e50-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58e50-112">Not supported.</span></span>|
|<span data-ttu-id="58e50-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58e50-113">Application</span></span>|<span data-ttu-id="58e50-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58e50-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58e50-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58e50-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="58e50-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58e50-116">Request headers</span></span>
|<span data-ttu-id="58e50-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58e50-117">Header</span></span>|<span data-ttu-id="58e50-118">Wert</span><span class="sxs-lookup"><span data-stu-id="58e50-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58e50-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e50-119">Authorization</span></span>|<span data-ttu-id="58e50-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58e50-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="58e50-121">Accept</span><span class="sxs-lookup"><span data-stu-id="58e50-121">Accept</span></span>|<span data-ttu-id="58e50-122">application/json</span><span class="sxs-lookup"><span data-stu-id="58e50-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58e50-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58e50-123">Request body</span></span>
<span data-ttu-id="58e50-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="58e50-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58e50-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="58e50-125">Response</span></span>
<span data-ttu-id="58e50-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="58e50-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_books_managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e50-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58e50-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="58e50-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58e50-128">Request</span></span>
<span data-ttu-id="58e50-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58e50-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="58e50-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="58e50-130">Response</span></span>
<span data-ttu-id="58e50-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58e50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```



