# <a name="create-conversation"></a><span data-ttu-id="654d5-101">Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="654d5-101">Create Conversation</span></span>
<span data-ttu-id="654d5-102">Erstellen Sie eine neue [Unterhaltung](../resources/conversation.md), indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="654d5-102">Create a new conversation by including a thread and a post.</span></span> 

<span data-ttu-id="654d5-103">Sie können die APIs [conversationThread: reply](conversationthread_reply.md) und [post: reply](post_reply.md) verwenden, um weitere Beiträge in der betreffenden Unterhaltung zu veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="654d5-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="654d5-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="654d5-104">Permissions</span></span>
<span data-ttu-id="654d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="654d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="654d5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="654d5-107">Permission type</span></span>      | <span data-ttu-id="654d5-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="654d5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="654d5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="654d5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="654d5-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654d5-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="654d5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="654d5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="654d5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="654d5-112">Not supported.</span></span>    |
|<span data-ttu-id="654d5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="654d5-113">Application</span></span> | <span data-ttu-id="654d5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="654d5-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="654d5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="654d5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="654d5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="654d5-116">Request headers</span></span>
| <span data-ttu-id="654d5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="654d5-117">Header</span></span>       | <span data-ttu-id="654d5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="654d5-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="654d5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="654d5-119">Authorization</span></span>  | <span data-ttu-id="654d5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="654d5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="654d5-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="654d5-122">Content-Type</span></span>  | <span data-ttu-id="654d5-123">application/json</span><span class="sxs-lookup"><span data-stu-id="654d5-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="654d5-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="654d5-124">Request body</span></span>
<span data-ttu-id="654d5-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversation](../resources/conversation.md)-Objekts an, das einen [conversationThread](../resources/conversationThread.md) und einen [post](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="654d5-125">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="654d5-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="654d5-126">Response</span></span>
<span data-ttu-id="654d5-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="654d5-127">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="654d5-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="654d5-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="654d5-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="654d5-129">Request</span></span>
<span data-ttu-id="654d5-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="654d5-130">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations
Content-type: application/json

{
  "topic": "New Conversation Topic",
  "threads": [{
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
  }]
}
```

#### <a name="response"></a><span data-ttu-id="654d5-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="654d5-131">Response</span></span>
<span data-ttu-id="654d5-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="654d5-132">Here is an example of the response.</span></span>
><span data-ttu-id="654d5-133">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="654d5-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="654d5-134">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="654d5-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->