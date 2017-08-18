# <a name="create-conversation-thread"></a><span data-ttu-id="55338-101">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="55338-101">Create conversation thread</span></span>

<span data-ttu-id="55338-102">Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="55338-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="55338-p101">Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt. Verwenden Sie [Auf Thread antworten](conversationthread_reply.md) oder [Auf Beitrag antworten](post_reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="55338-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="55338-105">Hinweis: Sie können auch [eine neuen Threads in einer bestehenden Unterhaltung beginnen](conversation_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="55338-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="55338-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="55338-106">Prerequisites</span></span>
<span data-ttu-id="55338-107">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="55338-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="55338-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55338-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="55338-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55338-109">Request headers</span></span>
| <span data-ttu-id="55338-110">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="55338-110">Header</span></span>       | <span data-ttu-id="55338-111">Wert</span><span class="sxs-lookup"><span data-stu-id="55338-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55338-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="55338-112">Authorization</span></span>  | <span data-ttu-id="55338-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55338-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="55338-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55338-115">Content-Type</span></span>  | <span data-ttu-id="55338-116">application/json</span><span class="sxs-lookup"><span data-stu-id="55338-116">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55338-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55338-117">Request body</span></span>
<span data-ttu-id="55338-118">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an, das einen [Beitrag](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="55338-118">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="55338-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="55338-119">Response</span></span>

<span data-ttu-id="55338-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55338-120">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55338-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55338-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55338-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55338-122">Request</span></span>
<span data-ttu-id="55338-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55338-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```
##### <a name="response"></a><span data-ttu-id="55338-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="55338-124">Response</span></span>
<span data-ttu-id="55338-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55338-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
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
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
