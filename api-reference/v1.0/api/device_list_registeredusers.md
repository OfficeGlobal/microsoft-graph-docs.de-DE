# <a name="list-registeredusers"></a><span data-ttu-id="c9e2e-101">registeredUsers auflisten</span><span class="sxs-lookup"><span data-stu-id="c9e2e-101">List registeredUsers</span></span>

<span data-ttu-id="c9e2e-102">Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="c9e2e-102">Retrieve a list of users that are registered users of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9e2e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c9e2e-103">Permissions</span></span>
<span data-ttu-id="c9e2e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9e2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="c9e2e-106">Device.ReadWrite.All und User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="c9e2e-106">Device.ReadWrite.All and User.ReadBasic.All</span></span>
- <span data-ttu-id="c9e2e-107">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9e2e-107">Directory.Read.All</span></span>
- <span data-ttu-id="c9e2e-108">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e2e-108">Directory.ReadWrite.All</span></span> 
- <span data-ttu-id="c9e2e-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9e2e-109">Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c9e2e-110">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9e2e-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c9e2e-111">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c9e2e-111">Optional query parameters</span></span>
<span data-ttu-id="c9e2e-112">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c9e2e-112">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9e2e-113">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9e2e-113">Request headers</span></span>
| <span data-ttu-id="c9e2e-114">Name</span><span class="sxs-lookup"><span data-stu-id="c9e2e-114">Name</span></span>       | <span data-ttu-id="c9e2e-115">Typ</span><span class="sxs-lookup"><span data-stu-id="c9e2e-115">Type</span></span> | <span data-ttu-id="c9e2e-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9e2e-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c9e2e-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9e2e-117">Authorization</span></span>  | <span data-ttu-id="c9e2e-118">string</span><span class="sxs-lookup"><span data-stu-id="c9e2e-118">string</span></span>  | <span data-ttu-id="c9e2e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c9e2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9e2e-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9e2e-121">Request body</span></span>
<span data-ttu-id="c9e2e-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c9e2e-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9e2e-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9e2e-123">Response</span></span>

<span data-ttu-id="c9e2e-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9e2e-124">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9e2e-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9e2e-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9e2e-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9e2e-126">Request</span></span>
<span data-ttu-id="c9e2e-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9e2e-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="c9e2e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9e2e-128">Response</span></span>
<span data-ttu-id="c9e2e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9e2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->