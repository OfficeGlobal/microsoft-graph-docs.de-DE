---
title: Thread erstellen
description: Dient zum Erstellen eines neuen Threads in der angegebenen Unterhaltung.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: cfd71883849fc820958a2d9548d865a23802bf52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824801"
---
# <a name="create-thread"></a><span data-ttu-id="e4b10-103">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="e4b10-103">Create thread</span></span>

> <span data-ttu-id="e4b10-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4b10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4b10-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4b10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4b10-106">Dient zum Erstellen eines neuen Threads in der angegebenen Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="e4b10-106">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="e4b10-p102">Ein Thread und ein Beitrag werden wie angegeben erstellt. Verwenden Sie [Auf Thread antworten](conversationthread-reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen. Wenn Sie die Beitrags-ID abrufen, können Sie auch auf diesen Beitrag in diesem Thread [antworten](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="e4b10-p102">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="e4b10-110">Hinweis: Sie können auch [eine neue Unterhaltung beginnen, indem Sie zuerst einen Thread erstellen](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="e4b10-110">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4b10-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4b10-111">Permissions</span></span>
<span data-ttu-id="e4b10-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4b10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4b10-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4b10-114">Permission type</span></span>      | <span data-ttu-id="e4b10-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4b10-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4b10-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4b10-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e4b10-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b10-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4b10-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4b10-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4b10-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4b10-119">Not supported.</span></span>    |
|<span data-ttu-id="e4b10-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4b10-120">Application</span></span> | <span data-ttu-id="e4b10-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b10-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4b10-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4b10-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="e4b10-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4b10-123">Request headers</span></span>
| <span data-ttu-id="e4b10-124">Name</span><span class="sxs-lookup"><span data-stu-id="e4b10-124">Name</span></span>       | <span data-ttu-id="e4b10-125">Typ</span><span class="sxs-lookup"><span data-stu-id="e4b10-125">Type</span></span> | <span data-ttu-id="e4b10-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4b10-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e4b10-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4b10-127">Authorization</span></span>  | <span data-ttu-id="e4b10-128">string</span><span class="sxs-lookup"><span data-stu-id="e4b10-128">string</span></span>  | <span data-ttu-id="e4b10-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4b10-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4b10-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4b10-131">Request body</span></span>
<span data-ttu-id="e4b10-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4b10-132">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e4b10-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4b10-133">Response</span></span>

<span data-ttu-id="e4b10-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4b10-134">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4b10-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4b10-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4b10-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4b10-136">Request</span></span>
<span data-ttu-id="e4b10-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4b10-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="e4b10-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4b10-138">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e4b10-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4b10-139">Response</span></span>

<span data-ttu-id="e4b10-p105">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das `id` im Antworttext zurückgegeben. Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e4b10-p105">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
