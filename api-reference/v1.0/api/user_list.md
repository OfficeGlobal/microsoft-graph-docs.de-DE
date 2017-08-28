# <a name="list-users"></a><span data-ttu-id="35a48-101">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="35a48-101">List users</span></span>

<span data-ttu-id="35a48-102">Mit dieser API können Sie eine Liste von Benutzerobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="35a48-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="35a48-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="35a48-103">Permissions</span></span>

<span data-ttu-id="35a48-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="35a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="35a48-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35a48-106">Permission type</span></span>      | <span data-ttu-id="35a48-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35a48-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35a48-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35a48-108">Delegated (work or school account)</span></span> | <span data-ttu-id="35a48-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35a48-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="35a48-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35a48-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35a48-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35a48-111">Not supported.</span></span>    |
|<span data-ttu-id="35a48-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35a48-112">Application</span></span> | <span data-ttu-id="35a48-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35a48-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35a48-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35a48-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35a48-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="35a48-115">Optional query parameters</span></span>

<span data-ttu-id="35a48-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="35a48-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="35a48-117">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="35a48-117">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="35a48-p102">Um einen alternativen Eigenschaftensatz zurückzugeben, müssen Sie den gewünschten Satz von [user](../resources/user.md)-Eigenschaften mithilfe des ODATA-Abfrageparameters `$select` angeben. Um zum Beispiel _displayName_, _givenName_, _id_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="35a48-p102">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return _displayName_, _givenName_, _id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="35a48-p103">Hinweis: Bestimmte Eigenschaften können innerhalb einer Benutzersammlung nicht zurückgegeben werden. Die folgenden Eigenschaften werden nur unterstützt, wenn [ein einzelner Benutzer abgerufen wird](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="35a48-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="35a48-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35a48-122">Request headers</span></span>

| <span data-ttu-id="35a48-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="35a48-123">Header</span></span>        | <span data-ttu-id="35a48-124">Wert</span><span class="sxs-lookup"><span data-stu-id="35a48-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="35a48-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="35a48-125">Authorization</span></span> | <span data-ttu-id="35a48-126">Bearer {token} (erforderlich)</span><span class="sxs-lookup"><span data-stu-id="35a48-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="35a48-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35a48-127">Content-Type</span></span>  | <span data-ttu-id="35a48-128">application/json</span><span class="sxs-lookup"><span data-stu-id="35a48-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="35a48-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35a48-129">Request body</span></span>

<span data-ttu-id="35a48-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35a48-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35a48-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="35a48-131">Response</span></span>

<span data-ttu-id="35a48-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35a48-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35a48-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35a48-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="35a48-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35a48-134">Request</span></span>

<span data-ttu-id="35a48-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35a48-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="35a48-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="35a48-136">Response</span></span>

<span data-ttu-id="35a48-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35a48-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
