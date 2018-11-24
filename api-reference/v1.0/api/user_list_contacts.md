# <a name="list-contacts"></a><span data-ttu-id="a98f0-101">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="a98f0-101">List contacts</span></span>

<span data-ttu-id="a98f0-102">Rufen Sie eine Kontakte-Auflistung aus dem Standardordner Kontakte des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a98f0-102">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="a98f0-103">Es gibt zwei Szenarien, in dem eine app Kontakte in einen anderen Benutzer Kontaktordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="a98f0-103">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="a98f0-104">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="a98f0-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a98f0-105">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer diesen Benutzer einen Kontaktordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="a98f0-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a98f0-106">Finden Sie [ausführliche Informationen und ein Beispiel](../../../concepts/outlook-get-shared-contacts-folders.md).</span><span class="sxs-lookup"><span data-stu-id="a98f0-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="a98f0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a98f0-107">Permissions</span></span>
<span data-ttu-id="a98f0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a98f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a98f0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a98f0-110">Permission type</span></span>      | <span data-ttu-id="a98f0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a98f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a98f0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a98f0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a98f0-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a98f0-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a98f0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a98f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a98f0-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a98f0-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a98f0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a98f0-116">Application</span></span> | <span data-ttu-id="a98f0-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a98f0-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a98f0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a98f0-118">HTTP request</span></span>

<span data-ttu-id="a98f0-119">So rufen Sie alle Kontakte in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="a98f0-119">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="a98f0-120">So rufen Sie Kontakte in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="a98f0-120">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a98f0-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a98f0-121">Optional query parameters</span></span>
<span data-ttu-id="a98f0-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a98f0-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a98f0-123">Zum Beispiel können Sie die `$filter` Abfrageparameter verwenden, um Kontakte auf Basis der Domäne mit ihren E-Mail-Adressen filtern:</span><span class="sxs-lookup"><span data-stu-id="a98f0-123">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="a98f0-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a98f0-124">Request headers</span></span>
| <span data-ttu-id="a98f0-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a98f0-125">Header</span></span>       | <span data-ttu-id="a98f0-126">Wert</span><span class="sxs-lookup"><span data-stu-id="a98f0-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a98f0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a98f0-127">Authorization</span></span>  | <span data-ttu-id="a98f0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a98f0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a98f0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a98f0-130">Content-Type</span></span>   | <span data-ttu-id="a98f0-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a98f0-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a98f0-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a98f0-132">Request body</span></span>
<span data-ttu-id="a98f0-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a98f0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a98f0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a98f0-134">Response</span></span>

<span data-ttu-id="a98f0-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a98f0-135">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a98f0-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a98f0-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a98f0-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a98f0-137">Request</span></span>
<span data-ttu-id="a98f0-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a98f0-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="a98f0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a98f0-139">Response</span></span>
<span data-ttu-id="a98f0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a98f0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
