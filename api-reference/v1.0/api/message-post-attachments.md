---
title: Anlage hinzufügen
description: 'Verwenden Sie diese API zum Hinzufügen einer Anlage zu einer Nachricht. '
author: angelgolfer-ms
ms.openlocfilehash: 868ce046a37d027c675b005cef013892deffe2a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314616"
---
# <a name="add-attachment"></a><span data-ttu-id="37e1a-103">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="37e1a-103">Add attachment</span></span>

<span data-ttu-id="37e1a-104">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einer Nachricht.</span><span class="sxs-lookup"><span data-stu-id="37e1a-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="37e1a-105">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="37e1a-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="37e1a-106">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="37e1a-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="37e1a-107">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="37e1a-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="37e1a-108">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="37e1a-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="37e1a-109">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="37e1a-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="37e1a-110">Sie können eine Anlage zu einer vorhandenen Nachricht hinzufügen, indem Sie sie in ihrer Anlagensammlung veröffentlichen, oder Sie können eine Anlage zu einer Nachricht hinzufügen, die gerade [erstellt wird und im laufenden Betrieb gesendet wird](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="37e1a-110">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="37e1a-111">Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="37e1a-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="37e1a-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="37e1a-112">Permissions</span></span>
<span data-ttu-id="37e1a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e1a-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37e1a-115">Permission type</span></span>      | <span data-ttu-id="37e1a-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37e1a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37e1a-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37e1a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="37e1a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37e1a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="37e1a-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37e1a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37e1a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37e1a-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="37e1a-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37e1a-121">Application</span></span> | <span data-ttu-id="37e1a-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37e1a-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="37e1a-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37e1a-123">HTTP request</span></span>
<span data-ttu-id="37e1a-124"><!-- { "blockType": "ignored" } -->Anlagen für eine [Nachricht](../resources/message.md) im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="37e1a-124"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="37e1a-125">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="37e1a-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="37e1a-p102">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="37e1a-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="37e1a-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37e1a-128">Request headers</span></span>
| <span data-ttu-id="37e1a-129">Name</span><span class="sxs-lookup"><span data-stu-id="37e1a-129">Name</span></span>       | <span data-ttu-id="37e1a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="37e1a-130">Type</span></span> | <span data-ttu-id="37e1a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37e1a-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="37e1a-132">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="37e1a-132">Authorization</span></span>  | <span data-ttu-id="37e1a-133">string</span><span class="sxs-lookup"><span data-stu-id="37e1a-133">string</span></span>  | <span data-ttu-id="37e1a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="37e1a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37e1a-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37e1a-136">Content-Type</span></span> | <span data-ttu-id="37e1a-137">string</span><span class="sxs-lookup"><span data-stu-id="37e1a-137">string</span></span>  | <span data-ttu-id="37e1a-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="37e1a-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37e1a-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37e1a-140">Request body</span></span>
<span data-ttu-id="37e1a-141">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="37e1a-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="37e1a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="37e1a-142">Response</span></span>

<span data-ttu-id="37e1a-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37e1a-143">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="37e1a-144">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="37e1a-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="37e1a-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37e1a-145">Request</span></span>
<span data-ttu-id="37e1a-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37e1a-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "base64R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="37e1a-147">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="37e1a-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="37e1a-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="37e1a-148">Response</span></span>
<span data-ttu-id="37e1a-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="37e1a-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP 201 Created
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
    "contentBytes": "base64R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="37e1a-150">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="37e1a-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="37e1a-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37e1a-151">Request</span></span>
<span data-ttu-id="37e1a-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37e1a-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_item_attachment_from_message"
}-->

```
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
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

##### <a name="response"></a><span data-ttu-id="37e1a-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="37e1a-153">Response</span></span>
<span data-ttu-id="37e1a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37e1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
