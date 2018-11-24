# <a name="get-contactfolder"></a><span data-ttu-id="52fdb-101">contactFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="52fdb-101">Get contactFolder</span></span>

<span data-ttu-id="52fdb-102">Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.</span><span class="sxs-lookup"><span data-stu-id="52fdb-102">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="52fdb-103">Es gibt zwei Szenarien, in dem eine app Kontaktordner eines anderen Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="52fdb-103">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="52fdb-104">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="52fdb-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="52fdb-105">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer diesen Benutzer einen Kontaktordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="52fdb-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="52fdb-106">Finden Sie [ausführliche Informationen und ein Beispiel](../../../concepts/outlook-get-shared-contacts-folders.md).</span><span class="sxs-lookup"><span data-stu-id="52fdb-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="52fdb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="52fdb-107">Permissions</span></span>
<span data-ttu-id="52fdb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="52fdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="52fdb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52fdb-110">Permission type</span></span>      | <span data-ttu-id="52fdb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52fdb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52fdb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52fdb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="52fdb-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52fdb-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="52fdb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52fdb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52fdb-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52fdb-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="52fdb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52fdb-116">Application</span></span> | <span data-ttu-id="52fdb-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52fdb-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="52fdb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52fdb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52fdb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="52fdb-119">Optional query parameters</span></span>
<span data-ttu-id="52fdb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="52fdb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52fdb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52fdb-121">Request headers</span></span>
| <span data-ttu-id="52fdb-122">Name</span><span class="sxs-lookup"><span data-stu-id="52fdb-122">Name</span></span>       | <span data-ttu-id="52fdb-123">Typ</span><span class="sxs-lookup"><span data-stu-id="52fdb-123">Type</span></span> | <span data-ttu-id="52fdb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52fdb-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52fdb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="52fdb-125">Authorization</span></span>  | <span data-ttu-id="52fdb-126">string</span><span class="sxs-lookup"><span data-stu-id="52fdb-126">string</span></span>  | <span data-ttu-id="52fdb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52fdb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52fdb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52fdb-129">Request body</span></span>
<span data-ttu-id="52fdb-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="52fdb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52fdb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="52fdb-131">Response</span></span>

<span data-ttu-id="52fdb-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52fdb-132">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52fdb-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52fdb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52fdb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52fdb-134">Request</span></span>
<span data-ttu-id="52fdb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52fdb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="52fdb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="52fdb-136">Response</span></span>
<span data-ttu-id="52fdb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52fdb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
