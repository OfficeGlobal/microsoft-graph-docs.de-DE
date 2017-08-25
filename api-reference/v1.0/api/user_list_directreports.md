# <a name="list-directreports"></a><span data-ttu-id="cb8aa-101">directReports auflisten</span><span class="sxs-lookup"><span data-stu-id="cb8aa-101">List directReports</span></span>

<span data-ttu-id="cb8aa-p101">Dient zum Abrufen des direkten Vorgesetzten des Benutzers. Zurückgegeben werden die Benutzer und Kontakte, denen der betreffende Benutzer als Manager zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="cb8aa-p101">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb8aa-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cb8aa-104">Permissions</span></span>
<span data-ttu-id="cb8aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb8aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb8aa-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb8aa-107">Permission type</span></span>      | <span data-ttu-id="cb8aa-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb8aa-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="cb8aa-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb8aa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="cb8aa-110">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb8aa-110">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="cb8aa-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb8aa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb8aa-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb8aa-112">User.Read, User.ReadWrite</span></span>    | 
|<span data-ttu-id="cb8aa-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb8aa-113">Application</span></span> | <span data-ttu-id="cb8aa-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8aa-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cb8aa-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb8aa-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb8aa-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cb8aa-116">Optional query parameters</span></span>
<span data-ttu-id="cb8aa-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cb8aa-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cb8aa-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb8aa-118">Request headers</span></span>
| <span data-ttu-id="cb8aa-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cb8aa-119">Header</span></span>       | <span data-ttu-id="cb8aa-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cb8aa-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="cb8aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb8aa-121">Authorization</span></span>  | <span data-ttu-id="cb8aa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb8aa-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb8aa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb8aa-124">Content-Type</span></span>   | <span data-ttu-id="cb8aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb8aa-125">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="cb8aa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb8aa-126">Request body</span></span>
<span data-ttu-id="cb8aa-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cb8aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb8aa-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb8aa-128">Response</span></span>

<span data-ttu-id="cb8aa-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb8aa-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb8aa-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb8aa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb8aa-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb8aa-131">Request</span></span>
<span data-ttu-id="cb8aa-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb8aa-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="cb8aa-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb8aa-133">Response</span></span>
<span data-ttu-id="cb8aa-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb8aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->