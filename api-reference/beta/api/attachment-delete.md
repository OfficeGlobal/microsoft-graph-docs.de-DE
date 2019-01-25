---
title: Anlage löschen
description: Löschen Sie eine Anlage aus einer Kalenderereignis, Nachricht, Outlook-Aufgabe oder Post.
localization_priority: Normal
ms.openlocfilehash: 5bb24fc97a2f99dbb0fbec77e2de941f770c27fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510897"
---
# <a name="delete-attachment"></a><span data-ttu-id="93c9e-103">Anlage löschen</span><span class="sxs-lookup"><span data-stu-id="93c9e-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93c9e-104">Löschen einer Anlage aus einem Kalender- [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="93c9e-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93c9e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="93c9e-105">Permissions</span></span>

<span data-ttu-id="93c9e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93c9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="93c9e-108">Beim Zugriff auf Anlagen in Nachrichten: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93c9e-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="93c9e-109">Beim Zugriff auf Anlagen in Ereignissen: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93c9e-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="93c9e-110">Wenn auf Anlagen in Outlook-Aufgaben zugreifen: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93c9e-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="93c9e-111">Wenn Anlagen in der Gruppe Beiträge zugreifen: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c9e-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="93c9e-112">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93c9e-112">HTTP request</span></span>

<span data-ttu-id="93c9e-113">Anlagen für ein [Ereignis](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="93c9e-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="93c9e-114">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="93c9e-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="93c9e-115">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="93c9e-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="93c9e-p102">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="93c9e-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. <!-- { "blockType": "ignored" } --></span></span>

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="93c9e-118">Anlagen für ein [Outlook-Aufgabe](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="93c9e-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="93c9e-119">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="93c9e-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93c9e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93c9e-120">Request headers</span></span>

| <span data-ttu-id="93c9e-121">Name</span><span class="sxs-lookup"><span data-stu-id="93c9e-121">Name</span></span>       | <span data-ttu-id="93c9e-122">Typ</span><span class="sxs-lookup"><span data-stu-id="93c9e-122">Type</span></span> | <span data-ttu-id="93c9e-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93c9e-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="93c9e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="93c9e-124">Authorization</span></span>  | <span data-ttu-id="93c9e-125">string</span><span class="sxs-lookup"><span data-stu-id="93c9e-125">string</span></span>  | <span data-ttu-id="93c9e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="93c9e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93c9e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93c9e-128">Request body</span></span>

<span data-ttu-id="93c9e-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="93c9e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93c9e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="93c9e-130">Response</span></span>

<span data-ttu-id="93c9e-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93c9e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93c9e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93c9e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="93c9e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93c9e-134">Request</span></span>

<span data-ttu-id="93c9e-135">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="93c9e-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="93c9e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="93c9e-136">Response</span></span>

<span data-ttu-id="93c9e-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93c9e-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
