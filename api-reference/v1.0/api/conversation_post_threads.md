# <a name="create-thread"></a><span data-ttu-id="00b6b-101">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="00b6b-101">Create thread</span></span>

<span data-ttu-id="00b6b-102">Dient zum Erstellen eines neuen Threads in der angegebenen Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="00b6b-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="00b6b-p101">Ein Thread und ein Beitrag werden wie angegeben erstellt. Verwenden Sie [Auf Thread antworten](conversationthread_reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen. Wenn Sie die Beitrags-ID abrufen, können Sie auch auf diesen Beitrag in diesem Thread [antworten](post_reply.md).</span><span class="sxs-lookup"><span data-stu-id="00b6b-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="00b6b-106">Hinweis: Sie können auch [eine neue Unterhaltung beginnen, indem Sie zuerst einen Thread erstellen](group_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="00b6b-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="00b6b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="00b6b-107">Permissions</span></span>
<span data-ttu-id="00b6b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00b6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00b6b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00b6b-110">Permission type</span></span>      | <span data-ttu-id="00b6b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00b6b-111">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="00b6b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00b6b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00b6b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00b6b-113">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="00b6b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00b6b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00b6b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00b6b-115">Not supported.</span></span>    | 
|<span data-ttu-id="00b6b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00b6b-116">Application</span></span> | <span data-ttu-id="00b6b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00b6b-117">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="00b6b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00b6b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="00b6b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00b6b-119">Request headers</span></span>
| <span data-ttu-id="00b6b-120">Name</span><span class="sxs-lookup"><span data-stu-id="00b6b-120">Name</span></span>       | <span data-ttu-id="00b6b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="00b6b-121">Type</span></span> | <span data-ttu-id="00b6b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00b6b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="00b6b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00b6b-123">Authorization</span></span>  | <span data-ttu-id="00b6b-124">string</span><span class="sxs-lookup"><span data-stu-id="00b6b-124">string</span></span>  | <span data-ttu-id="00b6b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="00b6b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00b6b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00b6b-127">Request body</span></span>
<span data-ttu-id="00b6b-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="00b6b-128">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00b6b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="00b6b-129">Response</span></span>

<span data-ttu-id="00b6b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00b6b-130">If successful, this method returns `201, Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00b6b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00b6b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00b6b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00b6b-132">Request</span></span>
<span data-ttu-id="00b6b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00b6b-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="00b6b-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="00b6b-134">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="00b6b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="00b6b-135">Response</span></span>

<span data-ttu-id="00b6b-p104">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das `id` im Antworttext zurückgegeben. Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="00b6b-p104">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
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
