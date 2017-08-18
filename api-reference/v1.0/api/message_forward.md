# <a name="message-forward"></a><span data-ttu-id="2d253-101">message: forward</span><span class="sxs-lookup"><span data-stu-id="2d253-101">message: forward</span></span>

<span data-ttu-id="2d253-p101">Leitet eine Nachricht weiter. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="2d253-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d253-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2d253-104">Prerequisites</span></span>
<span data-ttu-id="2d253-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="2d253-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="2d253-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d253-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="2d253-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d253-107">Request headers</span></span>
| <span data-ttu-id="2d253-108">Name</span><span class="sxs-lookup"><span data-stu-id="2d253-108">Name</span></span>       | <span data-ttu-id="2d253-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2d253-109">Type</span></span> | <span data-ttu-id="2d253-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d253-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d253-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d253-111">Authorization</span></span>  | <span data-ttu-id="2d253-112">string</span><span class="sxs-lookup"><span data-stu-id="2d253-112">string</span></span>  | <span data-ttu-id="2d253-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d253-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d253-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d253-115">Content-Type</span></span> | <span data-ttu-id="2d253-116">string</span><span class="sxs-lookup"><span data-stu-id="2d253-116">string</span></span>  | <span data-ttu-id="2d253-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d253-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d253-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d253-119">Request body</span></span>
<span data-ttu-id="2d253-120">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2d253-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d253-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="2d253-121">Parameter</span></span>    | <span data-ttu-id="2d253-122">Typ</span><span class="sxs-lookup"><span data-stu-id="2d253-122">Type</span></span>   |<span data-ttu-id="2d253-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d253-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d253-124">comment</span><span class="sxs-lookup"><span data-stu-id="2d253-124">comment</span></span>|<span data-ttu-id="2d253-125">String</span><span class="sxs-lookup"><span data-stu-id="2d253-125">String</span></span>|<span data-ttu-id="2d253-p104">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="2d253-p104">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="2d253-128">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2d253-128">toRecipients</span></span>|<span data-ttu-id="2d253-129">[Recipient collection](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="2d253-129">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="2d253-130">Die Liste der Empfänger.</span><span class="sxs-lookup"><span data-stu-id="2d253-130">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="2d253-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d253-131">Response</span></span>

<span data-ttu-id="2d253-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d253-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d253-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d253-134">Example</span></span>
<span data-ttu-id="2d253-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2d253-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d253-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d253-136">Request</span></span>
<span data-ttu-id="2d253-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d253-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="2d253-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d253-138">Response</span></span>
##### <a name="response"></a><span data-ttu-id="2d253-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d253-139">Response</span></span>
<span data-ttu-id="2d253-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d253-140">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
