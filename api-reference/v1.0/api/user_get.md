# <a name="get-a-user"></a><span data-ttu-id="e421f-101">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="e421f-101">Get a user</span></span>

<span data-ttu-id="e421f-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.</span><span class="sxs-lookup"><span data-stu-id="e421f-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="e421f-p101">Hinweis: Durch das Auflisten eines Benutzers wird nur ein standardmäßiger Satz von Eigenschaften zurückgegeben (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Verwenden Sie `$select`, um die anderen Eigenschaften und Beziehungen für das [user](../resources/user.md)-Objekt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="e421f-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e421f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e421f-105">Permissions</span></span>
<span data-ttu-id="e421f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e421f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e421f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e421f-108">Permission type</span></span>      | <span data-ttu-id="e421f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e421f-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e421f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e421f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e421f-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e421f-111">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="e421f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e421f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e421f-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e421f-113">User.Read, User.ReadWrite</span></span>    | 
|<span data-ttu-id="e421f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e421f-114">Application</span></span> | <span data-ttu-id="e421f-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e421f-115">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e421f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e421f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e421f-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e421f-117">Optional query parameters</span></span>
<span data-ttu-id="e421f-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e421f-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e421f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e421f-119">Request headers</span></span>
| <span data-ttu-id="e421f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e421f-120">Header</span></span>       | <span data-ttu-id="e421f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e421f-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e421f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e421f-122">Authorization</span></span>  | <span data-ttu-id="e421f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e421f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e421f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e421f-125">Content-Type</span></span>   | <span data-ttu-id="e421f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e421f-126">application/json</span></span> | 

## <a name="request-body"></a><span data-ttu-id="e421f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e421f-127">Request body</span></span>
<span data-ttu-id="e421f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e421f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e421f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e421f-129">Response</span></span>

<span data-ttu-id="e421f-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e421f-130">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e421f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e421f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e421f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e421f-132">Request</span></span>
<span data-ttu-id="e421f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e421f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="e421f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e421f-134">Response</span></span>
<span data-ttu-id="e421f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e421f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
