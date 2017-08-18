# <a name="get-conversationthread"></a><span data-ttu-id="68613-101">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="68613-101">Get conversationThread</span></span>

<span data-ttu-id="68613-p101">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="68613-p101">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="68613-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="68613-104">Prerequisites</span></span>
<span data-ttu-id="68613-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All; Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="68613-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="68613-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68613-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="68613-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="68613-107">Optional query parameters</span></span>
<span data-ttu-id="68613-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68613-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="68613-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68613-109">Request headers</span></span>
| <span data-ttu-id="68613-110">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="68613-110">Header</span></span>       | <span data-ttu-id="68613-111">Wert</span><span class="sxs-lookup"><span data-stu-id="68613-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68613-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="68613-112">Authorization</span></span>  | <span data-ttu-id="68613-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68613-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68613-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68613-115">Request body</span></span>
<span data-ttu-id="68613-116">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="68613-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68613-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="68613-117">Response</span></span>

<span data-ttu-id="68613-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68613-118">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68613-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68613-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68613-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68613-120">Request</span></span>
<span data-ttu-id="68613-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68613-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="68613-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="68613-122">Response</span></span>
<span data-ttu-id="68613-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68613-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
