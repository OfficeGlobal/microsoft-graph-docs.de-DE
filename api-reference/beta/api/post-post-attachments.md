---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine Anlage auf einen Beitrag hinzuzufügen. Seit dort
ms.openlocfilehash: 38126f015d19890a9a1f08d458f05505faa09e9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059387"
---
# <a name="add-attachment"></a><span data-ttu-id="8d27d-104">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8d27d-104">Add attachment</span></span>

> <span data-ttu-id="8d27d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d27d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d27d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d27d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d27d-p103">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Beitrag. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="8d27d-p103">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="8d27d-109">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="8d27d-109">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="8d27d-110">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="8d27d-110">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="8d27d-111">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="8d27d-111">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="8d27d-112">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="8d27d-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="8d27d-113">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="8d27d-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8d27d-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8d27d-114">Permissions</span></span>
<span data-ttu-id="8d27d-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d27d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d27d-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d27d-117">Permission type</span></span>      | <span data-ttu-id="8d27d-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d27d-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d27d-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d27d-119">Delegated (work or school account)</span></span> | <span data-ttu-id="8d27d-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d27d-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d27d-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d27d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d27d-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d27d-122">Not supported.</span></span>    |
|<span data-ttu-id="8d27d-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d27d-123">Application</span></span> | <span data-ttu-id="8d27d-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d27d-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d27d-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d27d-125">HTTP request</span></span>
<span data-ttu-id="8d27d-126"><!-- { "blockType": "ignored" } -->Anlagen für einen [Posten](../resources/post.md) in einem [Thread](../resources/conversationthread.md) , die zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehören.</span><span class="sxs-lookup"><span data-stu-id="8d27d-126"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="8d27d-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d27d-127">Request headers</span></span>
| <span data-ttu-id="8d27d-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d27d-128">Header</span></span>       | <span data-ttu-id="8d27d-129">Wert</span><span class="sxs-lookup"><span data-stu-id="8d27d-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d27d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d27d-130">Authorization</span></span>  | <span data-ttu-id="8d27d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8d27d-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d27d-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d27d-133">Request body</span></span>
<span data-ttu-id="8d27d-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8d27d-134">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8d27d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d27d-135">Response</span></span>

<span data-ttu-id="8d27d-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d27d-136">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="8d27d-137">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="8d27d-137">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8d27d-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d27d-138">Request</span></span>
<span data-ttu-id="8d27d-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d27d-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="8d27d-140">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8d27d-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="8d27d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d27d-141">Response</span></span>
<span data-ttu-id="8d27d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d27d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="8d27d-145">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="8d27d-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8d27d-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d27d-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="8d27d-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d27d-147">Response</span></span>
<span data-ttu-id="8d27d-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d27d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


## <a name="example-reference-attachment"></a><span data-ttu-id="8d27d-151">Beispiel (Verweisanlage)</span><span class="sxs-lookup"><span data-stu-id="8d27d-151">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8d27d-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d27d-152">Request</span></span>
<span data-ttu-id="8d27d-153">Es folgt ein Beispiel einer Anforderung, die eine Anlage Verweis auf einen vorhandenen Beitrag hinzufügt.</span><span class="sxs-lookup"><span data-stu-id="8d27d-153">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="8d27d-154">Das Attachment-Objekt verweist auf einen Ordner auf OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8d27d-154">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_post",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```

##### <a name="response"></a><span data-ttu-id="8d27d-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d27d-155">Response</span></span>
<span data-ttu-id="8d27d-156">Es folgt ein Beispiel einer vollständigen Antwort.</span><span class="sxs-lookup"><span data-stu-id="8d27d-156">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
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
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
