# <a name="get-attachment"></a><span data-ttu-id="a9e4b-101">Anlage abrufen</span><span class="sxs-lookup"><span data-stu-id="a9e4b-101">Get attachment</span></span>

<span data-ttu-id="a9e4b-102">Lesen Sie die Eigenschaften und  Beziehungen einer Anlage, die einem [Ereignis](../resources/event.md), einer [Nachricht](../resources/message.md) oder einem [Beitrag](../resources/post.md) angehängt ist.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-102">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="a9e4b-103">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="a9e4b-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="a9e4b-104">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="a9e4b-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="a9e4b-p101">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource) Mithilfe von `$expand` können Sie die Eigenschaften des betreffenden Elements abrufen. Unten finden Sie ein [Beispiel](#request-2).</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p101">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="a9e4b-108">Link zu einer Datei ([referenceAttachment](../resources/referenceAttachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="a9e4b-108">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="a9e4b-109">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 


## <a name="permissions"></a><span data-ttu-id="a9e4b-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a9e4b-110">Permissions</span></span>
<span data-ttu-id="a9e4b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="a9e4b-113">Beim Zugriff auf Anlagen in Nachrichten: Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a9e4b-113">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="a9e4b-114">Beim Zugriff auf Anlagen in Ereignissen: Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a9e4b-114">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="a9e4b-115">Beim Zugriff auf Anlagen in Gruppenereignissen oder -beiträgen: Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9e4b-115">If accessing attachments in group events or posts: Group.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a9e4b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9e4b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a9e4b-117">Anlagen für ein [Ereignis](../resources/event.md) im Standard[kalender](../resources/calendar.md) des Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-117">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /groups/{id}/events/{id}/attachments/{id}

GET /me/calendar/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
```
<span data-ttu-id="a9e4b-118">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="a9e4b-119">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="a9e4b-120">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-120">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="a9e4b-121">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-121">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="a9e4b-p103">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="a9e4b-124">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9e4b-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a9e4b-125">Optional query parameters</span></span>
<span data-ttu-id="a9e4b-126">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a9e4b-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9e4b-127">Request headers</span></span>
| <span data-ttu-id="a9e4b-128">Name</span><span class="sxs-lookup"><span data-stu-id="a9e4b-128">Name</span></span>       | <span data-ttu-id="a9e4b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a9e4b-129">Type</span></span> | <span data-ttu-id="a9e4b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9e4b-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a9e4b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9e4b-131">Authorization</span></span>  | <span data-ttu-id="a9e4b-132">string</span><span class="sxs-lookup"><span data-stu-id="a9e4b-132">string</span></span>  | <span data-ttu-id="a9e4b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9e4b-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9e4b-135">Request body</span></span>
<span data-ttu-id="a9e4b-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9e4b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9e4b-137">Response</span></span>

<span data-ttu-id="a9e4b-p105">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein **attachment**-Objekt im Antworttext zurückgegeben. Die Eigenschaften des jeweiligen Anlagentyps werden zurückgegeben: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) oder [referenceAttachment](../resources/referenceAttachment.md).</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p105">If successful, this method returns a `200 OK` response code and an **attachment** object in the response body. The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md).</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a9e4b-140">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="a9e4b-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a9e4b-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9e4b-141">Request</span></span>
<span data-ttu-id="a9e4b-142">Hier finden Sie ein Beispiel für die Anforderung zum Abrufen einer Dateianlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-142">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a><span data-ttu-id="a9e4b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9e4b-143">Response</span></span>
<span data-ttu-id="a9e4b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "contentType": "contentType-value",
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
## <a name="example-item-attachment"></a><span data-ttu-id="a9e4b-147">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="a9e4b-147">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="a9e4b-148">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="a9e4b-148">Request 1</span></span>
<span data-ttu-id="a9e4b-p107">Im ersten Beispiel wird gezeigt, wie Sie eine Elementanlage zu einer Nachricht abrufen. Die Eigenschaften der **itemAttachment**-Ressource werden zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p107">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```

##### <a name="response-1"></a><span data-ttu-id="a9e4b-151">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="a9e4b-151">Response 1</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

##### <a name="request-2"></a><span data-ttu-id="a9e4b-152">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="a9e4b-152">Request 2</span></span>
<span data-ttu-id="a9e4b-p108">Im nächsten Beispiel wird gezeigt, wie Sie mit `$expand` die Eigenschaften des Elements abrufen, das an die Nachricht angefügt ist. In diesem Beispiel ist das Element eine Nachricht; die Eigenschaften der angefügten Nachricht werden ebenfalls zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p108">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item 
```

##### <a name="response-2"></a><span data-ttu-id="a9e4b-155">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="a9e4b-155">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



## <a name="example-reference-attachment"></a><span data-ttu-id="a9e4b-156">Beispiel (Verweisanlage)</span><span class="sxs-lookup"><span data-stu-id="a9e4b-156">Example (reference attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="a9e4b-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9e4b-157">Request</span></span>
<span data-ttu-id="a9e4b-158">Hier finden Sie ein Beispiel für die Anforderung zum Abrufen einer Verweisanlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-158">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="a9e4b-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9e4b-159">Response</span></span>
<span data-ttu-id="a9e4b-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9e4b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "contentType": "contentType-value",
  "lastModifiedDateTime": "datetime-value",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99,
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
