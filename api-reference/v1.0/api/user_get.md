# <a name="get-a-user"></a><span data-ttu-id="5a0d7-101">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="5a0d7-101">Get a user</span></span>

<span data-ttu-id="5a0d7-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="5a0d7-p101">Hinweis: Durch das Auflisten eines Benutzers wird nur ein standardmäßiger Satz von Eigenschaften zurückgegeben (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Verwenden Sie `$select`, um die anderen Eigenschaften und Beziehungen für das [user](../resources/user.md)-Objekt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a0d7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5a0d7-105">Permissions</span></span>
<span data-ttu-id="5a0d7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a0d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a0d7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a0d7-108">Permission type</span></span>      | <span data-ttu-id="5a0d7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a0d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a0d7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a0d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a0d7-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a0d7-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a0d7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a0d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a0d7-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a0d7-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="5a0d7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a0d7-114">Application</span></span> | <span data-ttu-id="5a0d7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0d7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a0d7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a0d7-116">HTTP request</span></span>
<span data-ttu-id="5a0d7-117">Für einen bestimmten Benutzer:</span><span class="sxs-lookup"><span data-stu-id="5a0d7-117">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="5a0d7-118">Für den angemeldeten Benutzer:</span><span class="sxs-lookup"><span data-stu-id="5a0d7-118">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a0d7-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5a0d7-119">Optional query parameters</span></span>
<span data-ttu-id="5a0d7-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5a0d7-121">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="5a0d7-121">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="5a0d7-122">Um einen alternativen Eigenschaftensatz zurückzugeben, müssen Sie den gewünschten Satz von [user](../resources/user.md)-Eigenschaften mithilfe des Odata-Abfrageparameters `$select` angeben.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-122">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="5a0d7-123">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-123">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a0d7-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a0d7-124">Request headers</span></span>
| <span data-ttu-id="5a0d7-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5a0d7-125">Header</span></span>       | <span data-ttu-id="5a0d7-126">Wert</span><span class="sxs-lookup"><span data-stu-id="5a0d7-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="5a0d7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a0d7-127">Authorization</span></span>  | <span data-ttu-id="5a0d7-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a0d7-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a0d7-130">Content-Type</span></span>   | <span data-ttu-id="5a0d7-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5a0d7-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a0d7-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a0d7-132">Request body</span></span>
<span data-ttu-id="5a0d7-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a0d7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a0d7-134">Response</span></span>

<span data-ttu-id="5a0d7-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-135">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a0d7-136">Beispiele</span><span class="sxs-lookup"><span data-stu-id="5a0d7-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="5a0d7-137">Beispiel 1: Standard-Benutzeranforderung</span><span class="sxs-lookup"><span data-stu-id="5a0d7-137">Example 1: Standard users request</span></span>

<span data-ttu-id="5a0d7-138">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="5a0d7-138">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="5a0d7-139">Dieses Beispiel zeigt die standardmäßige Anforderung und Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-139">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="5a0d7-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a0d7-140">Response</span></span>

<!-- { "blockType": "ignored" } -->
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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="5a0d7-141">Beispiel 2: Anforderung des angemeldeten Benutzers</span><span class="sxs-lookup"><span data-stu-id="5a0d7-141">Example 2: Signed-in user request</span></span>

<span data-ttu-id="5a0d7-142">Sie können die Benutzerinformationen des angemeldeten Benutzers abrufen, indem Sie `/users/{id | userPrincipalName}` durch `/me` ersetzen.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-142">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="5a0d7-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a0d7-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="5a0d7-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a0d7-144">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="5a0d7-145">Beispiel 3: Benutzeranforderung mit $select</span><span class="sxs-lookup"><span data-stu-id="5a0d7-145">Example 2: Users request using $select</span></span>

<span data-ttu-id="5a0d7-146">Wenn Sie einen anderen Eigenschaftensatz benötigen, können Sie den OData-Abfrageparameter `$select` verwenden.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-146">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="5a0d7-147">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-147">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="5a0d7-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a0d7-148">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="5a0d7-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a0d7-149">Response</span></span>
<!-- { "blockType": "ignored" } -->
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
