---
title: Anlage abrufen
description: Lesen Sie die Eigenschaften und Beziehungen der Anlage, die ein Ereignis, Nachricht, Outlook-Aufgabe oder Post zugeordnet ist.
ms.openlocfilehash: 040e6995a24fcff62e8e7f476afdc602a6c9617c
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771814"
---
# <a name="get-attachment"></a><span data-ttu-id="4e5b5-103">Anlage abrufen</span><span class="sxs-lookup"><span data-stu-id="4e5b5-103">Get attachment</span></span>

> <span data-ttu-id="4e5b5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e5b5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e5b5-106">Lesen Sie die Eigenschaften und Beziehungen der Anlage, die ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-106">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

<span data-ttu-id="4e5b5-107">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="4e5b5-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="4e5b5-108">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="4e5b5-p102">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource) Mithilfe von `$expand` können Sie die Eigenschaften des betreffenden Elements abrufen. Unten finden Sie ein [Beispiel](#request-2).</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p102">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="4e5b5-112">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="4e5b5-113">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e5b5-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4e5b5-114">Permissions</span></span>

<span data-ttu-id="4e5b5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="4e5b5-117">Wenn Anlagen in Nachrichten zugreifen: Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4e5b5-117">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="4e5b5-118">Wenn das Zugreifen auf Anlagen in Ereignisse: Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4e5b5-118">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="4e5b5-119">Wenn auf Anlagen in Outlook-Aufgaben zugreifen: Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="4e5b5-119">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="4e5b5-120">Wenn Anlagen in der Gruppe Beiträge zugreifen: Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e5b5-120">If accessing attachments in group posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="4e5b5-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e5b5-121">HTTP request</span></span>

<span data-ttu-id="4e5b5-122">Anlagen für ein [Ereignis](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="4e5b5-122">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="4e5b5-123">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-123">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="4e5b5-124">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-124">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="4e5b5-125">Anlagen für eine [Nachricht](../resources/message.md) , die in einem untergeordneten Ordner von einem [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-125">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="4e5b5-126">Das folgende Beispiel zeigt eine Ebene von schachteln, aber eine Nachricht kann befinden in ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-126">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="4e5b5-127">Anlagen für ein [Outlook-Aufgabe](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="4e5b5-127">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="4e5b5-128">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-128">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e5b5-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4e5b5-129">Optional query parameters</span></span>

<span data-ttu-id="4e5b5-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e5b5-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e5b5-131">Request headers</span></span>

| <span data-ttu-id="4e5b5-132">Name</span><span class="sxs-lookup"><span data-stu-id="4e5b5-132">Name</span></span>       | <span data-ttu-id="4e5b5-133">Typ</span><span class="sxs-lookup"><span data-stu-id="4e5b5-133">Type</span></span> | <span data-ttu-id="4e5b5-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e5b5-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4e5b5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e5b5-135">Authorization</span></span>  | <span data-ttu-id="4e5b5-136">string</span><span class="sxs-lookup"><span data-stu-id="4e5b5-136">string</span></span>  | <span data-ttu-id="4e5b5-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e5b5-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e5b5-139">Request body</span></span>

<span data-ttu-id="4e5b5-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e5b5-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e5b5-141">Response</span></span>

<span data-ttu-id="4e5b5-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-142">If successful, this method returns a `200 OK` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="4e5b5-143">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-143">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="4e5b5-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e5b5-144">Request</span></span>

<span data-ttu-id="4e5b5-145">Hier finden Sie ein Beispiel für die Anforderung zum Abrufen einer Dateianlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-145">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="4e5b5-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e5b5-146">Response</span></span>

<span data-ttu-id="4e5b5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="4e5b5-150">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-150">Example (item attachment)</span></span>

### <a name="request-1"></a><span data-ttu-id="4e5b5-151">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="4e5b5-151">Request 1</span></span>

<span data-ttu-id="4e5b5-p107">Im ersten Beispiel wird gezeigt, wie Sie eine Elementanlage zu einer Nachricht abrufen. Die Eigenschaften der **itemAttachment**-Ressource werden zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p107">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```

### <a name="response-1"></a><span data-ttu-id="4e5b5-154">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="4e5b5-154">Response 1</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="request-2"></a><span data-ttu-id="4e5b5-155">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="4e5b5-155">Request 2</span></span>

<span data-ttu-id="4e5b5-p108">Im nächsten Beispiel wird gezeigt, wie Sie mit `$expand` die Eigenschaften des Elements abrufen, das an die Nachricht angefügt ist. In diesem Beispiel ist das Element eine Nachricht; die Eigenschaften der angefügten Nachricht werden ebenfalls zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p108">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```

### <a name="response-2"></a><span data-ttu-id="4e5b5-158">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="4e5b5-158">Response 2</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
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
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
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
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="4e5b5-159">Beispiel (Verweisanlage)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-159">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="4e5b5-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e5b5-160">Request</span></span>

<span data-ttu-id="4e5b5-161">Hier finden Sie ein Beispiel für die Anforderung zum Abrufen einer Verweisanlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-161">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```

### <a name="response"></a><span data-ttu-id="4e5b5-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e5b5-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
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
