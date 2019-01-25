---
title: Anlage hinzufügen
description: 'Verwenden Sie diese API zum Hinzufügen einer Anlage zu einer Nachricht. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 56693a04d6f0579d043b4d745fe53ae61536b82e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510092"
---
# <a name="add-attachment"></a><span data-ttu-id="11a37-103">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="11a37-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11a37-104">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einer Nachricht.</span><span class="sxs-lookup"><span data-stu-id="11a37-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="11a37-105">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="11a37-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="11a37-106">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="11a37-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="11a37-107">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="11a37-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="11a37-108">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="11a37-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="11a37-109">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="11a37-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="11a37-110">Sie können eine Anlage zu einer vorhandenen Nachricht hinzufügen, indem das Veröffentlichen in der Attachments-Auflistung, oder an eine neue Nachricht werden, die [entworfen](../api/user-post-messages.md)oder [erstellt und gesendet, die dynamisch](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="11a37-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="11a37-111">Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="11a37-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="11a37-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11a37-112">Permissions</span></span>
<span data-ttu-id="11a37-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11a37-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11a37-115">Permission type</span></span>      | <span data-ttu-id="11a37-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11a37-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11a37-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11a37-117">Delegated (work or school account)</span></span> | <span data-ttu-id="11a37-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11a37-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11a37-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11a37-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11a37-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11a37-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11a37-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11a37-121">Application</span></span> | <span data-ttu-id="11a37-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11a37-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="11a37-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11a37-123">HTTP request</span></span>
<span data-ttu-id="11a37-124"><!-- { "blockType": "ignored" } -->Anlagen für eine [Nachricht](../resources/message.md) im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="11a37-124"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="11a37-125">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="11a37-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="11a37-p102">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="11a37-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="11a37-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11a37-128">Request headers</span></span>
| <span data-ttu-id="11a37-129">Name</span><span class="sxs-lookup"><span data-stu-id="11a37-129">Name</span></span>       | <span data-ttu-id="11a37-130">Typ</span><span class="sxs-lookup"><span data-stu-id="11a37-130">Type</span></span> | <span data-ttu-id="11a37-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11a37-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11a37-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="11a37-132">Authorization</span></span>  | <span data-ttu-id="11a37-133">string</span><span class="sxs-lookup"><span data-stu-id="11a37-133">string</span></span>  | <span data-ttu-id="11a37-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11a37-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11a37-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11a37-136">Content-Type</span></span> | <span data-ttu-id="11a37-137">string</span><span class="sxs-lookup"><span data-stu-id="11a37-137">string</span></span>  | <span data-ttu-id="11a37-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11a37-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11a37-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11a37-140">Request body</span></span>
<span data-ttu-id="11a37-141">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="11a37-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="11a37-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="11a37-142">Response</span></span>

<span data-ttu-id="11a37-143">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und [Attachment](../resources/attachment.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11a37-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="11a37-144">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="11a37-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="11a37-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11a37-145">Request</span></span>
<span data-ttu-id="11a37-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11a37-146">Here is an example of the request.</span></span>
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

<span data-ttu-id="11a37-147">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="11a37-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="11a37-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="11a37-148">Response</span></span>
<span data-ttu-id="11a37-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11a37-149">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="11a37-150">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="11a37-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="11a37-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11a37-151">Request</span></span>
<span data-ttu-id="11a37-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11a37-152">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="11a37-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="11a37-153">Response</span></span>
<span data-ttu-id="11a37-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11a37-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="11a37-157">Beispiel (Verweisanlage)</span><span class="sxs-lookup"><span data-stu-id="11a37-157">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="11a37-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11a37-158">Request</span></span>
<span data-ttu-id="11a37-159">Hier ist ein Beispiel für eine Anforderung, die eine Anlage Verweis auf eine vorhandene Nachricht hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="11a37-159">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="11a37-160">Das Attachment-Objekt verweist auf einen Ordner auf OneDrive.</span><span class="sxs-lookup"><span data-stu-id="11a37-160">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="11a37-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="11a37-161">Response</span></span>
<span data-ttu-id="11a37-162">Es folgt ein Beispiel einer vollständigen Antwort.</span><span class="sxs-lookup"><span data-stu-id="11a37-162">Here is an example of a full response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
