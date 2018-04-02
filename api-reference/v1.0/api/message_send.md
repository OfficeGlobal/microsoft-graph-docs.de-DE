# <a name="message-send"></a><span data-ttu-id="660bd-101">message: send</span><span class="sxs-lookup"><span data-stu-id="660bd-101">message: send</span></span>

<span data-ttu-id="660bd-p101">Sendet eine Nachricht im Ordner „Entwürfe“. Der Entwurf kann ein Entwurf für eine neue Nachricht, eine Antwort, eine Antwort an alle oder eine Weiterleitung sein. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="660bd-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="660bd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="660bd-105">Permissions</span></span>
<span data-ttu-id="660bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="660bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="660bd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="660bd-108">Permission type</span></span>      | <span data-ttu-id="660bd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="660bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="660bd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="660bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="660bd-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="660bd-111">Mail.Send</span></span>    |
|<span data-ttu-id="660bd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="660bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="660bd-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="660bd-113">Mail.Send</span></span>    |
|<span data-ttu-id="660bd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="660bd-114">Application</span></span> | <span data-ttu-id="660bd-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="660bd-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="660bd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="660bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="660bd-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="660bd-117">Request headers</span></span>
| <span data-ttu-id="660bd-118">Name</span><span class="sxs-lookup"><span data-stu-id="660bd-118">Name</span></span>       | <span data-ttu-id="660bd-119">Typ</span><span class="sxs-lookup"><span data-stu-id="660bd-119">Type</span></span> | <span data-ttu-id="660bd-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="660bd-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="660bd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="660bd-121">Authorization</span></span>  | <span data-ttu-id="660bd-122">string</span><span class="sxs-lookup"><span data-stu-id="660bd-122">string</span></span>  | <span data-ttu-id="660bd-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="660bd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="660bd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="660bd-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="660bd-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="660bd-126">Response</span></span>

<span data-ttu-id="660bd-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="660bd-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="660bd-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="660bd-129">Example</span></span>
<span data-ttu-id="660bd-130">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="660bd-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="660bd-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="660bd-131">Request</span></span>
<span data-ttu-id="660bd-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="660bd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="660bd-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="660bd-133">Response</span></span>

<span data-ttu-id="660bd-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="660bd-134">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
