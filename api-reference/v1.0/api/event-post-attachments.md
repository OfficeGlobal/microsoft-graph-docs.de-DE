---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine Anlage auf ein Ereignis hinzuzufügen. Seit dort
ms.openlocfilehash: e64a012738c0b742c83e6baa247746daaf16dcdf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018920"
---
# <a name="add-attachment"></a><span data-ttu-id="f5cd3-104">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f5cd3-104">Add attachment</span></span>

<span data-ttu-id="f5cd3-p102">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Ereignis. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5cd3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5cd3-107">Permissions</span></span>
<span data-ttu-id="f5cd3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5cd3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5cd3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5cd3-110">Permission type</span></span>      | <span data-ttu-id="f5cd3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5cd3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5cd3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5cd3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5cd3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5cd3-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f5cd3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5cd3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5cd3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5cd3-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f5cd3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5cd3-116">Application</span></span> | <span data-ttu-id="f5cd3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5cd3-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5cd3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5cd3-118">HTTP request</span></span>
<span data-ttu-id="f5cd3-119">Anlagen für ein [Ereignis](../resources/event.md) in der Benutzer als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="f5cd3-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="f5cd3-120">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="f5cd3-121">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="f5cd3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5cd3-122">Request headers</span></span>
| <span data-ttu-id="f5cd3-123">Name</span><span class="sxs-lookup"><span data-stu-id="f5cd3-123">Name</span></span>       | <span data-ttu-id="f5cd3-124">Typ</span><span class="sxs-lookup"><span data-stu-id="f5cd3-124">Type</span></span> | <span data-ttu-id="f5cd3-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5cd3-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5cd3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5cd3-126">Authorization</span></span>  | <span data-ttu-id="f5cd3-127">string</span><span class="sxs-lookup"><span data-stu-id="f5cd3-127">string</span></span>  | <span data-ttu-id="f5cd3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5cd3-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5cd3-130">Content-Type</span></span> | <span data-ttu-id="f5cd3-131">string</span><span class="sxs-lookup"><span data-stu-id="f5cd3-131">string</span></span>  | <span data-ttu-id="f5cd3-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5cd3-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5cd3-134">Request body</span></span>
<span data-ttu-id="f5cd3-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f5cd3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5cd3-136">Response</span></span>

<span data-ttu-id="f5cd3-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-137">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f5cd3-138">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="f5cd3-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f5cd3-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5cd3-139">Request</span></span>
<span data-ttu-id="f5cd3-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_file_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```

<span data-ttu-id="f5cd3-141">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-141">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f5cd3-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5cd3-142">Response</span></span>
<span data-ttu-id="f5cd3-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="f5cd3-144">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="f5cd3-144">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f5cd3-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5cd3-145">Request</span></span>

<span data-ttu-id="f5cd3-146">Nachfolgend finden Sie ein Beispiel, in dem ein Ereignis als Elementanlage an ein anderes Element angefügt wird.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-146">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_item_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
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

##### <a name="response"></a><span data-ttu-id="f5cd3-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5cd3-147">Response</span></span>
<span data-ttu-id="f5cd3-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5cd3-148">Here is an example of the response.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
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