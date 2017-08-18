# <a name="conversationthread-reply"></a><span data-ttu-id="2f02b-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="2f02b-101">conversationThread: reply</span></span>

<span data-ttu-id="2f02b-p101">Dient zum Antworten auf einen Thread in einer Gruppenunterhaltung und zum Hinzufügen eines neuen Beitrags. Sie können die übergeordnete Unterhaltung in der Anforderung angeben, oder Sie können nur den Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="2f02b-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f02b-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2f02b-104">Prerequisites</span></span>
<span data-ttu-id="2f02b-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="2f02b-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="2f02b-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f02b-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="2f02b-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f02b-107">Request headers</span></span>
| <span data-ttu-id="2f02b-108">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f02b-108">Header</span></span>       | <span data-ttu-id="2f02b-109">Wert</span><span class="sxs-lookup"><span data-stu-id="2f02b-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f02b-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f02b-110">Authorization</span></span>  | <span data-ttu-id="2f02b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f02b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f02b-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f02b-113">Content-Type</span></span>  | <span data-ttu-id="2f02b-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2f02b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f02b-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f02b-116">Request body</span></span>
<span data-ttu-id="2f02b-117">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2f02b-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f02b-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="2f02b-118">Parameter</span></span>    | <span data-ttu-id="2f02b-119">Typ</span><span class="sxs-lookup"><span data-stu-id="2f02b-119">Type</span></span>   |<span data-ttu-id="2f02b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f02b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f02b-121">Beitrag</span><span class="sxs-lookup"><span data-stu-id="2f02b-121">post</span></span>|[<span data-ttu-id="2f02b-122">post</span><span class="sxs-lookup"><span data-stu-id="2f02b-122">post</span></span>](../resources/post.md)|<span data-ttu-id="2f02b-123">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="2f02b-123">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="2f02b-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f02b-124">Response</span></span>

<span data-ttu-id="2f02b-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f02b-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f02b-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f02b-127">Example</span></span>
<span data-ttu-id="2f02b-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2f02b-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f02b-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f02b-129">Request</span></span>
<span data-ttu-id="2f02b-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f02b-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="2f02b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f02b-131">Response</span></span>
<span data-ttu-id="2f02b-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f02b-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
