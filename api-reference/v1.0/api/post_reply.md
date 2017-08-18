# <a name="post-reply"></a><span data-ttu-id="7cd58-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="7cd58-101">post: reply</span></span>

<span data-ttu-id="7cd58-p101">Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="7cd58-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cd58-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7cd58-104">Prerequisites</span></span>
<span data-ttu-id="7cd58-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="7cd58-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="7cd58-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="7cd58-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="7cd58-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cd58-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="7cd58-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7cd58-108">Request headers</span></span>
| <span data-ttu-id="7cd58-109">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7cd58-109">Header</span></span>       | <span data-ttu-id="7cd58-110">Wert</span><span class="sxs-lookup"><span data-stu-id="7cd58-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7cd58-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cd58-111">Authorization</span></span>  | <span data-ttu-id="7cd58-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7cd58-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7cd58-114">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7cd58-114">Request body</span></span>
<span data-ttu-id="7cd58-115">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7cd58-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7cd58-116">Parameter</span><span class="sxs-lookup"><span data-stu-id="7cd58-116">Parameter</span></span>    | <span data-ttu-id="7cd58-117">Typ</span><span class="sxs-lookup"><span data-stu-id="7cd58-117">Type</span></span>   |<span data-ttu-id="7cd58-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7cd58-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cd58-119">Beitrag</span><span class="sxs-lookup"><span data-stu-id="7cd58-119">post</span></span>|[<span data-ttu-id="7cd58-120">post</span><span class="sxs-lookup"><span data-stu-id="7cd58-120">post</span></span>](../resources/post.md)|<span data-ttu-id="7cd58-121">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="7cd58-121">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="7cd58-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cd58-122">Response</span></span>

<span data-ttu-id="7cd58-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cd58-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cd58-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7cd58-125">Example</span></span>
<span data-ttu-id="7cd58-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7cd58-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7cd58-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cd58-127">Request</span></span>
<span data-ttu-id="7cd58-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7cd58-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
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
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="7cd58-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cd58-129">Response</span></span>
##### <a name="response"></a><span data-ttu-id="7cd58-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cd58-130">Response</span></span>
<span data-ttu-id="7cd58-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7cd58-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
