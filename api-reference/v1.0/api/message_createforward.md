# <a name="message-createforward"></a><span data-ttu-id="4e58a-101">message: createForward</span><span class="sxs-lookup"><span data-stu-id="4e58a-101">message: createForward</span></span>

<span data-ttu-id="4e58a-p101">Erstellt einen Entwurf der Weiterleitungsnachricht. Sie können den Entwurf dann [aktualisieren](../api/message_update.md) oder [senden](../api/message_send.md).</span><span class="sxs-lookup"><span data-stu-id="4e58a-p101">Create a draft of the Forward message. You can then [update](../api/message_update.md) or [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e58a-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4e58a-104">Permissions</span></span>
<span data-ttu-id="4e58a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e58a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4e58a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e58a-107">Permission type</span></span>      | <span data-ttu-id="4e58a-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e58a-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4e58a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e58a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4e58a-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e58a-110">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="4e58a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e58a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e58a-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e58a-112">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="4e58a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e58a-113">Application</span></span> | <span data-ttu-id="4e58a-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e58a-114">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4e58a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e58a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="4e58a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e58a-116">Request headers</span></span>
| <span data-ttu-id="4e58a-117">Name</span><span class="sxs-lookup"><span data-stu-id="4e58a-117">Name</span></span>       | <span data-ttu-id="4e58a-118">Typ</span><span class="sxs-lookup"><span data-stu-id="4e58a-118">Type</span></span> | <span data-ttu-id="4e58a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e58a-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4e58a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e58a-120">Authorization</span></span>  | <span data-ttu-id="4e58a-121">string</span><span class="sxs-lookup"><span data-stu-id="4e58a-121">string</span></span>  | <span data-ttu-id="4e58a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e58a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e58a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e58a-124">Content-Type</span></span> | <span data-ttu-id="4e58a-125">string</span><span class="sxs-lookup"><span data-stu-id="4e58a-125">string</span></span>  | <span data-ttu-id="4e58a-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e58a-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e58a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e58a-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4e58a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e58a-129">Response</span></span>

<span data-ttu-id="4e58a-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e58a-130">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e58a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e58a-131">Example</span></span>
<span data-ttu-id="4e58a-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4e58a-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e58a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e58a-133">Request</span></span>
<span data-ttu-id="4e58a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e58a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
Content-type: application/json
Content-length: 248

{
  "comment": "Comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "address-value"
      }
    },
    {
      "emailAddress": {
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="4e58a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e58a-135">Response</span></span>
<span data-ttu-id="4e58a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e58a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
