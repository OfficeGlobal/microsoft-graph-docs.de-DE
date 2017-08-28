# <a name="list-manager"></a><span data-ttu-id="27a0e-101">Manager auflisten</span><span class="sxs-lookup"><span data-stu-id="27a0e-101">List manager</span></span>

<span data-ttu-id="27a0e-p101">Ruft den Vorgesetzten des Benutzers ab. Gibt den Benutzer oder Kontakt zurück, der als Vorgesetzter des Benutzers zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="27a0e-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="27a0e-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="27a0e-104">Permissions</span></span>
<span data-ttu-id="27a0e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27a0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27a0e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="27a0e-107">Permission type</span></span>      | <span data-ttu-id="27a0e-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="27a0e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27a0e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="27a0e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="27a0e-110">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="27a0e-110">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27a0e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="27a0e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27a0e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27a0e-112">Not supported.</span></span>    |
|<span data-ttu-id="27a0e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="27a0e-113">Application</span></span> | <span data-ttu-id="27a0e-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a0e-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27a0e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="27a0e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27a0e-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="27a0e-116">Optional query parameters</span></span>
<span data-ttu-id="27a0e-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="27a0e-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="27a0e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="27a0e-118">Request headers</span></span>
| <span data-ttu-id="27a0e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="27a0e-119">Header</span></span>       | <span data-ttu-id="27a0e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="27a0e-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="27a0e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="27a0e-121">Authorization</span></span>  | <span data-ttu-id="27a0e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="27a0e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27a0e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27a0e-124">Content-Type</span></span>   | <span data-ttu-id="27a0e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27a0e-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27a0e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="27a0e-126">Request body</span></span>
<span data-ttu-id="27a0e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="27a0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27a0e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="27a0e-128">Response</span></span>

<span data-ttu-id="27a0e-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27a0e-129">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27a0e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27a0e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27a0e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="27a0e-131">Request</span></span>
<span data-ttu-id="27a0e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="27a0e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="27a0e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="27a0e-133">Response</span></span>
<span data-ttu-id="27a0e-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="27a0e-134">Here is an example of the response.</span></span>
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
