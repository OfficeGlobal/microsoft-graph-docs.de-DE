---
title: Anlage löschen
description: Löschen einer Anlage aus einem Kalenderereignis
ms.openlocfilehash: 5e5fe0205e667908947993b01388f90c1688c95e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058719"
---
# <a name="delete-attachment"></a><span data-ttu-id="3adb8-103">Anlage löschen</span><span class="sxs-lookup"><span data-stu-id="3adb8-103">Delete attachment</span></span>

> <span data-ttu-id="3adb8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3adb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3adb8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3adb8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3adb8-106">Löschen einer Anlage aus einem Kalender- [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="3adb8-106">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3adb8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3adb8-107">Permissions</span></span>
<span data-ttu-id="3adb8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3adb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="3adb8-110">Wenn Anlagen in Nachrichten zugreifen: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3adb8-110">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="3adb8-111">Wenn das Zugreifen auf Anlagen in Ereignisse: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3adb8-111">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="3adb8-112">Wenn auf Anlagen in Outlook-Aufgaben zugreifen: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3adb8-112">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="3adb8-113">Wenn Anlagen in der Gruppe Beiträge zugreifen: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3adb8-113">If accessing attachments in group posts: Group.ReadWrite.All</span></span>
<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="3adb8-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3adb8-114">HTTP request</span></span>
<span data-ttu-id="3adb8-115">Anlagen für ein [Ereignis](../resources/event.md) in der Benutzer als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="3adb8-115">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
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

<span data-ttu-id="3adb8-116">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="3adb8-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="3adb8-117">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="3adb8-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="3adb8-118">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="3adb8-118">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="3adb8-119">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="3adb8-119">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="3adb8-120">Anlagen für eine [Nachricht](../resources/message.md) , die in einem untergeordneten Ordner von einem [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="3adb8-120">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="3adb8-121">Das folgende Beispiel zeigt eine Ebene von schachteln, aber eine Nachricht kann befinden in ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="3adb8-121">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="3adb8-122">Anlagen für [Outlook-Aufgabe](../resources/outlooktask.md) in das Postfach des Benutzers oder in einem angegebenen Ordner oder "Task Group".</span><span class="sxs-lookup"><span data-stu-id="3adb8-122">Attachments for an [Outlook task](../resources/outlooktask.md) in the user's mailbox, or in a specified task folder or task group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
```

<span data-ttu-id="3adb8-123">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="3adb8-123">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3adb8-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3adb8-124">Request headers</span></span>
| <span data-ttu-id="3adb8-125">Name</span><span class="sxs-lookup"><span data-stu-id="3adb8-125">Name</span></span>       | <span data-ttu-id="3adb8-126">Typ</span><span class="sxs-lookup"><span data-stu-id="3adb8-126">Type</span></span> | <span data-ttu-id="3adb8-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3adb8-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3adb8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="3adb8-128">Authorization</span></span>  | <span data-ttu-id="3adb8-129">string</span><span class="sxs-lookup"><span data-stu-id="3adb8-129">string</span></span>  | <span data-ttu-id="3adb8-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3adb8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3adb8-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3adb8-132">Request body</span></span>
<span data-ttu-id="3adb8-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3adb8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3adb8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3adb8-134">Response</span></span>

<span data-ttu-id="3adb8-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3adb8-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3adb8-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3adb8-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3adb8-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3adb8-138">Request</span></span>
<span data-ttu-id="3adb8-139">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="3adb8-139">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="3adb8-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="3adb8-140">Response</span></span>
<span data-ttu-id="3adb8-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3adb8-141">Here is an example of the response.</span></span>
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
