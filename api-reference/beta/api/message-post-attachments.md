---
title: Anlage hinzufügen
description: 'Verwenden Sie diese API zum Hinzufügen einer Anlage zu einer Nachricht. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fc24c0a444c07dc8fb8e33814498fe5454b1b3fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991902"
---
# <a name="add-attachment"></a><span data-ttu-id="58d30-103">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="58d30-103">Add attachment</span></span>

> <span data-ttu-id="58d30-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="58d30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58d30-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58d30-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58d30-106">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einer Nachricht.</span><span class="sxs-lookup"><span data-stu-id="58d30-106">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="58d30-107">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="58d30-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="58d30-108">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="58d30-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="58d30-109">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="58d30-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="58d30-110">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="58d30-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="58d30-111">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="58d30-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="58d30-112">Sie können eine Anlage zu einer vorhandenen Nachricht hinzufügen, indem das Veröffentlichen in der Attachments-Auflistung, oder an eine neue Nachricht werden, die [entworfen](../api/user-post-messages.md)oder [erstellt und gesendet, die dynamisch](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="58d30-112">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="58d30-113">Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="58d30-113">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="58d30-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="58d30-114">Permissions</span></span>
<span data-ttu-id="58d30-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58d30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58d30-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58d30-117">Permission type</span></span>      | <span data-ttu-id="58d30-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58d30-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58d30-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58d30-119">Delegated (work or school account)</span></span> | <span data-ttu-id="58d30-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58d30-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="58d30-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58d30-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58d30-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58d30-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="58d30-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58d30-123">Application</span></span> | <span data-ttu-id="58d30-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58d30-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="58d30-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58d30-125">HTTP request</span></span>
<span data-ttu-id="58d30-126"><!-- { "blockType": "ignored" } -->Anlagen für eine [Nachricht](../resources/message.md) im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="58d30-126"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="58d30-127">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="58d30-127">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="58d30-p103">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="58d30-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="58d30-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58d30-130">Request headers</span></span>
| <span data-ttu-id="58d30-131">Name</span><span class="sxs-lookup"><span data-stu-id="58d30-131">Name</span></span>       | <span data-ttu-id="58d30-132">Typ</span><span class="sxs-lookup"><span data-stu-id="58d30-132">Type</span></span> | <span data-ttu-id="58d30-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58d30-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58d30-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="58d30-134">Authorization</span></span>  | <span data-ttu-id="58d30-135">string</span><span class="sxs-lookup"><span data-stu-id="58d30-135">string</span></span>  | <span data-ttu-id="58d30-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58d30-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58d30-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58d30-138">Content-Type</span></span> | <span data-ttu-id="58d30-139">string</span><span class="sxs-lookup"><span data-stu-id="58d30-139">string</span></span>  | <span data-ttu-id="58d30-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58d30-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58d30-142">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58d30-142">Request body</span></span>
<span data-ttu-id="58d30-143">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="58d30-143">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="58d30-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="58d30-144">Response</span></span>

<span data-ttu-id="58d30-145">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und [Attachment](../resources/attachment.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="58d30-145">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="58d30-146">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="58d30-146">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="58d30-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58d30-147">Request</span></span>
<span data-ttu-id="58d30-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58d30-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="58d30-149">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="58d30-149">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="58d30-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="58d30-150">Response</span></span>
<span data-ttu-id="58d30-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="58d30-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 202

{
    "id": "AAMkADNkN2R",
    "lastModifiedDateTime": "2017-01-26T08:48:28Z",
    "name": "smile",
    "contentType": "image/gif",
    "size": 1008,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "R0lGODdhEAYEAA7"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="58d30-152">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="58d30-152">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="58d30-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58d30-153">Request</span></span>
<span data-ttu-id="58d30-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58d30-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
    "@odata.type": "microsoft.graph.event",
    "subject": "Discuss gifts for children",
    "body": {
      "contentType": "HTML",
      "content": "Let's look for funding!"
    },
    "start": {
      "dateTime": "2016-12-02T18:00:00",
      "timeZone": "Pacific Standard Time"
    },
    "end": {
      "dateTime": "2016-12-02T19:00:00",
      "timeZone": "Pacific Standard Time"
    }
  }
}

```

##### <a name="response"></a><span data-ttu-id="58d30-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="58d30-155">Response</span></span>
<span data-ttu-id="58d30-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58d30-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "id":"AAMkADNkNJp5JVnQIe9r0=",
  "lastModifiedDateTime":"2016-12-01T22:27:13Z",
  "name":"Holiday event",
  "contentType":null,
  "size":2473,
  "isInline":false
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="58d30-159">Beispiel (Verweisanlage)</span><span class="sxs-lookup"><span data-stu-id="58d30-159">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="58d30-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58d30-160">Request</span></span>
<span data-ttu-id="58d30-161">Hier ist ein Beispiel für eine Anforderung, die eine Anlage Verweis auf eine vorhandene Nachricht hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="58d30-161">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="58d30-162">Das Attachment-Objekt verweist auf einen Ordner auf OneDrive.</span><span class="sxs-lookup"><span data-stu-id="58d30-162">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_message",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M88AADUv0uFAAA=/attachments
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

##### <a name="response"></a><span data-ttu-id="58d30-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="58d30-163">Response</span></span>
<span data-ttu-id="58d30-164">Es folgt ein Beispiel einer vollständigen Antwort.</span><span class="sxs-lookup"><span data-stu-id="58d30-164">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/messages/AAMkAGE1M88AADUv0uFAAA%3D/attachments/$entity",
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
