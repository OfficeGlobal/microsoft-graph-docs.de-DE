---
title: Unterhaltungsthread erstellen
description: 'Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b47f23d8162728089934e95d9d0c4a1babc8a2a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984570"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="fd8b5-103">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="fd8b5-103">Create conversation thread</span></span>

> <span data-ttu-id="fd8b5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd8b5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd8b5-106">Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-106">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="fd8b5-p102">Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt. Verwenden Sie [Auf Thread antworten](conversationthread-reply.md) oder [Auf Beitrag antworten](post-reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-p102">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="fd8b5-109">Hinweis: Sie können auch [eine neuen Threads in einer bestehenden Unterhaltung beginnen](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="fd8b5-109">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="fd8b5-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd8b5-110">Permissions</span></span>
<span data-ttu-id="fd8b5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd8b5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd8b5-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd8b5-113">Permission type</span></span>      | <span data-ttu-id="fd8b5-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd8b5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd8b5-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd8b5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fd8b5-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd8b5-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd8b5-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd8b5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd8b5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd8b5-118">Not supported.</span></span>    |
|<span data-ttu-id="fd8b5-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd8b5-119">Application</span></span> | <span data-ttu-id="fd8b5-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd8b5-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd8b5-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd8b5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="fd8b5-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd8b5-122">Request headers</span></span>
| <span data-ttu-id="fd8b5-123">Header</span><span class="sxs-lookup"><span data-stu-id="fd8b5-123">Header</span></span>       | <span data-ttu-id="fd8b5-124">Wert</span><span class="sxs-lookup"><span data-stu-id="fd8b5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd8b5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd8b5-125">Authorization</span></span>  | <span data-ttu-id="fd8b5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd8b5-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd8b5-128">Content-Type</span></span>  | <span data-ttu-id="fd8b5-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fd8b5-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd8b5-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd8b5-130">Request body</span></span>
<span data-ttu-id="fd8b5-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an, das einen [Beitrag](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-131">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="fd8b5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd8b5-132">Response</span></span>
<span data-ttu-id="fd8b5-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-133">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd8b5-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd8b5-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fd8b5-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd8b5-135">Request</span></span>
<span data-ttu-id="fd8b5-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```

#### <a name="response"></a><span data-ttu-id="fd8b5-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd8b5-137">Response</span></span>
<span data-ttu-id="fd8b5-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-138">The following is an example of the response.</span></span>
><span data-ttu-id="fd8b5-139">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fd8b5-140">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fd8b5-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
