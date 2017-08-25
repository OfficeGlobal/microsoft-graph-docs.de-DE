# <a name="create-conversation-thread"></a><span data-ttu-id="64fc7-101">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="64fc7-101">Create conversation thread</span></span>

<span data-ttu-id="64fc7-102">Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="64fc7-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="64fc7-p101">Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt. Verwenden Sie [Auf Thread antworten](conversationthread_reply.md) oder [Auf Beitrag antworten](post_reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="64fc7-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="64fc7-105">Hinweis: Sie können auch [einen neuen Thread in einer bestehenden Unterhaltung starten](conversation_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="64fc7-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="64fc7-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64fc7-106">Permissions</span></span>
<span data-ttu-id="64fc7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64fc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64fc7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64fc7-109">Permission type</span></span>      | <span data-ttu-id="64fc7-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64fc7-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="64fc7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64fc7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64fc7-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64fc7-112">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="64fc7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64fc7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64fc7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64fc7-114">Not supported.</span></span>    | 
|<span data-ttu-id="64fc7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64fc7-115">Application</span></span> | <span data-ttu-id="64fc7-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64fc7-116">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="64fc7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64fc7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="64fc7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64fc7-118">Request headers</span></span>
| <span data-ttu-id="64fc7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="64fc7-119">Header</span></span>       | <span data-ttu-id="64fc7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="64fc7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64fc7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64fc7-121">Authorization</span></span>  | <span data-ttu-id="64fc7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64fc7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64fc7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64fc7-124">Content-Type</span></span>  | <span data-ttu-id="64fc7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64fc7-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64fc7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64fc7-126">Request body</span></span>
<span data-ttu-id="64fc7-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an, das einen [Beitrag](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="64fc7-127">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="64fc7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="64fc7-128">Response</span></span>

<span data-ttu-id="64fc7-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64fc7-129">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64fc7-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64fc7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64fc7-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64fc7-131">Request</span></span>
<span data-ttu-id="64fc7-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64fc7-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="64fc7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="64fc7-133">Response</span></span>
<span data-ttu-id="64fc7-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64fc7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
