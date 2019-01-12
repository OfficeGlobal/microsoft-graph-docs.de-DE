---
title: Thread erstellen
description: Dient zum Erstellen eines neuen Threads in der angegebenen Unterhaltung.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4df6ba09df66966a741d6cff25580c0177848085
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960532"
---
# <a name="create-thread"></a><span data-ttu-id="7322e-103">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="7322e-103">Create thread</span></span>

> <span data-ttu-id="7322e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7322e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7322e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7322e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7322e-106">Dient zum Erstellen eines neuen Threads in der angegebenen Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="7322e-106">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="7322e-p102">Ein Thread und ein Beitrag werden wie angegeben erstellt. Verwenden Sie [Auf Thread antworten](conversationthread-reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen. Wenn Sie die Beitrags-ID abrufen, können Sie auch auf diesen Beitrag in diesem Thread [antworten](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="7322e-p102">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="7322e-110">Hinweis: Sie können auch [eine neue Unterhaltung beginnen, indem Sie zuerst einen Thread erstellen](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="7322e-110">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7322e-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7322e-111">Permissions</span></span>
<span data-ttu-id="7322e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7322e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7322e-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7322e-114">Permission type</span></span>      | <span data-ttu-id="7322e-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7322e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7322e-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7322e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7322e-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7322e-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7322e-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7322e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7322e-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7322e-119">Not supported.</span></span>    |
|<span data-ttu-id="7322e-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7322e-120">Application</span></span> | <span data-ttu-id="7322e-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7322e-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7322e-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7322e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="7322e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7322e-123">Request headers</span></span>
| <span data-ttu-id="7322e-124">Name</span><span class="sxs-lookup"><span data-stu-id="7322e-124">Name</span></span>       | <span data-ttu-id="7322e-125">Typ</span><span class="sxs-lookup"><span data-stu-id="7322e-125">Type</span></span> | <span data-ttu-id="7322e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7322e-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7322e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7322e-127">Authorization</span></span>  | <span data-ttu-id="7322e-128">string</span><span class="sxs-lookup"><span data-stu-id="7322e-128">string</span></span>  | <span data-ttu-id="7322e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7322e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7322e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7322e-131">Request body</span></span>
<span data-ttu-id="7322e-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7322e-132">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7322e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7322e-133">Response</span></span>

<span data-ttu-id="7322e-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7322e-134">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7322e-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7322e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7322e-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7322e-136">Request</span></span>
<span data-ttu-id="7322e-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7322e-137">Here is an example of the request.</span></span>
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
<span data-ttu-id="7322e-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7322e-138">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7322e-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="7322e-139">Response</span></span>

<span data-ttu-id="7322e-p105">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das `id` im Antworttext zurückgegeben. Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7322e-p105">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
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
