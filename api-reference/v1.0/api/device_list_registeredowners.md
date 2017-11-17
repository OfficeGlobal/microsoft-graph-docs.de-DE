# <a name="list-registeredowners"></a><span data-ttu-id="f753d-101">registeredOwners auflisten</span><span class="sxs-lookup"><span data-stu-id="f753d-101">List registeredOwners</span></span>

<span data-ttu-id="f753d-102">Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="f753d-102">Retrieve a list of users that are registered owners of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="f753d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f753d-103">Permissions</span></span>
<span data-ttu-id="f753d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f753d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="f753d-106">Device.ReadWrite.All und User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f753d-106">Device.ReadWrite.All and User.ReadBasic.All</span></span>
- <span data-ttu-id="f753d-107">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f753d-107">Directory.Read.All</span></span>
- <span data-ttu-id="f753d-108">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f753d-108">Directory.ReadWrite.All</span></span> 
- <span data-ttu-id="f753d-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f753d-109">Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f753d-110">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f753d-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f753d-111">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f753d-111">Optional query parameters</span></span>
<span data-ttu-id="f753d-112">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f753d-112">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f753d-113">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f753d-113">Request headers</span></span>
| <span data-ttu-id="f753d-114">Name</span><span class="sxs-lookup"><span data-stu-id="f753d-114">Name</span></span>       | <span data-ttu-id="f753d-115">Typ</span><span class="sxs-lookup"><span data-stu-id="f753d-115">Type</span></span> | <span data-ttu-id="f753d-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f753d-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f753d-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="f753d-117">Authorization</span></span>  | <span data-ttu-id="f753d-118">string</span><span class="sxs-lookup"><span data-stu-id="f753d-118">string</span></span>  | <span data-ttu-id="f753d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f753d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f753d-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f753d-121">Request body</span></span>
<span data-ttu-id="f753d-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f753d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f753d-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="f753d-123">Response</span></span>

<span data-ttu-id="f753d-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f753d-124">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f753d-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f753d-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f753d-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f753d-126">Request</span></span>
<span data-ttu-id="f753d-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f753d-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="f753d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f753d-128">Response</span></span>
<span data-ttu-id="f753d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f753d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->