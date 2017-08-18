# <a name="list-posts"></a><span data-ttu-id="6f6c0-101">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="6f6c0-101">List posts</span></span>

<span data-ttu-id="6f6c0-p101">Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="6f6c0-p101">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f6c0-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="6f6c0-104">Prerequisites</span></span>
<span data-ttu-id="6f6c0-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All; Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="6f6c0-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="6f6c0-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f6c0-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f6c0-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6f6c0-107">Optional query parameters</span></span>
<span data-ttu-id="6f6c0-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6f6c0-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6f6c0-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f6c0-109">Request headers</span></span>
| <span data-ttu-id="6f6c0-110">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f6c0-110">Header</span></span>       | <span data-ttu-id="6f6c0-111">Wert</span><span class="sxs-lookup"><span data-stu-id="6f6c0-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6f6c0-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f6c0-112">Authorization</span></span>  | <span data-ttu-id="6f6c0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f6c0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f6c0-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f6c0-115">Request body</span></span>
<span data-ttu-id="6f6c0-116">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6f6c0-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f6c0-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f6c0-117">Response</span></span>

<span data-ttu-id="6f6c0-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Post](../resources/post.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f6c0-118">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f6c0-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f6c0-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f6c0-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f6c0-120">Request</span></span>
<span data-ttu-id="6f6c0-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f6c0-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="6f6c0-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f6c0-122">Response</span></span>
<span data-ttu-id="6f6c0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f6c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
