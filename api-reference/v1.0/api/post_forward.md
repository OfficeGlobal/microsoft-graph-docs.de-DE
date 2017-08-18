# <a name="post-forward"></a><span data-ttu-id="10d45-101">post: forward</span><span class="sxs-lookup"><span data-stu-id="10d45-101">post: forward</span></span>

<span data-ttu-id="10d45-p101">Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="10d45-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="10d45-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10d45-104">Prerequisites</span></span>
<span data-ttu-id="10d45-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="10d45-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="10d45-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="10d45-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="10d45-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10d45-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="10d45-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10d45-108">Request headers</span></span>
| <span data-ttu-id="10d45-109">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="10d45-109">Header</span></span>       | <span data-ttu-id="10d45-110">Wert</span><span class="sxs-lookup"><span data-stu-id="10d45-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10d45-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="10d45-111">Authorization</span></span>  | <span data-ttu-id="10d45-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10d45-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10d45-114">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10d45-114">Request body</span></span>
<span data-ttu-id="10d45-115">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="10d45-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="10d45-116">Parameter</span><span class="sxs-lookup"><span data-stu-id="10d45-116">Parameter</span></span>    | <span data-ttu-id="10d45-117">Typ</span><span class="sxs-lookup"><span data-stu-id="10d45-117">Type</span></span>   |<span data-ttu-id="10d45-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10d45-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10d45-119">comment</span><span class="sxs-lookup"><span data-stu-id="10d45-119">comment</span></span>|<span data-ttu-id="10d45-120">String</span><span class="sxs-lookup"><span data-stu-id="10d45-120">String</span></span>|<span data-ttu-id="10d45-121">Optionaler Kommentar, der zusammen mit dem Beitrag weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="10d45-121">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="10d45-122">toRecipients</span><span class="sxs-lookup"><span data-stu-id="10d45-122">toRecipients</span></span>|<span data-ttu-id="10d45-123">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="10d45-123">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="10d45-124">Die Empfänger, an die der Thread weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="10d45-124">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="10d45-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="10d45-125">Response</span></span>

<span data-ttu-id="10d45-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10d45-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10d45-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10d45-128">Example</span></span>
<span data-ttu-id="10d45-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="10d45-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="10d45-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10d45-130">Request</span></span>
<span data-ttu-id="10d45-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10d45-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="10d45-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="10d45-132">Response</span></span>
<span data-ttu-id="10d45-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="10d45-133">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
