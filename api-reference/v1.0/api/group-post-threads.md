---
title: Unterhaltungsthread erstellen
description: 'Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 34a38c0700eeb9ab1074a2f7cb2b396168266c97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922298"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="0f026-103">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="0f026-103">Create conversation thread</span></span>
<span data-ttu-id="0f026-104">Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="0f026-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="0f026-p101">Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt. Verwenden Sie [Auf Thread antworten](conversationthread-reply.md) oder [Auf Beitrag antworten](post-reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="0f026-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="0f026-107">Hinweis: Sie können auch [eine neuen Threads in einer bestehenden Unterhaltung beginnen](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="0f026-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0f026-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f026-108">Permissions</span></span>
<span data-ttu-id="0f026-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f026-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f026-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f026-111">Permission type</span></span>      | <span data-ttu-id="0f026-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f026-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f026-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f026-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0f026-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f026-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f026-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f026-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f026-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f026-116">Not supported.</span></span>    |
|<span data-ttu-id="0f026-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f026-117">Application</span></span> | <span data-ttu-id="0f026-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f026-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f026-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f026-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="0f026-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f026-120">Request headers</span></span>
| <span data-ttu-id="0f026-121">Header</span><span class="sxs-lookup"><span data-stu-id="0f026-121">Header</span></span>       | <span data-ttu-id="0f026-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0f026-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f026-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f026-123">Authorization</span></span>  | <span data-ttu-id="0f026-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f026-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f026-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f026-126">Content-Type</span></span>  | <span data-ttu-id="0f026-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0f026-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f026-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f026-128">Request body</span></span>
<span data-ttu-id="0f026-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an, das einen [Beitrag](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="0f026-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="0f026-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f026-130">Response</span></span>
<span data-ttu-id="0f026-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f026-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f026-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f026-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0f026-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f026-133">Request</span></span>
<span data-ttu-id="0f026-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f026-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
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
#### <a name="response"></a><span data-ttu-id="0f026-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f026-135">Response</span></span>
<span data-ttu-id="0f026-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f026-136">The following is an example of the response.</span></span>
><span data-ttu-id="0f026-137">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="0f026-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0f026-138">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0f026-138">All the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
