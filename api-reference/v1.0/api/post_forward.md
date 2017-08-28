# <a name="post-forward"></a><span data-ttu-id="c341b-101">post: forward</span><span class="sxs-lookup"><span data-stu-id="c341b-101">post: forward</span></span>

<span data-ttu-id="c341b-p101">Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="c341b-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c341b-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c341b-104">Permissions</span></span>
<span data-ttu-id="c341b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c341b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c341b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c341b-107">Permission type</span></span>      | <span data-ttu-id="c341b-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c341b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c341b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c341b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c341b-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c341b-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c341b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c341b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c341b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c341b-112">Not supported.</span></span>    |
|<span data-ttu-id="c341b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c341b-113">Application</span></span> | <span data-ttu-id="c341b-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c341b-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c341b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c341b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="c341b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c341b-116">Request headers</span></span>
| <span data-ttu-id="c341b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c341b-117">Header</span></span>       | <span data-ttu-id="c341b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c341b-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c341b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c341b-119">Authorization</span></span>  | <span data-ttu-id="c341b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c341b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c341b-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c341b-122">Request body</span></span>
<span data-ttu-id="c341b-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c341b-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c341b-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="c341b-124">Parameter</span></span>    | <span data-ttu-id="c341b-125">Typ</span><span class="sxs-lookup"><span data-stu-id="c341b-125">Type</span></span>   |<span data-ttu-id="c341b-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c341b-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c341b-127">comment</span><span class="sxs-lookup"><span data-stu-id="c341b-127">comment</span></span>|<span data-ttu-id="c341b-128">String</span><span class="sxs-lookup"><span data-stu-id="c341b-128">String</span></span>|<span data-ttu-id="c341b-129">Optionaler Kommentar, der zusammen mit dem Beitrag weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="c341b-129">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="c341b-130">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c341b-130">toRecipients</span></span>|<span data-ttu-id="c341b-131">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="c341b-131">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="c341b-132">Die Empfänger, an die der Thread weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="c341b-132">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="c341b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c341b-133">Response</span></span>

<span data-ttu-id="c341b-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c341b-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c341b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c341b-136">Example</span></span>
<span data-ttu-id="c341b-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c341b-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c341b-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c341b-138">Request</span></span>
<span data-ttu-id="c341b-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c341b-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c341b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="c341b-140">Response</span></span>
<span data-ttu-id="c341b-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c341b-141">Here is an example of the response.</span></span>
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
