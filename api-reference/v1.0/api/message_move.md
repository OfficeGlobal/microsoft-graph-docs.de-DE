# <a name="message-move"></a><span data-ttu-id="464ec-101">message: move</span><span class="sxs-lookup"><span data-stu-id="464ec-101">message: move</span></span>

<span data-ttu-id="464ec-p101">Verschiebt eine Nachricht in einen Ordner. Dadurch wird eine neue Kopie der Nachricht im Zielordner erstellt.</span><span class="sxs-lookup"><span data-stu-id="464ec-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="464ec-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="464ec-104">Permissions</span></span>
<span data-ttu-id="464ec-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="464ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="464ec-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="464ec-107">Permission type</span></span>      | <span data-ttu-id="464ec-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="464ec-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="464ec-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="464ec-109">Delegated (work or school account)</span></span> | <span data-ttu-id="464ec-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="464ec-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="464ec-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="464ec-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="464ec-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="464ec-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="464ec-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="464ec-113">Application</span></span> | <span data-ttu-id="464ec-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="464ec-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="464ec-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="464ec-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="464ec-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="464ec-116">Request headers</span></span>
| <span data-ttu-id="464ec-117">Name</span><span class="sxs-lookup"><span data-stu-id="464ec-117">Name</span></span>       | <span data-ttu-id="464ec-118">Typ</span><span class="sxs-lookup"><span data-stu-id="464ec-118">Type</span></span> | <span data-ttu-id="464ec-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="464ec-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="464ec-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="464ec-120">Authorization</span></span>  | <span data-ttu-id="464ec-121">string</span><span class="sxs-lookup"><span data-stu-id="464ec-121">string</span></span>  | <span data-ttu-id="464ec-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="464ec-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="464ec-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="464ec-124">Content-Type</span></span> | <span data-ttu-id="464ec-125">string</span><span class="sxs-lookup"><span data-stu-id="464ec-125">string</span></span>  | <span data-ttu-id="464ec-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="464ec-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="464ec-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="464ec-128">Request body</span></span>
<span data-ttu-id="464ec-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="464ec-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="464ec-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="464ec-130">Parameter</span></span>    | <span data-ttu-id="464ec-131">Typ</span><span class="sxs-lookup"><span data-stu-id="464ec-131">Type</span></span>   |<span data-ttu-id="464ec-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="464ec-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="464ec-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="464ec-133">DestinationId</span></span>|<span data-ttu-id="464ec-134">String</span><span class="sxs-lookup"><span data-stu-id="464ec-134">String</span></span>|<span data-ttu-id="464ec-135">Die Zielordner-ID oder ein bekannter Ordnername wie *Posteingang*, *Entwürfe*, *Gesendete Objekte* oder *Gelöschte Objekte*.</span><span class="sxs-lookup"><span data-stu-id="464ec-135">The destination folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="464ec-136">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="464ec-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="464ec-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="464ec-137">Response</span></span>

<span data-ttu-id="464ec-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="464ec-138">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="464ec-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="464ec-139">Example</span></span>
<span data-ttu-id="464ec-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="464ec-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="464ec-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="464ec-141">Request</span></span>
<span data-ttu-id="464ec-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="464ec-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="464ec-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="464ec-143">Response</span></span>
<span data-ttu-id="464ec-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="464ec-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
