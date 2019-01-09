---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine Anlage auf ein Ereignis hinzuzufügen. Seit dort
author: angelgolfer-ms
ms.openlocfilehash: 071ecdecf3ac7fd835c7c5004463661b685be003
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771772"
---
# <a name="add-attachment"></a><span data-ttu-id="1114b-104">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="1114b-104">Add attachment</span></span>

> <span data-ttu-id="1114b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1114b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1114b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1114b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1114b-p103">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Ereignis. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="1114b-p103">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="1114b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1114b-109">Permissions</span></span>

<span data-ttu-id="1114b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1114b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1114b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1114b-112">Permission type</span></span>      | <span data-ttu-id="1114b-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1114b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1114b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1114b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1114b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1114b-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1114b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1114b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1114b-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1114b-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1114b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1114b-118">Application</span></span> | <span data-ttu-id="1114b-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1114b-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1114b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1114b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="1114b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1114b-121">Request headers</span></span>

| <span data-ttu-id="1114b-122">Name</span><span class="sxs-lookup"><span data-stu-id="1114b-122">Name</span></span>       | <span data-ttu-id="1114b-123">Typ</span><span class="sxs-lookup"><span data-stu-id="1114b-123">Type</span></span> | <span data-ttu-id="1114b-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1114b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1114b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1114b-125">Authorization</span></span>  | <span data-ttu-id="1114b-126">string</span><span class="sxs-lookup"><span data-stu-id="1114b-126">string</span></span>  | <span data-ttu-id="1114b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1114b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1114b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1114b-129">Content-Type</span></span> | <span data-ttu-id="1114b-130">string</span><span class="sxs-lookup"><span data-stu-id="1114b-130">string</span></span>  | <span data-ttu-id="1114b-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1114b-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1114b-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1114b-133">Request body</span></span>

<span data-ttu-id="1114b-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1114b-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1114b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1114b-135">Response</span></span>

<span data-ttu-id="1114b-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1114b-136">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="1114b-137">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="1114b-137">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="1114b-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1114b-138">Request</span></span>

<span data-ttu-id="1114b-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1114b-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

<span data-ttu-id="1114b-140">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1114b-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="1114b-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="1114b-141">Response</span></span>

<span data-ttu-id="1114b-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1114b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="1114b-145">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="1114b-145">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="1114b-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1114b-146">Request</span></span>

<span data-ttu-id="1114b-147">Nachfolgend finden Sie ein Beispiel, in dem ein Ereignis als Elementanlage an ein anderes Element angefügt wird.</span><span class="sxs-lookup"><span data-stu-id="1114b-147">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
Content-type: application/json
Content-length: 600

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

### <a name="response"></a><span data-ttu-id="1114b-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="1114b-148">Response</span></span>

<span data-ttu-id="1114b-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1114b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/beta/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="1114b-152">Beispiel (Verweisanlage)</span><span class="sxs-lookup"><span data-stu-id="1114b-152">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="1114b-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1114b-153">Request</span></span>

<span data-ttu-id="1114b-154">Hier ist ein Beispiel für eine Anforderung, die eine Anlage Verweis auf ein vorhandenes Ereignis hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1114b-154">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="1114b-155">Das Attachment-Objekt verweist auf einen Ordner auf OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1114b-155">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments
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

### <a name="response"></a><span data-ttu-id="1114b-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="1114b-156">Response</span></span>

<span data-ttu-id="1114b-157">Es folgt ein Beispiel einer vollständigen Antwort.</span><span class="sxs-lookup"><span data-stu-id="1114b-157">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP 201 Created

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
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
