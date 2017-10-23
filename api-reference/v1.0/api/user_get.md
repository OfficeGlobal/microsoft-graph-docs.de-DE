# <a name="get-a-user"></a><span data-ttu-id="bd02a-101">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="bd02a-101">Get a user</span></span>

<span data-ttu-id="bd02a-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.</span><span class="sxs-lookup"><span data-stu-id="bd02a-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="bd02a-p101">Hinweis: Durch das Auflisten eines Benutzers wird nur ein standardmäßiger Satz von Eigenschaften zurückgegeben (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Verwenden Sie `$select`, um die anderen Eigenschaften und Beziehungen für das [user](../resources/user.md)-Objekt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="bd02a-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd02a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd02a-105">Permissions</span></span>
<span data-ttu-id="bd02a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd02a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd02a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd02a-108">Permission type</span></span>      | <span data-ttu-id="bd02a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd02a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd02a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd02a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd02a-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd02a-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd02a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd02a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd02a-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd02a-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="bd02a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd02a-114">Application</span></span> | <span data-ttu-id="bd02a-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd02a-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd02a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd02a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd02a-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bd02a-117">Optional query parameters</span></span>
<span data-ttu-id="bd02a-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bd02a-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="bd02a-119">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="bd02a-119">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="bd02a-120">Um einen alternativen Eigenschaftensatz zurückzugeben, müssen Sie den gewünschten Satz von [user](../resources/user.md)-Eigenschaften mithilfe des Odata-Abfrageparameters `$select` angeben.</span><span class="sxs-lookup"><span data-stu-id="bd02a-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return displayName, givenName, id and postalCode, you would use the add the following to your query </span></span> <span data-ttu-id="bd02a-121">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="bd02a-121">To return an alternative property set, you must specify the desired set of user properties using the ODATA  query parameter. For example, to return _displayName_, _givenName, id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd02a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd02a-122">Request headers</span></span>
| <span data-ttu-id="bd02a-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bd02a-123">Header</span></span>       | <span data-ttu-id="bd02a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="bd02a-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="bd02a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd02a-125">Authorization</span></span>  | <span data-ttu-id="bd02a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bd02a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd02a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd02a-128">Content-Type</span></span>   | <span data-ttu-id="bd02a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bd02a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd02a-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd02a-130">Request body</span></span>
<span data-ttu-id="bd02a-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bd02a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd02a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd02a-132">Response</span></span>

<span data-ttu-id="bd02a-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd02a-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd02a-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bd02a-134">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="bd02a-135">Beispiel 1: Standard-Benutzeranforderung</span><span class="sxs-lookup"><span data-stu-id="bd02a-135">Example 1: Standard users request</span></span>

<span data-ttu-id="bd02a-136">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="bd02a-136">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="bd02a-137">Dieses Beispiel zeigt die standardmäßige Anforderung und Antwort.</span><span class="sxs-lookup"><span data-stu-id="bd02a-137">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="bd02a-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd02a-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="bd02a-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd02a-139">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="bd02a-140">Beispiel 2: Benutzeranforderung mit $select</span><span class="sxs-lookup"><span data-stu-id="bd02a-140">Example 2: Users request using $select</span></span>

<span data-ttu-id="bd02a-141">Wenn Sie einen anderen Eigenschaftensatz benötigen, können Sie den OData-Abfrageparameter `$select` verwenden.</span><span class="sxs-lookup"><span data-stu-id="bd02a-141">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="bd02a-142">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="bd02a-142">To return an alternative property set, you must specify the desired set of user properties using the ODATA  query parameter. For example, to return _displayName_, _givenName, id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="bd02a-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd02a-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="bd02a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd02a-144">Response</span></span>
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
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
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
