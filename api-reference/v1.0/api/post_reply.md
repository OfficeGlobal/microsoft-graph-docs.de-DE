# <a name="post-reply"></a><span data-ttu-id="34054-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="34054-101">post: reply</span></span>

<span data-ttu-id="34054-p101">Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="34054-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="34054-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34054-104">Permissions</span></span>
<span data-ttu-id="34054-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="34054-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="34054-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34054-107">Permission type</span></span>      | <span data-ttu-id="34054-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34054-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34054-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34054-109">Delegated (work or school account)</span></span> | <span data-ttu-id="34054-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34054-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="34054-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34054-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34054-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34054-112">Not supported.</span></span>    |
|<span data-ttu-id="34054-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34054-113">Application</span></span> | <span data-ttu-id="34054-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34054-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34054-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34054-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="34054-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34054-116">Request headers</span></span>
| <span data-ttu-id="34054-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="34054-117">Header</span></span>       | <span data-ttu-id="34054-118">Wert</span><span class="sxs-lookup"><span data-stu-id="34054-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34054-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="34054-119">Authorization</span></span>  | <span data-ttu-id="34054-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="34054-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34054-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34054-122">Request body</span></span>
<span data-ttu-id="34054-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="34054-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34054-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="34054-124">Parameter</span></span>    | <span data-ttu-id="34054-125">Typ</span><span class="sxs-lookup"><span data-stu-id="34054-125">Type</span></span>   |<span data-ttu-id="34054-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34054-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34054-127">Beitrag</span><span class="sxs-lookup"><span data-stu-id="34054-127">post</span></span>|[<span data-ttu-id="34054-128">post</span><span class="sxs-lookup"><span data-stu-id="34054-128">post</span></span>](../resources/post.md)|<span data-ttu-id="34054-129">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="34054-129">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="34054-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="34054-130">Response</span></span>

<span data-ttu-id="34054-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34054-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34054-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34054-133">Example</span></span>
<span data-ttu-id="34054-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="34054-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34054-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34054-135">Request</span></span>
<span data-ttu-id="34054-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34054-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="34054-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="34054-137">Response</span></span>
<span data-ttu-id="34054-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34054-138">Here is an example of the response.</span></span>
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
