# <a name="list-users"></a><span data-ttu-id="12a3a-101">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="12a3a-101">List users</span></span>

<span data-ttu-id="12a3a-102">Mit dieser API können Sie eine Liste von Benutzerobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="12a3a-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="12a3a-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12a3a-103">Permissions</span></span>

<span data-ttu-id="12a3a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12a3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12a3a-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12a3a-106">Permission type</span></span>      | <span data-ttu-id="12a3a-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12a3a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12a3a-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12a3a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="12a3a-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12a3a-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12a3a-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12a3a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a3a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12a3a-111">Not supported.</span></span>    |
|<span data-ttu-id="12a3a-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12a3a-112">Application</span></span> | <span data-ttu-id="12a3a-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12a3a-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12a3a-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12a3a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12a3a-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="12a3a-115">Optional query parameters</span></span>

<span data-ttu-id="12a3a-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="12a3a-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="12a3a-117">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="12a3a-117">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="12a3a-118">Um einen alternativen Eigenschaftensatz zurückzugeben, müssen Sie den gewünschten Satz von [user](../resources/user.md)-Eigenschaften mithilfe des Odata-Abfrageparameters `$select` angeben.</span><span class="sxs-lookup"><span data-stu-id="12a3a-118">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="12a3a-119">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="12a3a-119">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="12a3a-p103">Hinweis: Bestimmte Eigenschaften können innerhalb einer Benutzersammlung nicht zurückgegeben werden. Die folgenden Eigenschaften werden nur unterstützt, wenn [ein einzelner Benutzer abgerufen wird](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="12a3a-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="12a3a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12a3a-122">Request headers</span></span>

| <span data-ttu-id="12a3a-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="12a3a-123">Header</span></span>        | <span data-ttu-id="12a3a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="12a3a-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="12a3a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="12a3a-125">Authorization</span></span> | <span data-ttu-id="12a3a-126">Bearer {token} (erforderlich)</span><span class="sxs-lookup"><span data-stu-id="12a3a-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="12a3a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12a3a-127">Content-Type</span></span>  | <span data-ttu-id="12a3a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="12a3a-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="12a3a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12a3a-129">Request body</span></span>

<span data-ttu-id="12a3a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="12a3a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a3a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="12a3a-131">Response</span></span>

<span data-ttu-id="12a3a-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12a3a-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12a3a-133">Beispiele</span><span class="sxs-lookup"><span data-stu-id="12a3a-133">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="12a3a-134">Beispiel 1: Standard-Benutzeranforderung</span><span class="sxs-lookup"><span data-stu-id="12a3a-134">Example 1: Standard users request</span></span>

<span data-ttu-id="12a3a-135">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="12a3a-135">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="12a3a-136">Dieses Beispiel zeigt die standardmäßige Anforderung und Antwort.</span><span class="sxs-lookup"><span data-stu-id="12a3a-136">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="12a3a-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12a3a-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="12a3a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="12a3a-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
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
  ]
}
```

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="12a3a-139">Beispiel 2: Benutzeranforderung mit $select</span><span class="sxs-lookup"><span data-stu-id="12a3a-139">Example 2: Users request using $select</span></span>

<span data-ttu-id="12a3a-140">Wenn Sie einen anderen Eigenschaftensatz benötigen, können Sie den OData-Abfrageparameter `$select` verwenden.</span><span class="sxs-lookup"><span data-stu-id="12a3a-140">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="12a3a-141">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="12a3a-141">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="12a3a-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12a3a-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="12a3a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="12a3a-143">Response</span></span>

<span data-ttu-id="12a3a-144">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="12a3a-144">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
