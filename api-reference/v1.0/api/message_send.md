# <a name="message-send"></a><span data-ttu-id="13cfa-101">message: send</span><span class="sxs-lookup"><span data-stu-id="13cfa-101">message: send</span></span>

<span data-ttu-id="13cfa-p101">Sendet eine Nachricht im Ordner „Entwürfe“. Der Entwurf kann ein Entwurf für eine neue Nachricht, eine Antwort, eine Antwort an alle oder eine Weiterleitung sein. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="13cfa-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13cfa-105">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="13cfa-105">Prerequisites</span></span>
<span data-ttu-id="13cfa-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="13cfa-106">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="13cfa-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13cfa-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="13cfa-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13cfa-108">Request headers</span></span>
| <span data-ttu-id="13cfa-109">Name</span><span class="sxs-lookup"><span data-stu-id="13cfa-109">Name</span></span>       | <span data-ttu-id="13cfa-110">Typ</span><span class="sxs-lookup"><span data-stu-id="13cfa-110">Type</span></span> | <span data-ttu-id="13cfa-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13cfa-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13cfa-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="13cfa-112">Authorization</span></span>  | <span data-ttu-id="13cfa-113">string</span><span class="sxs-lookup"><span data-stu-id="13cfa-113">string</span></span>  | <span data-ttu-id="13cfa-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13cfa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13cfa-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13cfa-116">Request body</span></span>

## <a name="response"></a><span data-ttu-id="13cfa-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="13cfa-117">Response</span></span>

<span data-ttu-id="13cfa-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13cfa-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13cfa-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13cfa-120">Example</span></span>
<span data-ttu-id="13cfa-121">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="13cfa-121">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="13cfa-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13cfa-122">Request</span></span>
<span data-ttu-id="13cfa-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13cfa-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="13cfa-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="13cfa-124">Response</span></span>
##### <a name="response"></a><span data-ttu-id="13cfa-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="13cfa-125">Response</span></span>
<span data-ttu-id="13cfa-126">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="13cfa-126">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
