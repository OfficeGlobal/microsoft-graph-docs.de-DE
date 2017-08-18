# <a name="create-thread"></a><span data-ttu-id="e6199-101">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="e6199-101">Create thread</span></span>

<span data-ttu-id="e6199-102">Dient zum Erstellen eines neuen Threads in der angegebenen Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="e6199-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="e6199-p101">Ein Thread und ein Beitrag werden wie angegeben erstellt. Verwenden Sie [Auf Thread antworten](conversationthread_reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen. Wenn Sie die Beitrags-ID abrufen, können Sie auch auf diesen Beitrag in diesem Thread [antworten](post_reply.md).</span><span class="sxs-lookup"><span data-stu-id="e6199-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="e6199-106">Hinweis: Sie können auch [eine neue Unterhaltung beginnen, indem Sie zuerst einen Thread erstellen](group_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="e6199-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6199-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e6199-107">Prerequisites</span></span>
<span data-ttu-id="e6199-108">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="e6199-108">The following **scopes** are required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="e6199-109">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6199-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="e6199-110">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6199-110">Request headers</span></span>
| <span data-ttu-id="e6199-111">Name</span><span class="sxs-lookup"><span data-stu-id="e6199-111">Name</span></span>       | <span data-ttu-id="e6199-112">Typ</span><span class="sxs-lookup"><span data-stu-id="e6199-112">Type</span></span> | <span data-ttu-id="e6199-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6199-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6199-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6199-114">Authorization</span></span>  | <span data-ttu-id="e6199-115">string</span><span class="sxs-lookup"><span data-stu-id="e6199-115">string</span></span>  | <span data-ttu-id="e6199-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6199-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6199-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6199-118">Request body</span></span>
<span data-ttu-id="e6199-119">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e6199-119">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e6199-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6199-120">Response</span></span>

<span data-ttu-id="e6199-121">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6199-121">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6199-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6199-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6199-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6199-123">Request</span></span>
<span data-ttu-id="e6199-124">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6199-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="e6199-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e6199-125">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e6199-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6199-126">Response</span></span>

<span data-ttu-id="e6199-p103">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das `id` im Antworttext zurückgegeben. Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6199-p103">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
