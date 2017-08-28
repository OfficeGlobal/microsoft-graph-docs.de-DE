# <a name="list-posts"></a><span data-ttu-id="9711f-101">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="9711f-101">List posts</span></span>

<span data-ttu-id="9711f-p101">Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="9711f-p101">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9711f-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9711f-104">Permissions</span></span>
<span data-ttu-id="9711f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9711f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9711f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9711f-107">Permission type</span></span>      | <span data-ttu-id="9711f-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9711f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9711f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9711f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9711f-110">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9711f-110">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="9711f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9711f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9711f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9711f-112">Not supported.</span></span>    |
|<span data-ttu-id="9711f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9711f-113">Application</span></span> | <span data-ttu-id="9711f-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9711f-114">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9711f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9711f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="9711f-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9711f-116">Optional query parameters</span></span>
<span data-ttu-id="9711f-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9711f-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9711f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9711f-118">Request headers</span></span>
| <span data-ttu-id="9711f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9711f-119">Header</span></span>       | <span data-ttu-id="9711f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9711f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9711f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9711f-121">Authorization</span></span>  | <span data-ttu-id="9711f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9711f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9711f-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9711f-124">Request body</span></span>
<span data-ttu-id="9711f-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9711f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9711f-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="9711f-126">Response</span></span>

<span data-ttu-id="9711f-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Post](../resources/post.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9711f-127">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9711f-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9711f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9711f-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9711f-129">Request</span></span>
<span data-ttu-id="9711f-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9711f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="9711f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9711f-131">Response</span></span>
<span data-ttu-id="9711f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9711f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
