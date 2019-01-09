---
title: Anlage löschen
description: Löschen Sie eine Anlage aus einer Kalenderereignis, Nachricht, Outlook-Aufgabe oder Post.
ms.openlocfilehash: dbabde6b1783e477e3a15db3ea4d138be6e41b12
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771786"
---
# <a name="delete-attachment"></a><span data-ttu-id="43f7d-103">Anlage löschen</span><span class="sxs-lookup"><span data-stu-id="43f7d-103">Delete attachment</span></span>

> <span data-ttu-id="43f7d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="43f7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43f7d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43f7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43f7d-106">Löschen einer Anlage aus einem Kalender- [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="43f7d-106">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="43f7d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="43f7d-107">Permissions</span></span>

<span data-ttu-id="43f7d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43f7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="43f7d-110">Wenn Anlagen in Nachrichten zugreifen: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43f7d-110">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="43f7d-111">Wenn das Zugreifen auf Anlagen in Ereignisse: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43f7d-111">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="43f7d-112">Wenn auf Anlagen in Outlook-Aufgaben zugreifen: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43f7d-112">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="43f7d-113">Wenn Anlagen in der Gruppe Beiträge zugreifen: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f7d-113">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="43f7d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43f7d-114">HTTP request</span></span>

<span data-ttu-id="43f7d-115">Anlagen für ein [Ereignis](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="43f7d-115">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="43f7d-116">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="43f7d-116">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="43f7d-117">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="43f7d-117">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="43f7d-118">Anlagen für eine [Nachricht](../resources/message.md) , die in einem untergeordneten Ordner von einem [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="43f7d-118">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="43f7d-119">Das folgende Beispiel zeigt eine Ebene von schachteln, aber eine Nachricht kann befinden in ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="43f7d-119">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="43f7d-120">Anlagen für ein [Outlook-Aufgabe](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="43f7d-120">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="43f7d-121">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="43f7d-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="43f7d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43f7d-122">Request headers</span></span>

| <span data-ttu-id="43f7d-123">Name</span><span class="sxs-lookup"><span data-stu-id="43f7d-123">Name</span></span>       | <span data-ttu-id="43f7d-124">Typ</span><span class="sxs-lookup"><span data-stu-id="43f7d-124">Type</span></span> | <span data-ttu-id="43f7d-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43f7d-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43f7d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="43f7d-126">Authorization</span></span>  | <span data-ttu-id="43f7d-127">string</span><span class="sxs-lookup"><span data-stu-id="43f7d-127">string</span></span>  | <span data-ttu-id="43f7d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="43f7d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43f7d-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43f7d-130">Request body</span></span>

<span data-ttu-id="43f7d-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="43f7d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43f7d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="43f7d-132">Response</span></span>

<span data-ttu-id="43f7d-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43f7d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f7d-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43f7d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="43f7d-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43f7d-136">Request</span></span>

<span data-ttu-id="43f7d-137">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="43f7d-137">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="43f7d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="43f7d-138">Response</span></span>

<span data-ttu-id="43f7d-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43f7d-139">Here is an example of the response.</span></span>
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
