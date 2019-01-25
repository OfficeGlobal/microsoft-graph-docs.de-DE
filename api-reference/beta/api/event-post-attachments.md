---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine Anlage auf ein Ereignis hinzuzufügen. Seit dort
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ece15b579bae9e439eb9303c8b594631ce9b9b31
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525227"
---
# <a name="add-attachment"></a><span data-ttu-id="39a26-104">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="39a26-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39a26-p102">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Ereignis. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="39a26-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="39a26-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39a26-107">Permissions</span></span>

<span data-ttu-id="39a26-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39a26-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39a26-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39a26-110">Permission type</span></span>      | <span data-ttu-id="39a26-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39a26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39a26-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39a26-112">Delegated (work or school account)</span></span> | <span data-ttu-id="39a26-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39a26-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="39a26-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39a26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39a26-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39a26-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="39a26-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39a26-116">Application</span></span> | <span data-ttu-id="39a26-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39a26-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="39a26-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a26-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="39a26-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39a26-119">Request headers</span></span>

| <span data-ttu-id="39a26-120">Name</span><span class="sxs-lookup"><span data-stu-id="39a26-120">Name</span></span>       | <span data-ttu-id="39a26-121">Typ</span><span class="sxs-lookup"><span data-stu-id="39a26-121">Type</span></span> | <span data-ttu-id="39a26-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39a26-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="39a26-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39a26-123">Authorization</span></span>  | <span data-ttu-id="39a26-124">string</span><span class="sxs-lookup"><span data-stu-id="39a26-124">string</span></span>  | <span data-ttu-id="39a26-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39a26-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39a26-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39a26-127">Content-Type</span></span> | <span data-ttu-id="39a26-128">string</span><span class="sxs-lookup"><span data-stu-id="39a26-128">string</span></span>  | <span data-ttu-id="39a26-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39a26-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39a26-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39a26-131">Request body</span></span>

<span data-ttu-id="39a26-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="39a26-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="39a26-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a26-133">Response</span></span>

<span data-ttu-id="39a26-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39a26-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="39a26-135">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="39a26-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="39a26-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a26-136">Request</span></span>

<span data-ttu-id="39a26-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39a26-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="39a26-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="39a26-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="39a26-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a26-139">Response</span></span>

<span data-ttu-id="39a26-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39a26-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="39a26-143">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="39a26-143">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="39a26-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a26-144">Request</span></span>

<span data-ttu-id="39a26-145">Nachfolgend finden Sie ein Beispiel, in dem ein Ereignis als Elementanlage an ein anderes Element angefügt wird.</span><span class="sxs-lookup"><span data-stu-id="39a26-145">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

### <a name="response"></a><span data-ttu-id="39a26-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a26-146">Response</span></span>

<span data-ttu-id="39a26-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39a26-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="39a26-150">Beispiel (Verweisanlage)</span><span class="sxs-lookup"><span data-stu-id="39a26-150">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="39a26-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a26-151">Request</span></span>

<span data-ttu-id="39a26-152">Hier ist ein Beispiel für eine Anforderung, die eine Anlage Verweis auf ein vorhandenes Ereignis hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="39a26-152">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="39a26-153">Das Attachment-Objekt verweist auf einen Ordner auf OneDrive.</span><span class="sxs-lookup"><span data-stu-id="39a26-153">The attachment points to a folder on OneDrive.</span></span>
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

### <a name="response"></a><span data-ttu-id="39a26-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a26-154">Response</span></span>

<span data-ttu-id="39a26-155">Es folgt ein Beispiel einer vollständigen Antwort.</span><span class="sxs-lookup"><span data-stu-id="39a26-155">Here is an example of a full response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
