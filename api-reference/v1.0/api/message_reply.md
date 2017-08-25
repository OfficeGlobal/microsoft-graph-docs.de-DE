# <a name="message-reply"></a><span data-ttu-id="61f2c-101">message: reply</span><span class="sxs-lookup"><span data-stu-id="61f2c-101">message: reply</span></span>

<span data-ttu-id="61f2c-p101">Antwort auf eine Nachricht des Absenders. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="61f2c-p101">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="61f2c-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61f2c-104">Permissions</span></span>
<span data-ttu-id="61f2c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="61f2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61f2c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61f2c-107">Permission type</span></span>      | <span data-ttu-id="61f2c-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61f2c-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="61f2c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61f2c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="61f2c-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="61f2c-110">Mail.Send</span></span>    | 
|<span data-ttu-id="61f2c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61f2c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61f2c-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="61f2c-112">Mail.Send</span></span>    | 
|<span data-ttu-id="61f2c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61f2c-113">Application</span></span> | <span data-ttu-id="61f2c-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="61f2c-114">Mail.Send</span></span> | 

## <a name="http-request"></a><span data-ttu-id="61f2c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61f2c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="61f2c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61f2c-116">Request headers</span></span>
| <span data-ttu-id="61f2c-117">Name</span><span class="sxs-lookup"><span data-stu-id="61f2c-117">Name</span></span>       | <span data-ttu-id="61f2c-118">Typ</span><span class="sxs-lookup"><span data-stu-id="61f2c-118">Type</span></span> | <span data-ttu-id="61f2c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61f2c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="61f2c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="61f2c-120">Authorization</span></span>  | <span data-ttu-id="61f2c-121">string</span><span class="sxs-lookup"><span data-stu-id="61f2c-121">string</span></span>  | <span data-ttu-id="61f2c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61f2c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="61f2c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61f2c-124">Content-Type</span></span> | <span data-ttu-id="61f2c-125">string</span><span class="sxs-lookup"><span data-stu-id="61f2c-125">string</span></span>  | <span data-ttu-id="61f2c-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61f2c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61f2c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61f2c-128">Request body</span></span>
<span data-ttu-id="61f2c-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="61f2c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="61f2c-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="61f2c-130">Parameter</span></span>    | <span data-ttu-id="61f2c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="61f2c-131">Type</span></span>   |<span data-ttu-id="61f2c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61f2c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61f2c-133">comment</span><span class="sxs-lookup"><span data-stu-id="61f2c-133">comment</span></span>|<span data-ttu-id="61f2c-134">String</span><span class="sxs-lookup"><span data-stu-id="61f2c-134">String</span></span>|<span data-ttu-id="61f2c-p105">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="61f2c-p105">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="61f2c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="61f2c-137">Response</span></span>

<span data-ttu-id="61f2c-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61f2c-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61f2c-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61f2c-140">Example</span></span>
<span data-ttu-id="61f2c-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="61f2c-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="61f2c-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61f2c-142">Request</span></span>
<span data-ttu-id="61f2c-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61f2c-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="61f2c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="61f2c-144">Response</span></span>
##### <a name="response"></a><span data-ttu-id="61f2c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="61f2c-145">Response</span></span>
<span data-ttu-id="61f2c-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="61f2c-146">Here is an example of the response.</span></span>
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
