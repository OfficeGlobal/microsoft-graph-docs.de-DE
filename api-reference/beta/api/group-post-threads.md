---
title: Unterhaltungsthread erstellen
description: 'Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f320c465cee26ef5a91a821cd70b605f4056a9f3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517309"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="a157e-103">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="a157e-103">Create conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a157e-104">Beginnt eine neue Gruppenunterhaltung, indem zunächst ein Thread erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="a157e-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="a157e-p101">Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt. Verwenden Sie [Auf Thread antworten](conversationthread-reply.md) oder [Auf Beitrag antworten](post-reply.md), um weitere Beiträge zu diesem Thread hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="a157e-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="a157e-107">Hinweis: Sie können auch [eine neuen Threads in einer bestehenden Unterhaltung beginnen](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="a157e-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a157e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a157e-108">Permissions</span></span>
<span data-ttu-id="a157e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a157e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a157e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a157e-111">Permission type</span></span>      | <span data-ttu-id="a157e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a157e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a157e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a157e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a157e-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a157e-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a157e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a157e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a157e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a157e-116">Not supported.</span></span>    |
|<span data-ttu-id="a157e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a157e-117">Application</span></span> | <span data-ttu-id="a157e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a157e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a157e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a157e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="a157e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a157e-120">Request headers</span></span>
| <span data-ttu-id="a157e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a157e-121">Header</span></span>       | <span data-ttu-id="a157e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a157e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a157e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a157e-123">Authorization</span></span>  | <span data-ttu-id="a157e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a157e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a157e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a157e-126">Content-Type</span></span>  | <span data-ttu-id="a157e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a157e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a157e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a157e-128">Request body</span></span>
<span data-ttu-id="a157e-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [conversationThread](../resources/conversationthread.md)-Objekts an, das einen [Beitrag](../resources/post.md) enthält.</span><span class="sxs-lookup"><span data-stu-id="a157e-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="a157e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a157e-130">Response</span></span>
<span data-ttu-id="a157e-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a157e-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a157e-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a157e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a157e-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a157e-133">Request</span></span>
<span data-ttu-id="a157e-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a157e-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="a157e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a157e-135">Response</span></span>
<span data-ttu-id="a157e-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a157e-136">The following is an example of the response.</span></span>
><span data-ttu-id="a157e-137">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="a157e-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a157e-138">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a157e-138">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-threads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
