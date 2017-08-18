# <a name="message-move"></a><span data-ttu-id="d56d4-101">message: move</span><span class="sxs-lookup"><span data-stu-id="d56d4-101">message: move</span></span>

<span data-ttu-id="d56d4-p101">Verschiebt eine Nachricht in einen Ordner. Dadurch wird eine neue Kopie der Nachricht im Zielordner erstellt.</span><span class="sxs-lookup"><span data-stu-id="d56d4-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d56d4-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="d56d4-104">Prerequisites</span></span>
<span data-ttu-id="d56d4-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="d56d4-105">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="d56d4-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d56d4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="d56d4-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d56d4-107">Request headers</span></span>
| <span data-ttu-id="d56d4-108">Name</span><span class="sxs-lookup"><span data-stu-id="d56d4-108">Name</span></span>       | <span data-ttu-id="d56d4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d56d4-109">Type</span></span> | <span data-ttu-id="d56d4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d56d4-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d56d4-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="d56d4-111">Authorization</span></span>  | <span data-ttu-id="d56d4-112">string</span><span class="sxs-lookup"><span data-stu-id="d56d4-112">string</span></span>  | <span data-ttu-id="d56d4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d56d4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d56d4-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d56d4-115">Content-Type</span></span> | <span data-ttu-id="d56d4-116">string</span><span class="sxs-lookup"><span data-stu-id="d56d4-116">string</span></span>  | <span data-ttu-id="d56d4-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d56d4-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d56d4-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d56d4-119">Request body</span></span>
<span data-ttu-id="d56d4-120">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d56d4-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d56d4-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="d56d4-121">Parameter</span></span>    | <span data-ttu-id="d56d4-122">Typ</span><span class="sxs-lookup"><span data-stu-id="d56d4-122">Type</span></span>   |<span data-ttu-id="d56d4-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d56d4-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d56d4-124">DestinationId</span><span class="sxs-lookup"><span data-stu-id="d56d4-124">DestinationId</span></span>|<span data-ttu-id="d56d4-125">String</span><span class="sxs-lookup"><span data-stu-id="d56d4-125">String</span></span>|<span data-ttu-id="d56d4-126">Die ID des Zielordners oder der bekannte Ordnername `Inbox`, `Drafts`, `SentItems` oder `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="d56d4-126">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="d56d4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d56d4-127">Response</span></span>

<span data-ttu-id="d56d4-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d56d4-128">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d56d4-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d56d4-129">Example</span></span>
<span data-ttu-id="d56d4-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d56d4-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d56d4-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d56d4-131">Request</span></span>
<span data-ttu-id="d56d4-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d56d4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/move
Content-type: application/json
Content-length: 44

{
  "DestinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="d56d4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d56d4-133">Response</span></span>
<span data-ttu-id="d56d4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d56d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
