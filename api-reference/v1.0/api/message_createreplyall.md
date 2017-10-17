# <a name="message-createreplyall"></a><span data-ttu-id="ebab4-101">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="ebab4-101">message: createReplyAll</span></span>

<span data-ttu-id="ebab4-102">Erstellen Sie einen Entwurf, um dem Absender und allen Empfängern der angegebenen [Nachricht](../resources/message.md) zu antworten.</span><span class="sxs-lookup"><span data-stu-id="ebab4-102">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="ebab4-103">Anschließend können Sie den Entwurf [aktualisieren](../api/message_update.md), um den Antwortinhalt zum **Text** hinzuzufügen, oder andere Nachrichteneigenschaften ändern. Sie können den Entwurf auch einfach [senden](../api/message_send.md).</span><span class="sxs-lookup"><span data-stu-id="ebab4-103">You can then [update](../api/message_update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebab4-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ebab4-104">Permissions</span></span>
<span data-ttu-id="ebab4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ebab4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ebab4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebab4-107">Permission type</span></span>      | <span data-ttu-id="ebab4-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebab4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebab4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebab4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ebab4-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebab4-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ebab4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebab4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebab4-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebab4-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ebab4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebab4-113">Application</span></span> | <span data-ttu-id="ebab4-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebab4-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebab4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebab4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="ebab4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebab4-116">Request headers</span></span>
| <span data-ttu-id="ebab4-117">Name</span><span class="sxs-lookup"><span data-stu-id="ebab4-117">Name</span></span>       | <span data-ttu-id="ebab4-118">Typ</span><span class="sxs-lookup"><span data-stu-id="ebab4-118">Type</span></span> | <span data-ttu-id="ebab4-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebab4-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ebab4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebab4-120">Authorization</span></span>  | <span data-ttu-id="ebab4-121">string</span><span class="sxs-lookup"><span data-stu-id="ebab4-121">string</span></span>  | <span data-ttu-id="ebab4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ebab4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebab4-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebab4-124">Request body</span></span>
<span data-ttu-id="ebab4-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ebab4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebab4-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebab4-126">Response</span></span>

<span data-ttu-id="ebab4-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebab4-127">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebab4-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebab4-128">Example</span></span>
<span data-ttu-id="ebab4-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ebab4-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ebab4-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebab4-130">Request</span></span>
<span data-ttu-id="ebab4-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebab4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```

##### <a name="response"></a><span data-ttu-id="ebab4-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebab4-132">Response</span></span>
<span data-ttu-id="ebab4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebab4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
