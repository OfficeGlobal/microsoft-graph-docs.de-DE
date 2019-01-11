---
title: Anlage löschen
description: Mit dieser API können Sie Anlagen aus Kalenderereignissen, E-Mail-Nachrichten oder Gruppenbeiträgen löschen.
localization_priority: Normal
ms.openlocfilehash: f6ac2e60c9fdc8a224e22a49e6928cdc41e9730b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816996"
---
# <a name="delete-attachment"></a><span data-ttu-id="b0d45-103">Anlage löschen</span><span class="sxs-lookup"><span data-stu-id="b0d45-103">Delete attachment</span></span>

<span data-ttu-id="b0d45-104">Mit dieser API können Sie Anlagen aus Kalenderereignissen, E-Mail-Nachrichten oder Gruppenbeiträgen löschen.</span><span class="sxs-lookup"><span data-stu-id="b0d45-104">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0d45-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b0d45-105">Permissions</span></span>
<span data-ttu-id="b0d45-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0d45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="b0d45-108">Wenn Anlagen in Nachrichten zugreifen: Mail.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b0d45-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="b0d45-109">Wenn Anlagen in Ereignisse zugreifen: Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b0d45-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="b0d45-110">Wenn Anlagen in der Gruppe Beiträge zugreifen: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="b0d45-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="b0d45-111">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0d45-111">HTTP request</span></span>
<span data-ttu-id="b0d45-112">Anlagen für ein [Ereignis](../resources/event.md) im Standard[kalender](../resources/calendar.md) des Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="b0d45-112">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="b0d45-113">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b0d45-113">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="b0d45-114">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b0d45-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="b0d45-115">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b0d45-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b0d45-116">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b0d45-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b0d45-117">Anlagen für eine [Nachricht](../resources/message.md) , die in einem untergeordneten Ordner von einem [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="b0d45-117">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="b0d45-118">Das folgende Beispiel zeigt eine Ebene von schachteln, aber eine Nachricht kann befinden in ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="b0d45-118">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b0d45-119">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="b0d45-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b0d45-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0d45-120">Request headers</span></span>
| <span data-ttu-id="b0d45-121">Name</span><span class="sxs-lookup"><span data-stu-id="b0d45-121">Name</span></span>       | <span data-ttu-id="b0d45-122">Typ</span><span class="sxs-lookup"><span data-stu-id="b0d45-122">Type</span></span> | <span data-ttu-id="b0d45-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0d45-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0d45-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0d45-124">Authorization</span></span>  | <span data-ttu-id="b0d45-125">string</span><span class="sxs-lookup"><span data-stu-id="b0d45-125">string</span></span>  | <span data-ttu-id="b0d45-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b0d45-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0d45-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0d45-128">Request body</span></span>
<span data-ttu-id="b0d45-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b0d45-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0d45-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0d45-130">Response</span></span>

<span data-ttu-id="b0d45-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0d45-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0d45-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0d45-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0d45-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0d45-134">Request</span></span>
<span data-ttu-id="b0d45-135">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="b0d45-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="b0d45-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0d45-136">Response</span></span>
<span data-ttu-id="b0d45-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b0d45-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
