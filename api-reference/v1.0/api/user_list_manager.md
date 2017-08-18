# <a name="list-manager"></a><span data-ttu-id="2df81-101">Manager auflisten</span><span class="sxs-lookup"><span data-stu-id="2df81-101">List manager</span></span>

<span data-ttu-id="2df81-p101">Ruft den Vorgesetzten des Benutzers ab. Gibt den Benutzer oder Kontakt zurück, der als Vorgesetzter des Benutzers zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="2df81-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2df81-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2df81-104">Prerequisites</span></span>
<span data-ttu-id="2df81-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="2df81-105">One of the following **scopes** is required to execute this API: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="2df81-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2df81-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2df81-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2df81-107">Optional query parameters</span></span>
<span data-ttu-id="2df81-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2df81-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2df81-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2df81-109">Request headers</span></span>
| <span data-ttu-id="2df81-110">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2df81-110">Header</span></span>       | <span data-ttu-id="2df81-111">Wert</span><span class="sxs-lookup"><span data-stu-id="2df81-111">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="2df81-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df81-112">Authorization</span></span>  | <span data-ttu-id="2df81-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2df81-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2df81-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2df81-115">Content-Type</span></span>   | <span data-ttu-id="2df81-116">application/json</span><span class="sxs-lookup"><span data-stu-id="2df81-116">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="2df81-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2df81-117">Request body</span></span>
<span data-ttu-id="2df81-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2df81-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df81-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="2df81-119">Response</span></span>

<span data-ttu-id="2df81-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2df81-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2df81-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2df81-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2df81-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2df81-122">Request</span></span>
<span data-ttu-id="2df81-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2df81-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="2df81-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="2df81-124">Response</span></span>
<span data-ttu-id="2df81-125">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2df81-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
