# <a name="create-conversation"></a><span data-ttu-id="f4fb1-101">Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="f4fb1-101">Create conversation</span></span>
<span data-ttu-id="f4fb1-102">Erstellen Sie eine neue [Unterhaltung](../resources/conversation.md), indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-102">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="f4fb1-103">Sie können die APIs [conversationThread: reply](conversationthread_reply.md) und [post: reply](post_reply.md) verwenden, um weitere Beiträge in der betreffenden Unterhaltung zu veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4fb1-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f4fb1-104">Permissions</span></span>
<span data-ttu-id="f4fb1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4fb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f4fb1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4fb1-107">Permission type</span></span>      | <span data-ttu-id="f4fb1-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4fb1-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4fb1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4fb1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f4fb1-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4fb1-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4fb1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4fb1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4fb1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4fb1-112">Not supported.</span></span>    |
|<span data-ttu-id="f4fb1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4fb1-113">Application</span></span> | <span data-ttu-id="f4fb1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4fb1-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4fb1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4fb1-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="f4fb1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4fb1-116">Request headers</span></span>
| <span data-ttu-id="f4fb1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f4fb1-117">Header</span></span>       | <span data-ttu-id="f4fb1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f4fb1-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f4fb1-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f4fb1-119">Authorization</span></span>  | <span data-ttu-id="f4fb1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f4fb1-122">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="f4fb1-122">Content-Type</span></span>  | <span data-ttu-id="f4fb1-123">application/json</span><span class="sxs-lookup"><span data-stu-id="f4fb1-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f4fb1-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4fb1-124">Request body</span></span>
<span data-ttu-id="f4fb1-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversation](../resources/conversation.md)-Objekts an, das einen [conversationThread](../resources/conversationThread.md) und einen [post](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-125">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="f4fb1-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4fb1-126">Response</span></span>
<span data-ttu-id="f4fb1-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-127">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="f4fb1-128">Die Antwort enthält die IDs für die neue Unterhaltung und den Thread, die Sie im Vorgang [Beiträge auflisten](conversationthread_list_posts.md) auch verwenden können, um zu dem neuen Beitrag zu gelangen.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-128">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread_list_posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="f4fb1-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4fb1-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f4fb1-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4fb1-130">Request</span></span>
<span data-ttu-id="f4fb1-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["29981b6a-0e57-42dc-94c9-cd24f5306196"],
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
    "topic":"New locations for this quarter",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"What do we know so far?"
                    },
                    "newParticipants":[
                        {
                            "emailAddress":{
                                "name":"Adele Vance",
                                "address":"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="f4fb1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4fb1-132">Response</span></span>
<span data-ttu-id="f4fb1-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-133">The following is an example of the response.</span></span>
><span data-ttu-id="f4fb1-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f4fb1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADDVKtMlRp4Txc6k=",
    "threads@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADDVKtMlRp4Txc6k%3D')/threads",
    "threads":[
        {
            "id":"AAQkADQDarUNUq0yVGnhPFzqQ=="
        }
    ]
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