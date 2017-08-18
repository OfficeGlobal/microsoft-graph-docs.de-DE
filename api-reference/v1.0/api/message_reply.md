# <a name="message-reply"></a><span data-ttu-id="3ac63-101">message: reply</span><span class="sxs-lookup"><span data-stu-id="3ac63-101">message: reply</span></span>

<span data-ttu-id="3ac63-p101">Antwortet auf eine Nachricht des Absenders. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3ac63-p101">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ac63-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="3ac63-104">Prerequisites</span></span>
<span data-ttu-id="3ac63-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="3ac63-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="3ac63-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ac63-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="3ac63-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ac63-107">Request headers</span></span>
| <span data-ttu-id="3ac63-108">Name</span><span class="sxs-lookup"><span data-stu-id="3ac63-108">Name</span></span>       | <span data-ttu-id="3ac63-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3ac63-109">Type</span></span> | <span data-ttu-id="3ac63-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ac63-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ac63-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ac63-111">Authorization</span></span>  | <span data-ttu-id="3ac63-112">string</span><span class="sxs-lookup"><span data-stu-id="3ac63-112">string</span></span>  | <span data-ttu-id="3ac63-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ac63-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ac63-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ac63-115">Content-Type</span></span> | <span data-ttu-id="3ac63-116">string</span><span class="sxs-lookup"><span data-stu-id="3ac63-116">string</span></span>  | <span data-ttu-id="3ac63-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ac63-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ac63-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ac63-119">Request body</span></span>
<span data-ttu-id="3ac63-120">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3ac63-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ac63-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="3ac63-121">Parameter</span></span>    | <span data-ttu-id="3ac63-122">Typ</span><span class="sxs-lookup"><span data-stu-id="3ac63-122">Type</span></span>   |<span data-ttu-id="3ac63-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ac63-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ac63-124">comment</span><span class="sxs-lookup"><span data-stu-id="3ac63-124">comment</span></span>|<span data-ttu-id="3ac63-125">String</span><span class="sxs-lookup"><span data-stu-id="3ac63-125">String</span></span>|<span data-ttu-id="3ac63-p104">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="3ac63-p104">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="3ac63-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ac63-128">Response</span></span>

<span data-ttu-id="3ac63-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ac63-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ac63-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ac63-131">Example</span></span>
<span data-ttu-id="3ac63-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3ac63-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3ac63-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ac63-133">Request</span></span>
<span data-ttu-id="3ac63-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ac63-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="3ac63-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ac63-135">Response</span></span>
##### <a name="response"></a><span data-ttu-id="3ac63-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ac63-136">Response</span></span>
<span data-ttu-id="3ac63-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3ac63-137">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
