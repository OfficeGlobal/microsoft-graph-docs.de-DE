# <a name="get-mailfolder"></a><span data-ttu-id="0837d-101">mailFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="0837d-101">Get mailFolder</span></span>

<span data-ttu-id="0837d-102">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="0837d-102">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="0837d-103">Es gibt zwei Szenarien, in denen eine App den E-Mail-Ordner eines anderen Benutzers abrufen kann:</span><span class="sxs-lookup"><span data-stu-id="0837d-103">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="0837d-104">Wenn die App über Anwendungsberechtigungen verfügt, oder</span><span class="sxs-lookup"><span data-stu-id="0837d-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0837d-105">Wenn die App über die entsprechenden delegierten [Berechtigungen](#permissions) von einem Benutzer verfügt und ein anderer Benutzer einen E-Mail-Ordner für diesen Benutzer freigegeben hat oder delegierten Zugriff auf diesen Benutzer gewährt hat.</span><span class="sxs-lookup"><span data-stu-id="0837d-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0837d-106">Siehe [Details und ein Beispiel](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="0837d-106">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="0837d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0837d-107">Permissions</span></span>
<span data-ttu-id="0837d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0837d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0837d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0837d-110">Permission type</span></span>      | <span data-ttu-id="0837d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0837d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0837d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0837d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0837d-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0837d-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0837d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0837d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0837d-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0837d-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0837d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0837d-116">Application</span></span> | <span data-ttu-id="0837d-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0837d-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0837d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0837d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0837d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0837d-119">Optional query parameters</span></span>
<span data-ttu-id="0837d-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0837d-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0837d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0837d-121">Request headers</span></span>
| <span data-ttu-id="0837d-122">Name</span><span class="sxs-lookup"><span data-stu-id="0837d-122">Name</span></span>       | <span data-ttu-id="0837d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0837d-123">Type</span></span> | <span data-ttu-id="0837d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0837d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0837d-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0837d-125">Authorization</span></span>  | <span data-ttu-id="0837d-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0837d-126">string</span></span>  | <span data-ttu-id="0837d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0837d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0837d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0837d-129">Request body</span></span>
<span data-ttu-id="0837d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0837d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0837d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0837d-131">Response</span></span>

<span data-ttu-id="0837d-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0837d-132">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0837d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0837d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0837d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0837d-134">Request</span></span>
<span data-ttu-id="0837d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0837d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="0837d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0837d-136">Response</span></span>
<span data-ttu-id="0837d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0837d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
