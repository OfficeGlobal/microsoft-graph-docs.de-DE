# <a name="message-copy"></a><span data-ttu-id="dbd40-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="dbd40-101">message: copy</span></span>

<span data-ttu-id="dbd40-102">Mit dieser API können Sie Nachrichten in Ordner kopieren.</span><span class="sxs-lookup"><span data-stu-id="dbd40-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbd40-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dbd40-103">Permissions</span></span>
<span data-ttu-id="dbd40-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dbd40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dbd40-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dbd40-106">Permission type</span></span>      | <span data-ttu-id="dbd40-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dbd40-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbd40-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dbd40-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dbd40-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbd40-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dbd40-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dbd40-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbd40-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbd40-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dbd40-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dbd40-112">Application</span></span> | <span data-ttu-id="dbd40-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbd40-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbd40-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dbd40-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="dbd40-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dbd40-115">Request headers</span></span>
| <span data-ttu-id="dbd40-116">Name</span><span class="sxs-lookup"><span data-stu-id="dbd40-116">Name</span></span>       | <span data-ttu-id="dbd40-117">Typ</span><span class="sxs-lookup"><span data-stu-id="dbd40-117">Type</span></span> | <span data-ttu-id="dbd40-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbd40-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbd40-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbd40-119">Authorization</span></span>  | <span data-ttu-id="dbd40-120">string</span><span class="sxs-lookup"><span data-stu-id="dbd40-120">string</span></span>  | <span data-ttu-id="dbd40-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dbd40-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbd40-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbd40-123">Content-Type</span></span> | <span data-ttu-id="dbd40-124">string</span><span class="sxs-lookup"><span data-stu-id="dbd40-124">string</span></span>  | <span data-ttu-id="dbd40-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dbd40-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbd40-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dbd40-127">Request body</span></span>
<span data-ttu-id="dbd40-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="dbd40-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbd40-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="dbd40-129">Parameter</span></span>    | <span data-ttu-id="dbd40-130">Typ</span><span class="sxs-lookup"><span data-stu-id="dbd40-130">Type</span></span>   |<span data-ttu-id="dbd40-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbd40-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbd40-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="dbd40-132">destinationId</span></span>|<span data-ttu-id="dbd40-133">String</span><span class="sxs-lookup"><span data-stu-id="dbd40-133">String</span></span>|<span data-ttu-id="dbd40-134">Die Zielordner-ID oder ein bekannter Ordnername wie *Posteingang*, *Entwürfe*, *Gesendete Objekte* oder *Gelöschte Objekte*.</span><span class="sxs-lookup"><span data-stu-id="dbd40-134">The destination folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="dbd40-135">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="dbd40-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="dbd40-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="dbd40-136">Response</span></span>

<span data-ttu-id="dbd40-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dbd40-137">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbd40-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dbd40-138">Example</span></span>
<span data-ttu-id="dbd40-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="dbd40-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dbd40-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dbd40-140">Request</span></span>
<span data-ttu-id="dbd40-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dbd40-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="dbd40-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="dbd40-142">Response</span></span>
<span data-ttu-id="dbd40-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dbd40-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
