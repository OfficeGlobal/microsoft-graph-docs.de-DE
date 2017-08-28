# <a name="get-mailfolder"></a><span data-ttu-id="2844b-101">mailFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="2844b-101">Get mailFolder</span></span>

<span data-ttu-id="2844b-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs „mailfolder“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="2844b-102">Retrieve the properties and relationships of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2844b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2844b-103">Permissions</span></span>
<span data-ttu-id="2844b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2844b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2844b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2844b-106">Permission type</span></span>      | <span data-ttu-id="2844b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2844b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2844b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2844b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2844b-109">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2844b-109">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2844b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2844b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2844b-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2844b-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2844b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2844b-112">Application</span></span> | <span data-ttu-id="2844b-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2844b-113">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2844b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2844b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2844b-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2844b-115">Optional query parameters</span></span>
<span data-ttu-id="2844b-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2844b-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2844b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2844b-117">Request headers</span></span>
| <span data-ttu-id="2844b-118">Name</span><span class="sxs-lookup"><span data-stu-id="2844b-118">Name</span></span>       | <span data-ttu-id="2844b-119">Typ</span><span class="sxs-lookup"><span data-stu-id="2844b-119">Type</span></span> | <span data-ttu-id="2844b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2844b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2844b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2844b-121">Authorization</span></span>  | <span data-ttu-id="2844b-122">string</span><span class="sxs-lookup"><span data-stu-id="2844b-122">string</span></span>  | <span data-ttu-id="2844b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2844b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2844b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2844b-125">Request body</span></span>
<span data-ttu-id="2844b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2844b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2844b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2844b-127">Response</span></span>

<span data-ttu-id="2844b-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2844b-128">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2844b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2844b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2844b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2844b-130">Request</span></span>
<span data-ttu-id="2844b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2844b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="2844b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2844b-132">Response</span></span>
<span data-ttu-id="2844b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2844b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
