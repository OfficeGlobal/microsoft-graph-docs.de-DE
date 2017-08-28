# <a name="conversationthread-reply"></a><span data-ttu-id="47f66-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="47f66-101">conversationThread: reply</span></span>

<span data-ttu-id="47f66-p101">Dient zum Antworten auf einen Thread in einer Gruppenunterhaltung und zum Hinzufügen eines neuen Beitrags. Sie können die übergeordnete Unterhaltung in der Anforderung angeben, oder Sie können nur den Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="47f66-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="47f66-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="47f66-104">Permissions</span></span>
<span data-ttu-id="47f66-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47f66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47f66-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47f66-107">Permission type</span></span>      | <span data-ttu-id="47f66-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47f66-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47f66-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47f66-109">Delegated (work or school account)</span></span> | <span data-ttu-id="47f66-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f66-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47f66-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47f66-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47f66-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47f66-112">Not supported.</span></span>    |
|<span data-ttu-id="47f66-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47f66-113">Application</span></span> | <span data-ttu-id="47f66-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f66-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47f66-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47f66-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="47f66-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47f66-116">Request headers</span></span>
| <span data-ttu-id="47f66-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47f66-117">Header</span></span>       | <span data-ttu-id="47f66-118">Wert</span><span class="sxs-lookup"><span data-stu-id="47f66-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47f66-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="47f66-119">Authorization</span></span>  | <span data-ttu-id="47f66-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="47f66-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="47f66-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47f66-122">Content-Type</span></span>  | <span data-ttu-id="47f66-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="47f66-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47f66-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47f66-125">Request body</span></span>
<span data-ttu-id="47f66-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="47f66-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47f66-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="47f66-127">Parameter</span></span>    | <span data-ttu-id="47f66-128">Typ</span><span class="sxs-lookup"><span data-stu-id="47f66-128">Type</span></span>   |<span data-ttu-id="47f66-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47f66-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47f66-130">Beitrag</span><span class="sxs-lookup"><span data-stu-id="47f66-130">post</span></span>|[<span data-ttu-id="47f66-131">post</span><span class="sxs-lookup"><span data-stu-id="47f66-131">post</span></span>](../resources/post.md)|<span data-ttu-id="47f66-132">Der neue Beitrag, mit dem geantwortet wird.</span><span class="sxs-lookup"><span data-stu-id="47f66-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="47f66-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="47f66-133">Response</span></span>

<span data-ttu-id="47f66-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47f66-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f66-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47f66-136">Example</span></span>
<span data-ttu-id="47f66-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="47f66-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47f66-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47f66-138">Request</span></span>
<span data-ttu-id="47f66-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47f66-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="47f66-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="47f66-140">Response</span></span>
<span data-ttu-id="47f66-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="47f66-141">Here is an example of the response.</span></span>
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
