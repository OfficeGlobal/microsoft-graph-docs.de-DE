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
# <a name="delete-attachment"></a>Anlage löschen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Löschen einer Anlage aus einem Kalender- [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md).
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

* Wenn Anlagen in Nachrichten zugreifen: Mail.ReadWrite
* Wenn das Zugreifen auf Anlagen in Ereignisse: Calendars.ReadWrite
* Wenn auf Anlagen in Outlook-Aufgaben zugreifen: Tasks.ReadWrite
* Wenn Anlagen in der Gruppe Beiträge zugreifen: Group.ReadWrite.All
<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a>HTTP-Anforderung
Anlagen für ein [Ereignis](../resources/event.md) in der Benutzer als [Kalender](../resources/calendar.md).

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

Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
Anlagen für eine [Nachricht](../resources/message.md) , die in einem untergeordneten Ordner von einem [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers enthalten sind.  Das folgende Beispiel zeigt eine Ebene von schachteln, aber eine Nachricht kann befinden in ein untergeordnetes Element des ein untergeordnetes Element und so weiter.
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

Anlagen für [Outlook-Aufgabe](../resources/outlooktask.md) in das Postfach des Benutzers oder in einem angegebenen Ordner oder "Task Group".
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
```

Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
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